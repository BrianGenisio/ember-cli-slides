##  Lets add delete

### Hook the template
```html
<button {{action "remove"}} class="btn btn-xs btn-default">X</button>
```

### Create the index controller
```javascript
ember generate controller beer/index
```

### Add the controller action
```javascript
actions: {
  remove: function(beer) {
    beer.destroyRecord();
  }
}
```
