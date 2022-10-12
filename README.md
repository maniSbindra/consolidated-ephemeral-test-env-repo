
# Repository for completely isolated ephemeral environment creation solution

This repository includes all other repositories involved in the solution as git subtrees. The aim is to make testing the solution easier by cloning just a single repository.

## Index 
Folders and associated git sub trees for the nested repositories

|  Sr No. | FolderName  | Repo  | Description  |
|---|---|---|---|
|  1. |  sample-app-source-repo | [ephemeral-app](https://github.com/maniSbindra/ephemeral-app)  | Repository containing Sample Application code, docker file, and application team owned manifests to test creation of ephemreal testing environments |
|  2. |  environment-infra-helm-repo | [ephemeral-env-infra](https://github.com/maniSbindra/ephemeral-env-infra)  |This is the Infrastructure repository which contains the manifests / templates to provision the cloud services / resources needed for the ephemeral environment creation, when PR is created against the sample application repository  |
|  3. |  e2e-solution-setup |  [ephemeral-mgmt](https://github.com/maniSbindra/ephemeral-mgmt) | This is the Management repository which contains scripts to bootstrap 2 of the solutions to create completely isolated ephemeral test environments, using different tooling (one Argo CD based and one Flux based) |
|  4. |  sample-flux-pr-eph-env-controller | [pr-ephemeral-env-controller](https://github.com/maniSbindra/pr-ephemeral-env-controller)  | This is a **sample** PR ephemeral environment controller source code repository. This controller is used by the flux based solution. |adding line to  markdown for testing 8
