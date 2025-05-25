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
