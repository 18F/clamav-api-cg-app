# ClamAV API CG App

## Setup

### Create apps

`cf push`

### Configure networking

A network policy is required to route the TCP traffic from the rest app to the clamd server

`cf add-network-policy clamav-rest --destination-app clamav-server --protocol tcp --port 3310`

## Why this project

This project aims to create a deployable cloud.gov app that will expose a REST api for scanning files for malware with ClamAV.

It is inspired by, and borrows heavily from, https://blog.theodo.com/2017/11/implement-antivirus-api-10-min/


## Contributing

See [CONTRIBUTING](CONTRIBUTING.md) for additional information.

## Public domain

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
