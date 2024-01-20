# Monorepo Template

This project is designed a scaffold for handling projects that have to coordinate multiple apps and packages. This is built based on a couple of projects that have required this structure, and will be used in all future projects that require something similar.

## How to Use

1. Clone this project locally.
2. Rename any instances of `monorepo` to the actual name of your project (`@monorepo` should become `@new-name`).
3. If you need any packages, duplicate `package` and rename the folder, package.json and and update any references to the package in any apps.
2. If you need any apps, duplicate `app` and rename the folder, package.json and update any references to the commands in the root package.json.

## Project Structure

This project is broken up into two main directories:

* `/apps/`, which contains all discrete and deployable parts of the project
* `/packages/`, which contains any compilable and shareable code

In each, there is a singular (`app` and `package`) scaffold to help smooth out any bugs.

In `app`, we use:

* `eslint`
* `typescript`

In `package`, we use:

* `eslint`
* `typescript`
* `tsup`