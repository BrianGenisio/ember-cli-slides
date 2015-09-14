##  Component Use

Index Template
```html
{{beer-rating value=beer.rating model=beer onChange="updateRating"}}
```

Index Controller
```js
updateRating: function(beer, rating) {
  beer.set('rating', rating);
  beer.save();
},
```
