
                                           ;''
                                         ''';:
                                        ''
                                       ''
       ,':      `',     ,'.      ,;`   ''   ;'''`      ;;.     ;;.              ,;  .;;     `;:       '
     `@@@@@, @@#@@@@  `@@@@@  @@@@@@+ ;',   ''''';   +@@@@@  '@@@@@  @@   @@ @@@@@ @@@@@'  @@@@@` @@'@@ @@   @@
     @@: `@@ @@@  @@# @@` '@@ @@' '@@ '''    ''''',  @@  ;@# @@  +@@ @@   @@ @@@;;@@#  @@ @@' `@@ @@@+; @@, ,@@
    `@@   @@:@@,   @@.@@...@@ @@   @@ '''      ''''  @@@'   +@#   @@ @@   @@ @@   @@   .. @@...@@ @@'   ,@@ @@`
    ,@@   +@+@@    @@;@@@@@@@ @@   @@ .''':     `''`  @@@@@.@@;   @@ @@   @@ @@   @@      @@@@@@@.@@     @@ @@
    `@@   @@,@@,   @@.@@      @@   @@  ''''':    `',     #@@'@#   @@ @@   @@ @@   @@   @@ @@      @@     @@;@+
     @@' ,@@ @@@  @@# @@. :@@ @@   @@  ,''''''    ', @@  .@@ @@` #@@ @@' @@@ @@   @@# .@@ @@+ `@@ @@      @@@
      @@@@@. @@+@@@@  `@@@@@  @@   @@   ;'''''    '` '@@@@@` ,@@@@@  #@@@@@@ @@    @@@@@.  @@@@@. @@      @@@
        .`   @@. .`     `.                ''''    '    ..      ..      .             ..      ..           @@,
             @@.                                 ';                                                     @@@@
             @@.                                ''                                                      @@@`
                                           :'''';

# Alphecca

## Sass framework/library for OpenSourcery's theme system

### Description

For use in any Drupal project, Alphecca provides default styling as well as grid setup for Singularity. At this time during development, Alphecca is just a library. It may eventually become available as a Bower package or Compass extension.

Alphecca makes extensive use of ZURB Foundation 5.

### Requirements

1. [Sass](http://github.com/Snugug/training-glossary/wiki/Sass#head)
2. [Compass](http://github.com/Snugug/training-glossary/wiki/Compass#head)
3. [Breakpoint](http://github.com/team-sass/breakpoint) - Media Query Handling
4. [Singularity](http://github.com/Team-Sass/Singularity) - Fluid grid framework
5. [Toolkit](http://github.com/Team-Sass/toolkit) - Modern Web Development tools

### Directions

1. To use this library you need a makefile directive to put the library in a place where it can be compiled with the theme Sass. Something like this:

```bash
; Alphecca Sass Framework
libraries[alphecca][download][type] = "git"
libraries[alphecca][download][branch] = "master"
libraries[alphecca][download][url] = "https://github.com/opensourcery/alphecca.git"
libraries[alphecca][destination] = "themes/custom/MY_THEME_NAME/vendor"
libraries[alphecca][download][directory_name] = "alphecca"
```

2. Then in your base/global/root SASS file, just import:

```sass
@import '../vendor/alphecca/sass/styleguide';
```

3. This import should be one of the first so overrides are sane.

### Resources

* [Scalable and Modular Architecture for CSS](http://smacss.com)
* [ZURB Foundation](http://foundation.zurb.com)
* [Drush make](http://drush.ws/docs/make.txt)

### Licenses

* [IcoMoon Icons](http://icomoon.io/) are used in Alphecca under the [GPL license](http://www.gnu.org/licenses/gpl.html).
* [ZURB Foundation](http://foundation.zurb.com) components are used in Alphecca under the [MIT license](http://www.opensource.org/licenses/mit-license.php).
