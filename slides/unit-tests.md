##  Unit Tests?

### localhost:4200/tests

```js
test('it destroys object when canceled', function(assert) {
  let destroyed = false;
  let controller = this.subject();

  controller.model = {
    destroyRecord: function() {
      destroyed = true;
    }
  };

  controller.transitionToRoute = () => {};

  controller.send('cancel');

  assert.ok(destroyed);
});
```
