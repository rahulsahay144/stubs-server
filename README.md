# Stubs Server

This module is for creating and mocking API responses via json and stubs.

## Steps 

1. Install stubs-server using `npm insall --save stubs-router`.
2. Create an index.js file 

```
//'use strict';

var express = require('express');
var path = require('path');
var app = express();

var stubsUi = require('stubs-server')(app);

app.listen(9001, function() {
    console.log('server started on 9001');
});

//module.exports = app;
``` 

3. Run the server using `node index.js`
4. Open the webpage `http://localhost:9001`
5. Create new stubs by clicking 'Create New Stub'.
6. Type the 'api name'(e.g "test") and enter valid json and Click 'Add API'.
7. Search for API, edit and save.
8. Test your mock api by going to browser "http://localhost:9001/test".

![stubs-server](https://cloud.githubusercontent.com/assets/4962816/21962452/93464bac-db4c-11e6-82a9-65a73c9f9ce8.PNG)
