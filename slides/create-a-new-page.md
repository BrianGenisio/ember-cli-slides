##  Create a 'new' page

```javascript
ember generate route beer/new
```

### Generate a temporary model
```javascript
model: function() {
    return this.store.createRecord('beer');
}
```

