# Unicorn Documentation

Documentation for deployment and usage of the unicorn pipeline.

## General prerequisites
In order to use the pipeline, you need to have some existing AWS infrastructure setup
 - You must have 3 separate AWS accounts. The accounts should be allocated into a single organization
   - See [here](https://google.com) for more details on how to do this
 - The pipeline should not utilize more resources than an account has by default. See [here](https://google.com) for a a resource utilization list.
 - In order to deploy the pipeline it is strongly recommended you have python3.7+ installed.
   - This is nessecary to utilize any of the automated deployment options.
