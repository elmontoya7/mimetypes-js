# mimetypes-js
Convertion tool from mime type to extension and extensions to mime type.

# install
```javascript
npm install mimetypes-js --save
```

# usage
```javascript
var mime = require('mimetypes-js');

var file_extension = mime.getExt('video/quicktime');
//file_extension == 'mov'

var file_mime_type = mime.getMime('pdf');
//file_mime_type == 'application/pdf'
```
