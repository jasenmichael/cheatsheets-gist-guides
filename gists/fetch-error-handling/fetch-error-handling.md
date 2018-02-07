
### JavaScript fetch error handling

``` javascript
fetch("https://galvanize-leader-board.herokuapp.com/api/v1/leader-board/GBP")
    .then(function(response) {
        if (!response.ok) {
            throw Error(response.statusText);
        }
        return response;
    }).then(function(response) {
        console.log("ok");
    }).catch(function(error) {
        console.log(error);
    });
```
