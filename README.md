# img_checker

[![Build Status](https://travis-ci.org/Abhi2424shek/img_checker.svg)](https://travis-ci.org/Abhi2424shek/img_checker)
[![Gem Version](https://badge.fury.io/rb/img_checker.svg)](https://badge.fury.io/rb/img_checker)
[![Github All Releases](https://img.shields.io/github/downloads/abishekvashok/img_checker/total.svg)]()


Simple Linter to verify image sizes.

### How to use it?
Require the gem to be there:
`require img_checker`
or place it on your Gemfile
`gem 'img_checker'`

Then just put an img_config.yml at the root of the project.

### Format of the img_config.yml file
The img_config.yml file is used to hold the directories to scan for images
and also to hold the maximum size (width and height) an image can hold in a directory

This is the basic structure for a img_config entries:
```
- directory: <directory_path>
   width: <Max width for the images in the above directory>
   height: <Max height for the images in the above directory>
```

[Example](https://github.com/Abhi2424shek/img_checker/blob/master/test/img_config.yml)

**Note**: The image sizes must be specified in pixels although the units shouldn't be specified.

If you only want to scan specific files then change `./foo/*.*` to `./foo/*.extension` or
`./foo/imagename.extension`, to scan sub directories as well `./fool/**/*.*`.

## Branching policy
_development branch_: All development goes into this branch, if you want to make a PR, you should make it to this branch.
_master branch_: The master branch contqins stable releases and is a protected branch when there is a release we update the code from development to this branch and it isnfrom this branch that a release is made.

## Maintainers and contact information
- Abishek V Ashok (abhi2424shekvashok@gmail.com)
- Ankit R Gadiya
