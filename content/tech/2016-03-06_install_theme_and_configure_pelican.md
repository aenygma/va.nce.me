Title: Installing a pelican theme and configuring pelican
Modified: 2016-06-06 15:45
Tags: python, pelican, publishing, git
Summary: Installing a Pelican theme and setting up pelican to use the theme for [va.nce.me](http://va.nce.me/)

## Theme

The base theme I have chosen as the basis for my site is [Pure Pelican Theme](http://purepelican.com/).  It is possible that I may want or need to modify the core theme styles and templates, so I am going to [fork it on Github](https://github.com/vanceb/pure-single), then clone that repository to be used locally.  I am going to install the theme as a submodule of the [va.nce.me website](https://github.com/vanceb/va.nce.me)

``` shell
git clone git@github.com:vanceb/va.nce.me
cd va.nce.me
mkdir themes
git submodule add git@github.com:vanceb/pure-single themes/pure-single
```

## Configuring Pelican and the themes

The Pelican config file `pelicanconf.py` allows you to configure pelican for your site including [basics](http://docs.getpelican.com/en/3.6.3/settings.html) that the core Pelican uses as well as some variables that the theme can use.  You can check out my [`pelicanconf.py`](https://github.com/vanceb/va.nce.me/blob/master/pelicanconf.py) file in github.
