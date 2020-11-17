# Easy Way Crash Course Graphql with Express

`npm install`

`npm start`

> localhost:8082/graphql

# Create dummy data
```graphql
mutation {
  createCourse(input: {
    courseName: "Js graphql"
    price: 100
    stack: MOBILE
    teachingAssists: [
      {
        firstName: "Yee"
        lastName: "yz"
        experience: 4
      },
      {
        firstName: "Wilker"
        lastName: "Soh"
        experience: 1
      }
    ]
  }) {
    id
    courseName
  }
}
```

# Query Data
```graphql
query {
  getCourse(id: "getIDFromMutation") {
    id
    teachingAssists {
      firstName
    }
  }
}

```
