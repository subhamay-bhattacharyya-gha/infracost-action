## [1.0.1](https://github.com/subhamay-bhattacharyya-gha/infracost-action/compare/v1.0.0...v1.0.1) (2025-06-19)


### Bug Fixes

* add environment input for Gist URL construction in action.yaml ([9e7487f](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/9e7487ff7fa401a7ec5ee6dcc855d7681f52b50d))
* add environment variable logging for Gist fetching in action.yaml ([0da00bf](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/0da00bf9ddee95f6d0c679d6d2b79ab0d17b4198))
* add gist inputs and download step for Infracost configuration ([ea305a5](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/ea305a5ad0a4daba5b3aa7b9255fe0395edc8fb0))
* add Infracost setup step to action.yaml ([513ee53](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/513ee53758e1751c07ee8a8c1b70ab904f90ae2d))
* add shell and working directory for downloading Gist configuration in action.yaml ([f921812](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/f921812f603acc4d575b59dde648c46b5cd03d6d))
* add summary output for defined max cost in action.yaml ([940faed](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/940faedd576e0b5f4ef64585c3619b521b9156e9))
* correct syntax for accessing GitHub environment variable in action.yaml ([88c20ea](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/88c20ea4ef603e97a6cc010487035f72e6fe404e))
* correct syntax for repository name extraction in action.yaml ([f572f2f](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/f572f2ffc7987022c352dd5df5859490061fa3d3))
* correct syntax for repository name extraction in action.yaml ([ce55a03](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/ce55a032e594ffbc17e87446d007099bc64f905f))
* improve documentation and enhance max cost handling in action.yaml ([5ac49c6](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/5ac49c66ca463a47becd2bec409bcb4f8993d2f5))
* include environment in max cost summary output ([5e25498](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/5e254985bc531248b20eea2154fb56a9661012c3))
* reorganize inputs in action.yaml and update artifact handling ([7de47f0](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/7de47f0f0a883f510bb6e25d3af87ece2c5c3d21))
* update action.yaml inputs and remove unused parameters ([c97a140](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/c97a140b3bc3b9c06b8143178e58c91756317cdb))
* update environment input description and default value in action.yaml; enhance Gist fetching logic to include repository context ([941b131](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/941b13123e9b6d494fe680be03f34af8c1334aec))
* update max cost retrieval logic in action.yaml ([13c667b](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/13c667b41dd60b0b76d651c74f11c2b2d712b889))
* update max cost summary output to include environment variable ([99d57fb](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/99d57fb000f21b5a1f85223939544a3734cc7c6d))
* update max cost summary output to use input variable for environment ([51830b8](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/51830b8955387794e9fabcb1fbf15b97b4673f10))
* update README and action.yaml for improved clarity and input descriptions ([53ad4ee](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/53ad4ee07845e32709bcc14e81bd96d1cacb54fd))
* update repository name extraction logic in action.yaml ([5e771a3](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/5e771a363d618dda850884e4d9d784ccaba32db4))
* update syntax for repository name extraction in action.yaml ([ebda312](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/ebda31221af7040fd5b15ff00bfc6ec21553ba11))
* update tf-plan-name description for clarity and remove redundant lines ([1e3f71c](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/1e3f71ce5635d21b864277294209ac93dbce7c03))

# 1.0.0 (2025-05-25)


### Bug Fixes

* add CI pipeline input and update Infracost step to output monthly cost summary ([3f37ac2](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/3f37ac2472f573c487598d9e476deeb1bdb642cb))
* add required inputs for S3 bucket, region, and DynamoDB table in action.yaml ([3461565](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/34615657442c7c59de9c89e062255ff6f34faf22))
* add Terraform setup step before converting plan to JSON ([8203431](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/8203431c257bc94919d0d98c6163162301c7fe36))
* move Infracost API key to secrets and update JSON conversion output ([d08606f](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/d08606f37c44540b440124a015fa35f2dfe615f5))
* rename step to 'Run Infracost' and streamline API key export ([6a8a261](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/6a8a261fec7a25c36f54a8b32be86c10dc020eae))
* reorganize inputs in action.yaml and update Infracost API key handling ([6b3bf2b](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/6b3bf2ba6bd395cb292ec6d8b6a472e2ef8aa271))
* set default max-cost value and update Infracost summary output format ([f4c1f4c](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/f4c1f4cfe13e7c80c589f0ccb9c05f75ae264374))
* update links and names to reflect the infracost-action repository ([1da50f2](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/1da50f26be9062886863258fcaf296b94d58689a))
* update Terraform setup steps and add backend configuration ([525f57f](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/525f57f56523aac44375de553d051288df85f719))

## [1.1.2](https://github.com/subhamay-bhattacharyya-gha/infracost-action/compare/v1.1.1...v1.1.2) (2025-05-21)


### Bug Fixes

* update devcontainer configuration to include Node.js feature ([a6d9d47](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/a6d9d478096bf3f7a94f5fd44e26c3deb6e2611c))

## [1.1.1](https://github.com/subhamay-bhattacharyya-gha/infracost-action/compare/v1.1.0...v1.1.1) (2025-05-19)


### Bug Fixes

* add missing permissions for issue assignment workflow ([6c1c99c](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/6c1c99cb15f3df2cda6f7e8ea385447d43011bd7))

# [1.1.0](https://github.com/subhamay-bhattacharyya-gha/infracost-action/compare/v1.0.0...v1.1.0) (2025-05-19)


### Features

* add workflow to auto create branches on issue assignment ([c598e00](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/c598e002938006d48354017d1131d1f43e378393))

# 1.0.0 (2025-05-18)


### Bug Fixes

* update release configuration path in package.json ([d94b611](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/d94b61152ef216a98f5303e2ed2d78dbe309dd0e))


### Features

* add plugins for analyzing commits, generating release notes, preparing release, publishing, and verifying conditions ([60bfe70](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/60bfe70c3415559965a970971676f25a960d884f))
* add release configuration for semantic release ([bc81687](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/bc81687811d3ba20fb35a813afd29d222b37dbe0))
* initialize semantic release setup with custom plugins ([3a795e3](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/3a795e3f38397cceb825de4380c5d88907a3b744))
* migrate release configuration from release.config.js to .releaserc.json ([1351e55](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/1351e55fedf58fa9fb9bba217eecf1dba18c5a5c))
* reorder badges in README for better visibility ([f594ac6](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/f594ac67198dddcb460c3e8f14b06ecc05dc7c36))
* update actions/checkout and actions/setup-node to v4 ([ea8ec0d](https://github.com/subhamay-bhattacharyya-gha/infracost-action/commit/ea8ec0d94afac30900f7d7229330ad4e6cc00a3d))

# Changelog

All notable changes to this project will be documented in this file.
