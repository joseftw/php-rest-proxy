rest-proxy
==========

Simple PHP Rest-proxy, supports GET, POST, PUT and DELETE

Example Requests:

POST
```
var player = {};
player.Name = 'Zlatan Ibrahimovic';

$.ajax({
   url: 'index.php?url=http://www.arsenal.com/addPlayer/',
   type: 'POST',
   data: { data: JSON.stringify(player) },
   success: function(data) {
     console.log(data);
   }
});
```

GET
```
$.get( "index.php?url=http://www.arsenal.com", function( data ) {
  console.log(data);
});
```

PUT
```
var player = {};
player.Goals = 10000;

$.ajax({
   url: 'index.php?url=http://www.arsenal.com/players/10',
   type: 'PUT',
   data: JSON.stringify(player),
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