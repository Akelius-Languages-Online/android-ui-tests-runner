# android-ui-tests-runner

Automates android UI tests

## How to prepare

## Step 1

Check out your project inside `./repo`

## Step 2
Usually every android project has:

- google-services.json
- gradle.properties
- local.properties

Please fill them in the file placeholders in the root of the project.
They will be copied on top of the project on every run.

## Step 3

`scheduler.devices` defines the devices you want to run test on. It can be empty.
`scheduler.tests` defines the tests that need to run. It can be specific test or a group of tests. It can be empty.
`scheduler.package` defines the base UI tests java package name.
`scheduler.enabled` enable / disable the scheduler on runtime

## How to use it

This repo offers (two) main ways to run tests:

- automated with scheduler
- manual

### Automated

You can configure the script to monitor specific branch of a repo.
In cases of a change it will run all specified tests on predefined devices.

Run `./scheduler`

## Manual

It's a shortcut to calling gradle

`/tools/run-ui-tests testingenvironment.onlinemode.anonymoususer.a0.chapter1.Quiz RF8M53G6FFE` will run `testingenvironment.onlinemode.anonymoususer.a0.chapter1.Quiz` on device `RF8M53G6FFE`

## Requirements

gradle
