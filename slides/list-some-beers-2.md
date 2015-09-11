##  List some beers

### Update the template
```html
<ul>
    {{#each model as |beer|}}
        <li>
            {{beer.name}}
            {{beer.brewery}}
            {{beer.profile}}
        </li>
    {{/each}}
</ul>
```
