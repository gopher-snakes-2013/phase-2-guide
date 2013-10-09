# Params

* Params are how sinatra gets information from the user
* Params are accessed just like a hash
* All param values are strings

Given the form:

```
<form>
  <input name="car" type="text">
  <input name="bike" type="text">
  <input type="submit">
</form>
```

When I click the submit button
Then the params come in as a hash like:

```
p params
{
  "car" => "Mercedes",
  "bike" => "Cannondale"
}

```

You can also use nested params to get multiple stuff!

```
<form>
  <input name="vehicle[]" type="text" value="Car">
  <input name="vehicle[]" type="text" value="Bike">
  <input type="submit">
</form>
```

When I click the submit button
Then the params come in as a nested hash like:

```
p params
{
  "vehicle" => [
    "Car",
    "Bike"
  ]
}
```

You can also use nested params to get params as a hash.







```
<form>
  <input name="vehicle[make]" type="text" value="Mercedes">
  <input name="vehicle[model]" type="text" value="AMG 65">
  <input type="submit">
</form>
```

Gives you

```
p params
{
  "vehicle" => {
    "make" => "Mercedes",
    "model" => "AMG 65"
  }
}

```
