# fis-postpackager-qunit

A test plugin for fis to test js file.

## usage

    $ npm install -g fis-postpackager-qunit
    $ vi path/to/project/fis-conf.js

```javascript
//file : path/to/project/fis-conf.js
fis.config.merge({
    modules : {
        postpackager : 'qunit'
    },
    settings : {
        postpackager : {
            qunit: {
                all : ['test/*.html']
            }
        }
    }
});
```

```javascript
//for fis3
fis.match('::packager', {
  postpackager: fis.plugin('qunit', {
    all: ['test/*.html']
  })
});
```


more [options](https://github.com/gruntjs/grunt-contrib-qunit)

