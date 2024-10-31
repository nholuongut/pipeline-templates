# Azure Devops Pipeline Templates

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

This repository contains templates and examples for creating Azure Devops pipelines. You can easily create templates using job templates in the `templates` directory as building blocks. Usage examples of each job templates are available withing the `examples` directory along with more complete examples in the `examples/complete` directory.

The templates cover the following use cases:

- Building, testing a dotnet project
- Building and pushing a Docker image

## How to use a template in this repositotry

Firstly you will need to create a service connection to GitHub in your Azure Devops project settings. After that, follow any of the examples in the `examples` directory and make sure to include the following configuration in your pipeline YAML file:

```yaml
resources:
  repositories:
    - repository: pipeline-templates
      name: nholuongut/pipeline-templates
      type: github
      endpoint: githubServiceConnection
      # We recommend pinning the template to a specific version
      # ref: refs/tags/1.0.0
```

## Breaking Changes

Please consult [BREAKING_CHANGES.md](BREAKING_CHANGES.md) for more information about version history and compatibility.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on the process for
contributing to this project.

Be mindful of our [Code of Conduct](CODE_OF_CONDUCT.md).

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟