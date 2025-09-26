# Meltdown repository specification

## Repository naming

The repository may be named with either a proper name(e.g., `neon` or `libhallucinate`), a descriptive name(e.g., `md-repo-spec` or `md-toolchain`), or a meltdownified name of a taken project(e.g., `md-git`)

All names are in **kebab-case**

### Proper names

Proper names shall be given to a project if anyone comes up with one that is:
1. not already in use by any notable project
1. does not contain any controversial words(e.g. `raper`, etc.)
1. does not mislead users on what the project does(e.g. `*cc` for something that isnt a C compiler)

### Descriptive names

Descriptive names always start with `md-` and then a proper description of what the project is/does.

### Meltdownified names

This naming scheme is **strictly for reimplementations** and involves putting `md-` before the name of the original.

### Long names

The readme and other `.md` files must contain a long name that is just a description of what the project does alongside the name(if it isn't already a descriptive name).

These long names are in **Title Case**.

## Versioning

While the exact versioning scheme to use depends on what the project is, we recommend a Major-Minor-Patch system with or without codenames.

A custom versioning scheme may be defined under the `Versioning` heading of `README.md`

## Repository branches

### The development branch

The `dev` branch is for development. Developers can push to this branch, and this branch contains configurations for code editors and tools like `clang-format`

### The version branches

Each version can have a version branch for each version that must start with `ver/` and then the formatted version number.

### The feature branches

If the `dev` branch is not enough, you may add `feat/` branches for extra work; they are just copies of the `dev` branch.

## DEPS.md

This file is a simple list of the project's dependencies:
* **bold** dependencies are outside dependencies
* *italic* dependencies are optional dependencies

## LICENSE

The license of all repositories must be `0BSD` attributed to `The Meltdown project`.

## PURPOSE.md

This file is for specifying the purpose and scope of the project. Its purpose is to specify what features are in scope for the project.

### Purpose

The `Purpose` header must clearly define the purpose of the project.

### Scope

The `Scope` header must clearly define what each component(if separated) in the project is meant to do.

## README.md

The first heading of the README must be the project name, with the project description and badges below it.

### Building(optional)

This section may include building instructions or just a link to `BUILDING.md` if it's too long.

### Versioning(optional)

This section may describe an alternate versioning scheme for the project.

### Licensing

This section must say that `This project is licensed under the BSD Zero Clause License.`.

## SPEC.md

This file has to specify the intended behaviour of the project. Its format is left up to the project.