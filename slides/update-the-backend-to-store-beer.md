##  Update the backend to store beer

```javascript
var count = 0;
var beers = [
    {
      id: count++, ...
    },
    {
      id: count++, ...
    }
];

beersRouter.get('/', function(req, res) {
  res.send({
    'beers': beers
  });
});

beersRouter.post('/', function(req, res) {
  var beer = req.body.beer;
  beer.id = count++;
  beers.push(beer);

  res.status(201).send(req.body);
});

app.use('/api/beers', require('body-parser').json(), beersRouter);
```

```javascript
npm install body-parser --save-dev
```