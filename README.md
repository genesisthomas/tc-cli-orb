TestCraft cli Orb [![CircleCI Build Status](https://circleci.com/gh/genesisthomas/tc-cli-orb/tree/master.svg?style=shield "CircleCI Build Status")](https://app.circleci.com/pipelines/github/test-craft/tc-cli-orb) [![CircleCI Orb Version](https://img.shields.io/badge/endpoint.svg?url=https://badges.circleci.io/orb/circleci/gradle)](https://circleci.com/orbs/registry/orb/testcraft/testcraft) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/CircleCI-Public/gradle-orb/master/LICENSE) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)
==============================

### What is TestCraft cli Orb?
  This orb is a cli tool that enables you to execute TestCraft test automation scenarios and view their results through CircleCI’s CI/CD platform.
  

### Sample Config
An example config running TestCraft automation scenarios for multiple browsers in parallel with Maven

```yaml
version: 2.1
orbs:
  testcraft: testcraft/testcraft@2.4.7
jobs:
  run:
    docker: 
      - image: 'cimg/base:stable'
      - image: 'circleci/node:13.0.1'
workflows:
  browser_tests:
    jobs:
     ...
          
```

