# JavaScript Snowball Stemmers [![Build Status](https://travis-ci.org/mazko/jssnowball.svg?branch=master)](https://travis-ci.org/mazko/jssnowball)

Port from [Snowball](http://snowball.tartarus.org/) Stemmers. [Online](http://mazko.github.io/jssnowball/)

[snowball.es6](js_snowball/lib/snowball.es6) | [snowball.babel.js](js_snowball/lib/snowball.babel.js)

### ESJava (ES6) fun

- Run [bootstrap](snowball_cache/configure) script to download and regenerate last original Java Snowball stemmers

- Use your favorite IDE to remove unused code in *.java sources like ```copy_from```, ```hashCode``` e.t.c. Here is Eclipse EE Mars.1 Release (4.5.1) example:

*source -> cleanup*

![cleanup-profile](js_snowball/screenshots/cleanup-profile.png)

- ESJava has some restrictions like reflection e.t.c. You have to refactor manually such *.java sources too :(

- Merge all *java in to one single snowball.bundle.java: ```make bundle```

- Manually edit js-specific fragments: ```awk /:es6:/,/:end:/ js_snowball/lib/snowball.bundle.java```

- Enjoy ```make esjava``` !
