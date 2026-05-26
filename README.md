# devops-capstone-project

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python 3.9](https://img.shields.io/badge/Python-3.9-green.svg)](https://shields.io/)

This repository contains the starter code for the project in 
**IBM-CD0285EN-SkillsNetwork DevOps Capstone Project** which is part of the 
**IBM DevOps and Software Engineering Professional Certificate**

## Usage

You should use this template to start your DevOps Capstone project. 
It contains all of the code that you will need to get started.

## Development Environment

These labs are designed to be executed in the IBM Developer Skills Network 
Cloud IDE with OpenShift.

Once you are in the lab environment, initialize it with:

```bash
source bin/setup.sh
```

## Useful commands

### Activate the Python 3.9 virtual environment

```bash
source ~/venv/bin/activate
```

### Installing Python dependencies

```bash
make install
```

### Starting the Postgres Docker container

```bash
make db
```

## Project layout

```text
├── service         <- microservice package
│   ├── common/     <- common log and error handlers
│   ├── config.py   <- Flask configuration object
│   ├── models.py   <- code for the persistent model
│   └── routes.py   <- code for the REST API routes
├── setup.cfg       <- tools setup config
└── tests                       <- folder for all of the tests
    ├── factories.py            <- test factories
    ├── test_cli_commands.py    <- CLI tests
    ├── test_models.py          <- model unit tests
    └── test_routes.py          <- route unit tests
```

## Data Model

| Name | Type | Optional |
|------|------|----------|
| id | Integer | False |
| name | String(64) | False |
| email | String(64) | False |
| address | String(256) | False |
| phone_number | String(32) | True |
| date_joined | Date | False |

## Your Task

Complete this microservice by implementing REST APIs for READ, UPDATE, 
DELETE, and LIST while maintaining 95% code coverage.

## Author

John Rofrano, Senior Technical Staff Member, DevOps Champion, 
@ IBM Research, and Instructor @ Coursera

## License

Licensed under the Apache License. See LICENSE
