##  Create a 'new' page

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
            <label for="beerProfile">Profile</label>
            {{textarea value=model.profile class="form-control" id="beerProfile" rows="5"}}
        </div>      

        <button type="submit" class="btn btn-default">Create!</button>
        <button class="btn btn-primary" {{action "cancel"}}>Cancel</button>
    </form>
    
</div>
```
