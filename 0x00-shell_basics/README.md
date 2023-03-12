#!/bin/bash specifies program to execute the script is bash
ls -1a | sed -E 's|^(.*)/$|\1/|' | LC_COLLATE=C sort -d | awk '{printf "%s,", $0} END {print ""}'
