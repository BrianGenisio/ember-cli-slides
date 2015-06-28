##  Connect to a fake backend

```javascript
ember generate http-mock beers
```

### And edit your backend

```javascript
{
    id: 1,
    name: "Oberon",
    ...
},
{
    id: 2
    name: "Final Absolution",
    ...
}
```

### Use Ember Data in Router

```javascript
model: function() {
    return this.store.find('beer');
}
```

