# Pipeline for dotnet backend on Docker

This pipeline is an example that can be used to build, publish and deploy a dotnet backend runing in a Docker container.

## Usage

Firstly make sure you create a service connection to your Docker registry (Azure Container Registry, AWS Elastic Container Registry, DockerHub, etc.) Note the name of the registry.

You should create a variable group named Backend (or whatever is more convineant) and include the following variables. Note that your pipeline will be more flexible if you use Azure Devops variables library instead of hard coding these values within your pipeline. You can even consider spliting the variables into multiple variable groups.

- `projectPath`: value should be the path of the main project you want to build
- `projectsToTest`: value shoud be a pattern where your source code resides, i.e.: `$(Build.SourcesDirectory)/src/*Tests/*.csproj` 
- `dockerSerivceConnection`: the name of the service connection to your Docker registry you created earlier
- `imageRepository`: the name of the repository where to push
