rest-proxy
==========

Simple PHP Rest-proxy, supports GET, POST, PUT and DELETE

Example Requests:

POST
```

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
```
$.get( "index.php?url=https://www.facebook.com", function( data ) {
  console.log(data);
});
```

PUT
```
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
```
$.ajax({
    url: 'index.php?url=http://www.manutd.com/players/10',
    type: 'DELETE',
    success: function(data) {
        console.log(data);
    }
});
```