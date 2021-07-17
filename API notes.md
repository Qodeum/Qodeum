### APIs
#### Basics
- Applicaiton Programming Interface (all processing abstracted)
- Request/Response cycle
- GET, POST, PUT, DELETE and many more
- JSON Javascript Object Notation (curretly, most dominant data format): key value pairs
- If reponse sent a a string use JSON.parse(response) to represent as JSON
- Javascript "typeof" can be very helpful
- XMLHttpRequest: allows create an object with the ability to connect to a URL and retrieve data wihtout having to reload the page
- function()....is the callback
```javascript
  var request = new XMLHttpRequest();
  request.open('GET', 'https://hplussport.com/api/products');
  request.onload = function() {
    var response = request.response;
    var parsedData = JSON.parse(response);
    console.log(parsedData);
  }
  request,send();
```
- jQuery AJAX (Asynchronous Javascript and XML)
```javascript
  $.ajax({
    url: 'https://hplussport.com/api/products',
    success: function(response) {
      console.log(response)
    }
  })
```
- $.get(URL, success)
- Fetch (built on javascript promise)
```javascript
  fetch('https://hplussport.com/api/products')
  .then(
    function(response) {
      return response.json();
    }
  )
  .then(
    function(respData) {
      consoel.log(respData);
    }
  )
```
- 
#### Advanced
- REST
- CORS
- SOP
