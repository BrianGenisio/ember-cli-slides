##  Component Template

```html
{{#each ratings as |rating|}}
<i class="rating glyphicon glyphicon-{{if rating.isOn 'star' 'star-empty'}}"
   {{action 'setRating' rating.value}}></i>
{{/each}}
```
