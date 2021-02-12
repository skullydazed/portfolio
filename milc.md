---
layout: page
title: MILC
---

[MILC](https://milc.clueboard.co/) is a framework for writing CLI tools. It makes writing good CLI's easy.

## Why Did You Write Your Own Framework?

In a world where [Click](https://click.palletsprojects.com/) exists why did I write my own? Because Click is focused on services while MILC is focused on end users. You can write good tools for end users with Click but it's extra work. MILC makes writing good tools the easy thing to do, and in some cases the only thing.

## How Does MILC Make The Right Thing The Easy Thing?

MILC strikes a balance between flexibility for the programmer and good user interaction. All MILC scripts have flexible and configurable log output, the ability to turn colors on and off, and configuration file support. The programmer doesn't have to write any extra code to provide those features to the user.

MILC is opinionated. For example, it thinks you should use Python's built-in logging facility and does not provide the ability to use anything else. Another example is that command line arguments are automatically mapped to configuration file values so that users can always override a config file at runtime.

When the needs of the Programmer and the needs of End User come into conflict MILC tends to value the End User more.
