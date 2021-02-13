---
layout: page
title: MILC
---

[MILC](https://milc.clueboard.co/) is a framework for writing CLI tools. It makes writing good CLI's easy.

## Why Did You Write Your Own CLI Framework?

Before building the [QMK CLI](qmk_cli.md) I surveyed the available CLI frameworks and found them lacking. It seemed that there were two basic paths for building a CLI- integrate python modules like argparse, configparser, and logging myself or use a framework like Click.

In a world where [Click](https://click.palletsprojects.com/) exists why did I write my own? Because Click's focus is on daemons, not CLI's. You can write good CLI's with Click but it's extra work. I wanted to make writing good CLI's the easy thing to do.

The decision to make my own was cemented after I built two QMK CLI prototypes- one using Click and the other using argparse, configparser, and logger. I realized that my second prototype was basically my own CLI framework, and after a couple hours work the first version of MILC was released.

## How Does MILC Make The Right Thing The Easy Thing?

MILC strikes a balance between flexibility for the programmer and good user interaction. All MILC scripts have flexible and configurable log output, the ability to turn colors on and off, and configuration file support. The programmer doesn't have to write any extra code to provide those features to the user.

MILC is opinionated. For example, it thinks you should use Python's built-in logging facility and does not provide the ability to use anything else. Another example is that command line arguments are automatically mapped to configuration file values so that users can always override a config file at runtime.

When the needs of the Programmer and the needs of End User come into conflict MILC tends to value the End User more.

## Why Should Developers Use MILC?

It gives you a lot of features that aid development right out of the box:

* Automatic `-v` support so you can add `cli.log.debug()` messages and turn them on/off
* Automatic log file support
* Thread safety
* Fun Emoji's

## What is the biggest deficiency in MILC right now?

Insufficient testing. Right now the unit testing is non-existant while the integration testing is reasonable but not complete. I wish I could dedicate 40 hours to writing comprehensive unit tests.
