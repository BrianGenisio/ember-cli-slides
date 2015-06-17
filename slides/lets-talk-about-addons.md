##  Lets talk about addons

### Include Bootstrap
```javascript
ember install ember-bootstrap
```

### Use a Real Backend
```javascript
ember install ember-parse-adapter
```

### Replace the Application Adapter/Serializer
```javascript
ember generate serializer application
```

```javascript
import adapter from 'ember-parse-adapter/adapters/application';
export default adapter;

import serializer from 'ember-parse-adapter/serializers/application';
export default serializer;

APP: {
  applicationId: 'Ik9TL1QHMFbMIumhpCvwx5tNn2kSItKAcEnPAdOO',
  restApiId: 'hjX8ij6NepWbEDqB49Wo98udziyeD6IsiHGnWT0k'
}
```
