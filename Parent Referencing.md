[[One to Many relationship in MongoDB]]

# Parent Referencing
#resource 

A child table/document is referencing to eats parent.

```json
// Category
{
  _id: "5db66dd1f4892d34f4f4451a",  
  name: "Node.js",
  description: "Node.js tutorial",
}

// Tutorials
{ _id: "5db66dcdf4892d34f4f44515",
  title: "Tutorial #1",  
  author: "bezkoder",
  category_id: "5db66dd1f4892d34f4f4451a"
}

{ 
  _id: "5db66dd3f4892d34f4f4451b",
  title: "Tutorial #2",
  author: "bezkoder",
  category_id: "5db66dd1f4892d34f4f4451a"
}
```