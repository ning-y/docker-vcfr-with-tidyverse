# docker-vcfr-with-tidyverse

Docker image for the [vcfR](https://cran.r-project.org/web/packages/vcfR/vcfR.pdf) R package, built on a [rocker/tidyverse](https://hub.docker.com/r/rocker/tidyverse) base.

These images are tagged by vcfR version number.
For more information, please see [the Docker Hub page](https://hub.docker.com/r/docker/ningyuan/vcfr-with-tidyverse).

## Development

Some notes for myself:

- Build this image by passing the Dockerfile through `STDIN`: `docker build -t ningyuan/vcfr-with-tidyverse:1.12.0 - < Dockerfile`.
  This way, there will be no build context (which is a good thing).
- Tag and release this GitHub repository with each new Docker tag.
  This is just good practice.
