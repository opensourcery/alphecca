Alphecca
========

Sass framework/library for use in any project. This is not a compass extension,
rather it's just a library (for now, during develoment).

# Usage

To use this library you need a makefile directive to put the library in a place where it can be compiled with the theme SASS. Something like this:


```bash
; Alphecca Sass Framework
libraries[alphecca][download][type] = "git"
libraries[alphecca][download][branch] = "master"
libraries[alphecca][download][url] = "https://github.com/opensourcery/alphecca.git"
libraries[alphecca][destination] = "themes/custom/MY_THEME_NAME/vendor"
libraries[alphecca][download][directory_name] = "alphecca"
```

Then in your base/global/root SASS file, just import:

```sass
@import '../vendor/alphecca/sass/styleguide';
```

This import should be first so overrides are sane.
