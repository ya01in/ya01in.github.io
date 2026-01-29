---
layout: post
title: "Adding dark theme to default jekyll theme for github page"
---

## Problem

minima of the default jekyll theme is the best for just recording, but as a programmer, no interface is perfect without dark mode.

## Cause

the github-pages support on its component are rarely updated, as the time of this record, the support on minima is still `2.5.1`, and the latest minima on github is 3.0

## Solution

with a bit of researching, with a little tweak in config can force the jekyll to use the latest minima by pulling from its github repository.

1. change theme setting in _config.yml

    ```yaml
    theme: minima  # remove
    remote_theme: jekyll/minima # add
    ```

2. Execute `bundle install && bundle update` in cmd to install your build and update.
3. Execute `bundle exec jekyll serve` to see the changes.

## Reference

1. [stack overflow: Does minima dark skin work on github pages?](https://stackoverflow.com/questions/68518590/does-minima-dark-skin-work-on-github-pages)
