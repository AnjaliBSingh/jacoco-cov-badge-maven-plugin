# Jacoco Coverage Badge Maven Plugin

![build](https://travis-ci.org/HandOfGod94/jacoco-badge-maven-plugin.svg?branch=master)

> WIP

Jacoco is code coverage utility which generates nice report for
Java Based projects and is generally integrated as maven build plugin.

`Badges` are like the one you are seeing above, which represents `build` status.
There are several online utilities like `coveralls`, `shields.io` etc. which
provides badges as a service.

## Why?

None of the utilities mentioned above solves the problem of generating local
badges esp. for `Java` projects. There were few attempts in the past but they
were not satisfactory.

## What it does?

It's a `maven` plugin, which if included as part of build then will generate
an `svg`,`png` or `jpg` coverage badges based on user configuration.

It reads the coverage report generated by `jacoco` and generates a local badge,
which can then be included in any `.md` files.

> It is highly inspired from `gh-badges` which `shields.io` also uses for
> generating badges.

## Build Steps:
```shell
# To build jar file for plugin
mvn clean package

# To install it in local repo
mvn clean install
```

## Usage:
```console
foo@bar:~$ mvn org.gahan:jacoco-badge-maven-plugin:1.0-SNAPSHOT:badge
```

Currently, it requires fully qualified name for executing a goal, once
it's published to maven repository, it will change.

More documentation and features coming soon...
