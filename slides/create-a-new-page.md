##  Create a 'new' page

```javascript
ember generate route beer/new
```

### Generate a temporary model
```javascript
model: function() {
    return this.store.createRecord('beer');
}
```

### Add a template
```html
<h2>Add a new Beer</h2>

<div class="col-md-6">
    <form {{action "create" on="submit"}}>
        <div class="form-group">
            <label for="breweryName">Brewery</label>
            {{input value=model.brewery class="form-control" id="breweryName"}}
        </div>

        <div class="form-group">
            <label for="beerName">Name</label>
            {{input value=model.name class="form-control" id="beerName"}}
        </div>

        <div class="form-group">
            <label for="beerStyle">Style</label>
            {{input value=model.style class="form-control" id="beerStyle"}}
        </div>

        <div class="form-group">
            <label for="beerAbv">ABV %</label>
            {{input value=model.abv class="form-control" id="beerAbv" type="number"}}
        </div>

        <div class="form-group">
            <label for="beerProfile">Profile</label>
            {{textarea value=model.profile class="form-control" id="beerProfile" rows="5"}}
        </div>      

        <button type="submit" class="btn btn-default">Create!</button>
        <button class="btn btn-primary" {{action "cancel"}}>Cancel</button>
    </form>
    
</div>
```

