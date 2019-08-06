# how to build a container in cloud build

Set-up your repository, and then set-up your project to use a trigger (in cloud build).
Choose the option:

```option
Cloud Build configuration file (yaml or json)
Specify the path to a Cloud Build configuration file
```

Then update **cloudbuild.yaml**:

```yaml
  args: ['build', '--tag=gcr.io/<project>/<container>', '.']
images: ['gcr.io/<project>/<container>']
```

With your project and container name.
