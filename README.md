# k8s_manifest_templates

| NAME                     | PROMPT                                                    | DESCRIPTION                                                                  | EXAMPLE                                   |
|--------------------------|-----------------------------------------------------------|------------------------------------------------------------------------------|-------------------------------------------|
| app.yaml                 | a template Pod in a template namespace with default 'demo' image from gcr.io and maximum data and detalisation. | Defines the basic configuration for an application in Kubernetes            | [app.yaml](yaml/app.yaml?raw=true)             |
| app-livenessProbe.yaml   | a Pod with a liveness probe, which is used to check the health of the container running in the Pod via http request for specific path           | Configures liveness probes to check the health of the application            | [app-livenessProbe.yaml](yaml/app-livenessProbe.yaml?raw=true) |
| app-readinessProbe.yaml  | a Pod with a readiness probe          | Sets up readiness probes to ensure the application is ready to serve traffic | [app-readinessProbe.yaml](yaml/app-readinessProbe.yaml?raw=true) |
| app-volumeMounts.yaml    | a Pod with a several volume mounts of different types            | Defines volume mounts for the application                                    | [app-volumeMounts.yaml](yaml/app-volumeMounts.yaml?raw=true) |
| app-cronjob.yaml         | a template Pod in a template namespace with detailed cronjob and default demo image                 | Sets up a cron job within Kubernetes                                         | [app-cronjob.yaml](yaml/app-cronjob.yaml?raw=true) |
| app-job.yaml             | a Job which mounts volume and run rsync comman                     | Configures a Kubernetes job for running rsync with a volume| [app-job.yaml](yaml/app-job.yaml?raw=true)     |
| app-multicontainer.yaml  | a multi-container Pod configuration with volume         | Defines a pod with multiple containers and shared volume| [app-multicontainer.yaml](yaml/app-multicontainer.yaml?raw=true) |
| app-resources.yaml       | a Pod with specific configurations for resource allocation, health checks, and networking, etc               | Specifies resource requests and limits for the application                   | [app-resources.yaml](yaml/app-resources.yaml?raw=true) |
| app-secret-env.yaml      | a Pod named app-secret that utilizes a secret volume      | Manages sensitive information  in several ways, such as environment variables or as files in a volume.         | [app-secret-env.yaml](yaml/app-secret-env.yaml?raw=true) |

