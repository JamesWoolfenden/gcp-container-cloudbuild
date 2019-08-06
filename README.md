# how to build a container in cloud build

Set-up you repository and set your project to use a trigger(in cloud build):

```option
Cloud Build configuration file (yaml or json)
Specify the path to a Cloud Build configuration file
```

Update cloudbuild.yaml:

```yaml
  args: ['build', '--tag=gcr.io/<project>/<container>', '.']
images: ['gcr.io/<project>/<container>']
```

With your project and container name.