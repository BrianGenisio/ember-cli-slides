##  Connect to a fake backend

```javascript
ember generate adapter application
```

### And set the adapter's namespace

```javascript
export default DS.RESTAdapter.extend({
  namespace: 'api'
});
```
