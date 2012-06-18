# couchr

AMD-compatible, uses jQuery.ajax to make the XHR requests but with better CouchDB
error reporting and a simpler API.

**702 bytes** (packed and gzipped)


### Example

```javascript
require(['couchr'], function (couchr) {
    couchr.get('/dbname/docid', function (err, doc) {
        ...
    });
});
```

### Methods

    couchr.get(url, [params], callback)
    couchr.post(url, [data], callback)
    couchr.head(url, callback)
    couchr.put(url, [data], callback)
    couchr.delete(url, [data], callback)

    couchr.ajax(options, callback) - Works like the jQuery.ajax function
    but with the callback using couchr error handling.
