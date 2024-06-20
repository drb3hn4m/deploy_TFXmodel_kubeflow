# deploy a TFX model on Vertex ai with Kubeflow
- this deployment is based on the [the other project in the repo](https://github.com/drb3hn4m/classifier_tfx_vertex)
- This modern version of deployment with tfx pipline on VERTEX ai using kfp directly to the endpoint eliminates the need of programatically creating endpoint, model and then deploying the model to the endpoint with gcloud cmd.

- it takes advantages of newly added 'tfx.extensions.google_cloud_ai_platform' modules and the configuration to achieve that
- the deployment process may takes up to 15 minutes. The progress can be monitored via pipelines tab in Vertex AI which shows a DAG of the pipeline. Make sure that all components have labelled green before trying the predicitons.
- Three methods for for making predicitons are provided in a separate notebook