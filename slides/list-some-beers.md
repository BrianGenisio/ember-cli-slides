##  List some beers

```javascript
ember generate route beer/index
```

### Update the route with data
```javascript
model: function() {
    return [
      {
        name: "Oberon",
        brewery: "Bells",
        profile: "Wheat and citrus"
      },
      {
        name: "Final Absolution",
        brewery: "Dragonsmead",
        profile: "Belgian Tripel"
      }
    ]
  }
```

### Update the template
```html
<ul>
    {{#each beer in model}}
        <li>
            {{beer.name}}
            {{beer.brewery}}
            {{beer.profile}}
        </li>
    {{/each}}
</ul>
```