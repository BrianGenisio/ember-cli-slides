##  List some beers

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
