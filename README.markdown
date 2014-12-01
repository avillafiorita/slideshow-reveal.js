# Reveal.js - Slide Show

## What it is

A template which outputs reveal.js presentations using slideshow.


## What's Slide Show (S9)?

A Ruby gem that lets you create slide shows and author slides in plain text
using a wiki-style markup language that's easy-to-write and easy-to-read.
More [Slide Show (S9) Project Site](http://slideshow-s9.github.io).


## What's Reveal.js

Reveal.js is a HTML presentation framework created by [Hakim El Hattab](http://hakim.se/).  It is available at [Reveal.js on Github](https://github.com/hakimel/reveal.js)


## Installation

Clone this repository using `git` and save it in S9's templates directory:

    $ cd ~/.slideshow/templates
    $ git clone https://github.com/avillafiorita/slideshow-reveal.js.git

**Important!**  Reveal.js - Slide Show (this template) keeps [Reveal.js](https://github.com/hakimel/reveal.js) source files as a [git submodule](http://git-scm.com/book/en/v2/Git-Tools-Submodules). So you need to fetch it, otherwise you will get an error when building the presentation.

    $ cd ~/.slideshow/templates/slideshow-reveal.js
    $ git submodule init && git submodule update

To check if the new template got installed, use the `list` command:

    $ slideshow list

Listing something like:

    Installed templates include:
      reveal (~/.slideshow/templates/slideshow-reveal.js/reveal.txt)

Now you're ready to use it using the `-t/--template` switch. Example:

    $ slideshow build doc/s9-reveal.textile -t reveal --h2



## Troubleshooting

If you get an error like the following when building the presentation:

> *** error: No such file or directory @ rb_file_s_stat - /$HOME/.slideshow/templates/slideshow-reveal.js/reveal.js/Gruntfile.js

Then you probably forgot to fetch the reveal.js library. Run the following to fetch it and fix the problem.

    $ cd ~/.slideshow/templates/slideshow-reveal.js
    $ git submodule init && git submodule update


## Documentation

Have a look at:

    doc/s9-reveal.textile

which describes some of the features made available by S9 and Reveal.js.
