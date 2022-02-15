# Dronecan V1 website

[![Discussions](https://dronecan.org/discord)](https://dronecan.org/discord)


This repository contains sources of the DronCAN V1 website available at <https://dronecan.github.io>.

How to configure Jekyll with Github Pages: <https://help.github.com/articles/using-jekyll-with-pages>.

## Dependencies

### [Ruby](https://www.ruby-lang.org/en/)

Install Ruby 2.x. If necessary, activate it using [RVM](https://rvm.io/).

### [Bundler](http://bundler.io/)

Follow the instructions on the [repository page](https://github.com/bundler/bundler) to install Bundler.

### [Jekyll](http://jekyllrb.com/)

Enter your local clone derictory (make sure you have Gemfile there). Execute from the terminal: `bundle install`.

## Running the website locally

1. Enter your local clone derictory (where the Gemfile is located).
Make sure that all git submodules are initialized by running `git submodule update --init --recursive`.
2. Execute from the terminal `bundle exec jekyll serve` and wait until the page is generated.
3. Open your internet browser and navigate to <http://localhost:4000> to see your local website.

## Troubleshooting

In case you have an error like `in 'autodetect': Could not find a JavaScript runtime.`
while running `bundle exec jekyll serve`, add the following lines to the `Gemfile` in the parent folder:

```
gem 'execjs'
gem 'therubyracer'
```

Then open the terminal and run `bundle update && bundle install`.

## History

Much of the content of this website is based upon original work by
Pavel Kirienko and the UAVCAN Development Team. For contributors
please see https://github.com/UAVCAN/uavcan.github.io

The content is licensed under the Creative Commons Attribution License
4.0. See https://creativecommons.org/licenses/by/4.0/ for details.
