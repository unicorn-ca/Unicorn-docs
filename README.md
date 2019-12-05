# Unicorn Documentation

Documentation for deployment and usage of the unicorn pipeline.

## GitHub Repository

We have multiple repositories in our GitHub. An basic outline of them are:

- _Unicorn-Pipeline_: Our CA pipeline
- _Stable_: The launch wizard and pipeline installation
- _Saddle_: an AWS Cloud-Formation validator
- _Reins_: Stage-based auditing
- _Horn_: Property-based fuzzer

## General prerequisites
In order to use the pipeline, you need to have some existing AWS infrastructure setup
 - You must have 3 separate AWS accounts. The accounts should be allocated into a single organization.
   Create a IAM User for each account.
   - See [here](https://aws.amazon.com/cli/) for more details on how to do this
 - The pipeline should not utilize more resources than an account has by default. See [here](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Using_Filtering.html) for a a resource utilization list.
 - In order to deploy the pipeline it is strongly recommended you have python3.7+ installed.
   - This is nessecary to utilize any of the automated deployment options.

## Contribution

Please read our [contribution guidelines](https://github.com/unicorn-ca/Unicorn-docs/blob/master/CONTRIBUTING.md) before creating an issue or pull request!
