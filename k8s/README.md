## Build the pipeline


1. **Setup parameters** Alter, or copy the _namerequest-build-pipeline.param_ updating the values for your pipeline.
2. **Create the pipeline** process the template referencing your parameter file.

```bash
oc process -f templates/pipeline.yaml --param-file=namerequest-ui-pipeline.param  | oc create -f -
```
