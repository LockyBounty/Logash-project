My Logash


# Lodash 101

Lodash is one of the most popular utility-belt library. It can make you very productive and effective in writing Javascript programs. Check the npm [here](https://www.npmjs.com/package/lodash)

## Examples
#### Array of numbers

Let's create a data array withthe contents: 1,2,3,4,5. This array has 5 items.

To get the first item, we can use lodash's _.first.

```javascript
return _.first(data)
```

The result is 1.

---

To get the first 3 elements, we can use lodash's _.take

```javascript
return _.take(data, 3)
```

The result is 1,2,3.

#### Array of objects

Let's create a data array consisting of objects.

We can dump the content using the dump filter.

[{"name":"John","age":45},{"name":"Mary","age":32},{"name":"Peter","age":54}]

To retrieve the name field from each object in this array, lodash's _.pluck is very handy.

```javascript
return _.map(data,(item)=> {console.log( item.name ) });
```

The result is John,Mary,Peter.

---


Using _.find, we can look up an object by its field.

Let's try to find out how old Mary is.

```return _.find(data, {name: 'Mary'})```

Mary is 32 years-old.
