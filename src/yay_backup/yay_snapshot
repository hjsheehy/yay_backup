#!/bin/bash

DIR=~/.config/yay
FILE=$DIR/pkgs
mkdir -p $DIR
yay -Qet | awk '{print $1}' | tr '\n' ' ' > $FILE
