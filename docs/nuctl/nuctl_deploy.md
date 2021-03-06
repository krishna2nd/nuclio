## nuctl deploy

Build, deploy and run a function

### Synopsis


Build, deploy and run a function

```
nuctl deploy function-name [flags]
```

### Options

```
      --base-image string       Name of base image. If empty, per-runtime default is used
      --build-command String    Commands to run on build of processor image
      --data-bindings string    JSON encoded data bindings for the function (default "{}")
      --desc string             Function description
  -d, --disabled                Start function disabled (don't run yet)
  -e, --env string              Environment variables (name1=val1,name2=val2..)
  -f, --file string             Function configuration file
      --handler string          Name of handler
  -h, --help                    help for deploy
  -i, --image string            Docker image name, will use function name if not specified
  -l, --labels string           Additional function labels (lbl1=val1,lbl2=val2..)
      --max-replicas int        Maximum number of function replicas
      --min-replicas int        Minimum number of function replicas
      --no-pull                 Don't pull base images - use local versions
      --nuclio-src-dir string   Local directory with nuclio sources (avoid cloning)
      --nuclio-src-url string   nuclio sources url for git clone (default "https://github.com/nuclio/nuclio.git")
  -o, --output string           Build output type - docker|binary (default "docker")
  -p, --path string             Function source code path
      --port int                Public HTTP port (node port)
      --publish                 Publish the function
  -r, --registry string         URL of container registry (env: NUCTL_REGISTRY)
      --replicas int            If set, number of replicas is static (default 1)
      --run-image string        If specified, this is the image that the deploy will use, rather than try to build one
      --run-registry string     The registry URL to pull the image from, if differs from -r (env: NUCTL_RUN_REGISTRY)
      --runtime string          Runtime (e.g. golang, golang:1.8, python:2.7)
      --triggers string         JSON encoded triggers for the function (default "{}")
      --version string          Docker image version (default "latest")
```

### Options inherited from parent commands

```
  -k, --kubeconfig string   Path to Kubernetes config (admin.conf)
  -n, --namespace string    Kubernetes namespace (default "default")
      --platform string     One of kube/local/auto (default "auto")
  -v, --verbose             verbose output
```

### SEE ALSO
* [nuctl](nuctl.md)	 - nuclio command line interface

###### Auto generated by spf13/cobra on 1-Nov-2017
