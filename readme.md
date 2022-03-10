MongoDB CRUD:

Insert:
```javascript
db.books.inserMany([
    {
    title: "nameOne",
    description: "desc one",
    authors: "J.A.One"
    },
    {
    title: "nameTwo",
    description: "decs two",
    authors: "D.M.Two"
    },
  ]
)
```
Find:
```javascript
db.books.find({
  title: {
    $in: ['name'],
  }
})
```
Update:
```javascript
db.books.updateMany(
  {title: {
    $in: ['name'],
    }},
  {$set: {
    'description': 'updated desc'
    }
  }
)
```