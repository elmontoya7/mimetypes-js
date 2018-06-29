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

var file_mime_type = mime.getMime('my_file.gz');
//file_mime_type == 'application/x-gzip'

var file_name = mime.removeExt('my_movie_file.mov');
//file_name == 'my_movie_file'

var file_name = mime.addExt('my_memories', 'video/quicktime');
//file_name == 'my_memories.mov'

var file = { name: 'file_uploaded_from_device',
  data: <Buffer>,
  encoding: '7bit',
  mimetype: 'application/pdf',
  mv: [Function: mv] };
var file_name = mime.addExt(file);
//file_name == 'file_uploaded_from_device.pdf'

var has = mime.hasExt('file_uploaded.3gp')
//has == true
```
