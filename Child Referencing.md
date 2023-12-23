[[One to Many relationship in MongoDB]]

# Child Referencing
#resource 

A parent table/document is referencing a child table/document.

```json
// Tutorial
{
  _id: "5db579f5faf1f8434098f7f5"
  title: "Tutorial #1",
  author: "bezkoder"
  comments: [ "5db57a03faf1f8434098f7f8", "5db57a04faf1f8434098f7f9" ],
}

// Comments
{
  _id: "5db57a03faf1f8434098f7f8",
  username: "jack",
  text: "This is a great tutorial.",
  createdAt: 2019-10-27T11:05:39.898Z
}

{
  _id: "5db57a04faf1f8434098f7f9",
  username: "mary",
  text: "Thank you, it helps me alot.",
  createdAt: 2019-10-27T11:05:40.710Z
}
```