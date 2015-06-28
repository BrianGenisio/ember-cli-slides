##  Create a 'new' controller

```javascript
ember generate controller beer/new
```

### Add the Create and Cancel actions

```javascript
actions: {
  create: function() {
    this.model
      .save()
      .then(() => this.transitionToRoute('beer'));
  },

  cancel: function() {
    this.model.destroyRecord();
    this.transitionToRoute('beer');
  }
}
```
