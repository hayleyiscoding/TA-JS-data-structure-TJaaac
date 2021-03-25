```js
let user = {
  name: "Arya",
  sibling: ["Robb", "Ryan", "John"],
};
let allBrothers = ["Robb", "Ryan", "John"];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

<!-- To add this image here use ![name](./hello.jpg) -->

![screenshot](../hello.jpg)

2. Answer the following with reason:

- `user == newUser;` // false - datatype is an object which is only copy by reference
- `user === newUser;`// false - datatype is an object which is only copy by reference
- `user.name === newUser.name;` // "Arya" "Arya" true
- `user.name == newUser.name;`// true
- `user.sibling == newUser.sibling;` // false - copy by reference as they are arrays
- `user.sibling === newUser.sibling;` //false
- `user.sibling == allBrothers;`// false - copy by reference
- `user.sibling === allBrothers;` // false - copy by reference
- `brothersCopy === allBrothers;` // false - copy by reference
- `brothersCopy == allBrothers;` // false - copy by reference
- `brothersCopy == user.sibling;` // false - copy by reference
- `brothersCopy === user.sibling;`// false - copy by reference
- `brothersCopy[0] === user.sibling[0];` // false - copy by reference
- `brothersCopy[1] === user.sibling[1];` // false - copy by reference
- `user.sibling[1] === newUser.sibling[1];` // false - copy by reference
