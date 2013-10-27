MimeMagic is a library to detect the mime type of a file by extension or by content. It uses the mime database
provided by freedesktop.org (see http://freedesktop.org/wiki/Software/shared-mime-info/).

[![Build Status](https://secure.travis-ci.org/minad/mimemagic.png?branch=master)](http://travis-ci.org/minad/mimemagic) [![Code Climate](https://codeclimate.com/github/minad/mimemagic.png)](https://codeclimate.com/github/minad/mimemagic)
[![Gittip donate button](http://img.shields.io/gittip/bevry.png)](https://www.gittip.com/min4d/ "Donate weekly to this project using Gittip")
[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=min4d&url=https://github.com/minad/mimemagic&title=MimeMagic&language=&tags=github&category=software)

Usage
=====

    require 'mimemagic'
    MimeMagic.by_extension('html').text?
    MimeMagic.by_extension('.html').child_of? 'text/plain'
    MimeMagic.by_path('filename.txt')
    MimeMagic.by_magic(File.open('test.html'))
    # etc...

API
===

http://rdoc.info/github/minad/mimemagic/frames/file/README.md

Tests
=====

```
bundle install

rake test
```

Authors
=======

Daniel Mendler
