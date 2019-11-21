# Quickstart
Get quickly setup with Unicorn using Saddle and Herd.

**Ensure that you have met the general requirements specified on the repository** [**README**](https://google.com)

## 1. Dependancies
The automated build script depends on a few external tools in addition to the general requirements.
Ensure these are installed before proceeding.
 - git
 - python3.7+
 - ruby
 - sh style shell (sh, bash, zsh, ...)

## 2. Setup your AWS credentials
The Unicorn-Pipeline will never interact directly with your AWS credentials.
You will need to setup at least 3 profiles corresponding with each of the AWS account's IAM Users.
You can set these up with `aws configure --profile=my-role-profile`. Take note of the each of the profile
names.

## 2. Run the deployment script
The automated build script can be download here [here](https://google.com), this can be automated using `curl`.

On \*ix based systems run:
```
$ curl https://buildlocation | sh
```

On WSL systems run:
```
$ curl https://buildlocation | bash
```

## 3. Follow the wizard
TODO

The pipeline should now be deployed into your master aws account.
