# Overview

sparkcli (say 'sparkly' :) is a command line interface to Cisco Spark.

# Usage

Download [here](https://bintray.com/tdeckers/sparkcli/sparkcli#files)

For help:

    sparkcli -h

Examples

    # List rooms
    sparkcli room list
    
    # Send message to a room
    sparkcli message create <roomid> <msg>

# Development

Build and deploy using goxc: [See here.](https://github.com/laher/goxc/blob/master/README.md)

## Install go from source

    git clone https://go.googlesource.com/go
    git branch go1.5
    cd src
    ./all.bash 
    go get golang.org/x/tools/cmd/...

## Install goxc

    go install github.com/laher/goxc

## Run goxc

Inside the project directory, run:

    goxc

## bintray uploads

Add API key to .goxc.local.json

    goxc bintray
