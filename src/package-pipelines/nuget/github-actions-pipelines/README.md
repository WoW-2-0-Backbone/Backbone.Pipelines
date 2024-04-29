# Package Deployment to Nuget via Github Actions

These are deployment pipelines to package and publish .NET projects to Nuget public package repository using Github Actions

## Nuget Deployment Pipelines

### Pre-Release Test Pipeline

**Template** - [Template file](./build-and-publish-prerelease.yml)

- Trigger - `push`, `workflow_dispatch` - pipeline is triggered by any pushed commit or manually
- Trigger source - `src/**` - for any file change in `src` folder
- Target branch - `dev` - pipeline is triggered only for changes in `dev` branch
- Secrets - `NUGET_API_KEY` - your Nuget account API key

#### Pipeline Steps

**Build and Test** job

- Checks out latest code
- Sets up .NET Core environment
- Restores dependencies
- Builds the solution file
- Runs tests

**Publish PreRelease** job

- Checks out latest code
- Finds packable projects by checking for `<PackageId>` in `csproj` project files
- [Packs and Publishes each package](#pack-and-publish-step)

#### Pack and Publish step

- Extracts package Id
- Extracts package version
- [Validates package version](#package-version-validations)
- Packs the package
- Publishes to nuget

#### Package Version Validations

| Validation | Status |
|---------|--------|
| Validate if `Version` value exists for package | ✅ |
| Validate Major Number in version is equal to .NET Version | ✅ |
| Validate and skip if package version isn't changed  | ✅  |
| Validate version has `alpha` suffix | ✅  |
| Validate Minor and Patch numbers are equal or greater than latest if latest publish was alpha | ✅ |
| Validate Alpha number is 0 if current Minor or Patch versions are higher | ✅ |
| Validate Alpha number is higher if current Minor or Patch versions are equal to the latest version | ✅ |
| Validate Minor or Patch number must be one higher if the latest version is release version | ✅ |
| Validate Alpha number is 0 if the latest version is release version | ✅ |
| Validate Minor, Patch and Alpha numbers are all 0 if this is the first publish | ✅ |