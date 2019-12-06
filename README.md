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
 - In order to deploy the pipeline it is strongly recommended you have python3.7+, virtualenv,  AWS CLI and ruby (version >= 2.3) installed.
   - These are nessecary to utilize any of the automated deployment options.

## Installation

Once you have installed the relevant prerequisites, you can either:

1. Clone the Unicorn-Pipeline at: https://github.com/unicorn-ca/Unicorn-Pipeline and run the build script yourself.
2. Run the following line of shell code to download and run the build script.

### Installing via Curl

Install and run wizard.

```shell
curl https://raw.githubusercontent.com/unicorn-ca/Unicorn-Pipeline/master/build > tmp.sh; sh tmp.sh -w
```

The launch wizard should automatically open in your browser. If this doesn't work for you, try doing a headless install.

### Headless Install

Install the pipeline without running the wizard by removing the -w flag.

```shell
curl https://raw.githubusercontent.com/unicorn-ca/Unicorn-Pipeline/master/build > tmp.sh; sh tmp.sh
``` 

## Contribution

Please read our [contribution guidelines](https://github.com/unicorn-ca/Unicorn-docs/blob/master/CONTRIBUTING.md) before creating an issue or pull request!
