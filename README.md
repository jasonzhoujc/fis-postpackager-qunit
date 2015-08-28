# reasy-postpackager-qunit

A test plugin for reasy to test js file.

## usage

    $ npm install -g reasy-postpackager-qunit
    $ vi path/to/project/fis-conf.js


```javascript
//for fis3
fis.match('::packager', {
  postpackager: fis.plugin('qunit', {
    all: ['test/*.html']
  })
});
```

more [options](https://github.com/gruntjs/grunt-contrib-qunit)

