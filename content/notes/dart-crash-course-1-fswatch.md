+++
title="Vandad's Crash Course: 1. Use fswatch to run dart code after every file change"
date = 2024-01-15T01:15:00Z
+++

# Vandad’s Dart Crash Course: 1. Use fswatch to run dart code after every file change

I haven’t tried `fswatch` yet, but from what I understand, the tool will monitor for file change and it can then be set to run a command in response to the change. In the course, `fswatch` will rerun the `dart` command for the changed dart file (which I assume happens after every changed save). Use the following to run the `dart` command after every change within a directory: `fswatch bin/ | xargs -n1 -I{} sh -c 'clear;dart {}’`.

Source: [https://www.youtube.com/watch?v=uZELNjhtoPk&list=PL6yRaaP0WPkVLSOchfoIA0ZXySz4eSYV2&index=3](Dart Crash Course: Dart’s Variable and Data Types)
