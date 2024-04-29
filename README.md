[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<br />
<div align="center">

  <h3 align="center">Deployment CI/CD Pipelines</h3>

  <p align="center">
    Awesome tested and working examples of CI/CD pipelines to jumpstart your projects!
    <br />
    <a href="https://github.com/WoW-2-0"><strong>About our Community»</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    <a href="https://github.com/othneildrew/Best-README-Template/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    <a href="https://github.com/othneildrew/Best-README-Template/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About Deployment Pipelines</a>
      <ul>
        <li><a href="#why">Why</a></li>
      </ul>
      <ul>
        <li><a href="#built-with">How to create your pipeline</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About Deployment Pipelines

There are many deployment pipeline templates, available on open source projects, blogs, however we didn't find most of them not suitable for our needs so we created this ready pipelines source. Currently most of the pipelines we use will is stored here, but we may switch to different approaches or DevOps platforms in future. 

### Why

Here's why:
* When starting a project, we found ourselves to spend more resources on setting up a deployment pipeline rather brainstorming
* Most of the advanced pipelines for enterprise projects where budget of cloud resources didn't have an impact on their deployment strategy
* We want to implement DRY principles our delivery workflow: 🙃

## Getting Started

### Available pipelines

#### Package deployment

- [Deployment to Nuget using Github Actions](./src/package-pipelines/nuget/github-actions-pipelines/README.md)

#### Service deployment

This is an example of using Nuget prerelease pipeline to build and test your project and pack and publish it to package source you want

Copy the pipeline

## Usage

Simply a choose pipeline for your need, copy the template, change necessary variables and set up with your favorite platform.

For details refer 

## Roadmap

- [x] Add package to Nuget release and pre-release pipelines
- [ ] Add package to Github Packages release and pre-release pipelines
- [ ] Add service to Azure deployment release and pre-release pipelines
- [ ] Add service to Docker and Azure Hybrid release and pre-release pipelines

See the [open issues](https://github.com/WoW-2-0-Backbone/Backbone.Pipelines/issues) for a full list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

## License

Distributed under the MIT License. See [License](./LICENSE.txt) for more information.

## Contact

See [Community Team and Contacts](sultonbek_rakhimov)

## Acknowledgments

These pipelines are not ready for production use and might have security issues. They are primarily intended for development and learning purposes, to have basic pipelines to jumpstart projects. 

While every effort has been made to ensure the quality and safety of these pipelines, they should be thoroughly reviewed and tested in a controlled environment before considering them for a production scenario. 

[contributors-shield]: https://img.shields.io/github/contributors/WoW-2-0-Backbone/Backbone.Pipelines.svg?style=for-the-badge
[contributors-url]: https://github.com/WoW-2-0-Backbone/Backbone.Pipelines/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/WoW-2-0-Backbone/Backbone.Pipelines.svg?style=for-the-badge
[forks-url]: https://github.com/WoW-2-0-Backbone/Backbone.Pipelines/network/members
[stars-shield]: https://img.shields.io/github/stars/WoW-2-0-Backbone/Backbone.Pipelines.svg?style=for-the-badge
[stars-url]: https://github.com/WoW-2-0-Backbone/Backbone.Pipelines/stargazers
[issues-shield]: https://img.shields.io/github/issues/WoW-2-0-Backbone/Backbone.Pipelines.svg?style=for-the-badge
[issues-url]: https://github.com/WoW-2-0-Backbone/Backbone.Pipelines/issues
[license-shield]: https://img.shields.io/github/license/WoW-2-0-Backbone/Backbone.Pipelines.svg?style=for-the-badge
[license-url]: https://github.com/WoW-2-0-Backbone/Backbone.Pipelines/main/LICENSE.txt