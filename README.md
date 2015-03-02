# Simple Sufia App For Hacking

See also: [Sufia](https://github.com/projecthydra/sufia) source.

To replicate the base of this project, follow the
[basic application](https://github.com/projecthydra/sufia#creating-an-application)
instructions, except using relative path instead of a version
number for the Sufia dependency.

## Get Sufia source

Get Sufia source and dependencies

    git clone git@github.com:projecthydra/sufia.git
    cd sufia
    bundle install

## Set up new test app

    cd ..
    rails new sufiatest
    cd sufiatest

## Add Sufia dependency as source, not a published version

    gem 'sufia', path: '../sufia'

## Finish setup

Just follow the rest of the recommended Sufia setup, including running the
generators, migrations, and Jetty/Redis startup. Once everything is running,
you can modify most of the relevant code in Sufia and the application without
restarting any of the pieces.

