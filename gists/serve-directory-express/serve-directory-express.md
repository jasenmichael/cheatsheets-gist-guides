#### Server a directory with express

###### An simple way to host the client in a separate directory using node express


```javascript
var path = require('path')

var express = require('express')

var app = express()

app.use(express.static(path.join(__dirname, '../client')))
```
