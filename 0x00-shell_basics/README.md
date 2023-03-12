#!/bin/bash specifies program to execute the script is bash
rsync -avu --exclude='*' --include='*.html' ./ ../ coppies all html files from current workiing directory to parent directory
