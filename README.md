# mimext
Convertion tool from mime type to extension and extensions to mime type.

# install
```javascript
npm install mimext --save
```

# usage
```javascript
var mimext = require('mimext');

var file_extension = mimext.getExt('video/quicktime');
//file_extension == 'mov'

var file_mime_type = mimext.getMime('pdf');
//file_mime_type == 'application/pdf'
```
