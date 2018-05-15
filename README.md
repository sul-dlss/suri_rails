[![Build Status](https://travis-ci.org/sul-dlss/suri_rails.svg?branch=master)](https://travis-ci.org/sul-dlss/suri_rails)
[![Coverage Status](https://coveralls.io/repos/sul-dlss/suri_rails/badge.svg)](https://coveralls.io/r/sul-dlss/suri_rails)

# SURI

SURI is the Stanford Libraries' unique identifier minting system. It mints unique DRUIDs.

## Requirements

1. Ruby (2.4.1 or greater)

## Installation

Clone the repository

    $ git clone git@github.com:sul-dlss/suri_rails.git

Change directories into the app and install dependencies

    $ bundle install

Start the development server

    $ rails s

## Testing

The test suite (with RuboCop style enforcement) will be run with the default rake task (also run on travis)

    $ rake

The specs can be run without RuboCop enforcement

    $ rake spec

The RuboCop style enforcement can be run without running the tests

    $ rake rubocop

## Building for Docker

```
docker build -t suldlss/suri-rails:latest
```

Then run as:
```
docker run -d -p 127.0.0.1:3002:3000 suldlss/suri-rails:latest
```
