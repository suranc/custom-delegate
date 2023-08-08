# custom-delegate

## .harness/custom_delegate.yaml

This pipeline fetches the lastest supported delegate image for your harness account and then builds your custom delegate image from the Dockerfile specified. It then pushes the resulting image and sets the default delegate image on your account to the resulting image and tag. This will direct your delegate-auto-upgrader to pull your custom image rather than Harness' public image.

## Dockerfile.maximum

This adds all the tools necessary for the Harness platform that are not part of the base image to the minimal delegate. You can remove tools for features you don't use or update versions for your requirements.
