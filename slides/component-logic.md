##  Component Logic

```js
import Ember from 'ember';

export default Ember.Component.extend({
  tagName: 'span',
  model: null,
  value: 0,
  maxRating: 5,

  ratings: function() {
    let maxRating = this.get('maxRating');
    let value = this.get('value');

    return Array.from(new Array(maxRating), (x, i) => ({
      value: i + 1,
      isOn: value >= i + 1
    }));
  }.property('maxRating', 'value'),

  actions: {
    setRating: function(value) {
      this.sendAction('onChange', this.get('model'), value);
    }
  }
});
```
