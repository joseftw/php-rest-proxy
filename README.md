PHP REST-Proxy
==========

Simple PHP REST-proxy, supports GET, POST, PUT and DELETE

Example Requests:

POST
```javascript

$.ajax({
   url: 'index.php?url=http://www.arsenal.com/addPlayer/',
   type: 'POST',
   data: { name: 'Zlatan Ibrahimovic' },
   success: function(data) {
     console.log(data);
   }
});
```

GET
```javascript
$.get( "index.php?url=https://www.facebook.com", function( data ) {
  console.log(data);
});
```

PUT
```javascript
$.ajax({
   url: 'index.php?url=http://www.arsenal.com/players/10',
   type: 'PUT',
   data: { goals: 10000},
   success: function(data) {
     console.log(data);
   }
});
```

DELETE
```javascript
$.ajax({
    url: 'index.php?url=http://www.manutd.com/players/10',
    type: 'DELETE',
    success: function(data) {
        console.log(data);
    }
});
```