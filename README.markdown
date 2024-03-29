# ProjectTemplate [![Travis-CI build status](https://api.travis-ci.com/KentonWhite/ProjectTemplate.png?branch=master)](https://app.travis-ci.com/github/KentonWhite/ProjectTemplate)

The ProjectTemplate package lets you automatically build a directory for a new R project with a standardized subdirectory structure. Using this structure, ProjectTemplate automates data and package loading. The hope is that standardized data loading, automatic importing of best practice packages, integrated unit testing and useful nudges towards keeping a cleanly organized codebase will improve the quality of R coding.

The inspiration comes from the `rails` command from Ruby on Rails, which initializes a new Rails project with the proper skeletal structure automatically. Also, ProjectTemplate follows Rails's approach of preferring convention over configuration: the automatic data and library loading as well as the automatic testing work easily because assumptions are made about the directory structure and naming conventions used in your code. You can customize your codebase however you'd like, but you will have to edit the ProjectTemplate loading functions to use your conventions instead of the defaults.

## Installing
ProjectTemplate is now available on CRAN and can be installed using a simple call to `install.packages()`:

    install.packages('ProjectTemplate')

If you would like access to changes to this package that are not available in the version currently on CRAN, please install this package directly from Github,

	library('devtools')
	install_github('KentonWhite/ProjectTemplate')

For most users, running the bleeding edge version of this package is probably a mistake.

## Example Code
To create a project called `my-project`, open R and type:

    library('ProjectTemplate')
    create.project('my-project')
    setwd('my-project')
    load.project()

## Finding Out More
* Website: Visit the [ProjectTemplate website](http://projecttemplate.net) for more details.
