##  Use Sinon Instead

```
ember install ember-sinon
```

```js
app.import('bower_components/sinonjs/sinon.js');
```

```js
import sinon from 'sinon';

test('it transitions to "beers" when canceled', function(assert) {
  let controller = this.subject();

  controller.model = { destroyRecord: sinon.spy() };
  controller.transitionToRoute = sinon.spy();

  controller.send('cancel');

  assert.ok(controller.transitionToRoute.calledWith('beer'));
});

```