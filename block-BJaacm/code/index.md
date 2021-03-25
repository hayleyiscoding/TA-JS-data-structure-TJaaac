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

![screenshot](./hello2.jpg)

2. Answer the following with reason:

- `user == newUser;` // true
- `user === newUser;`// true
- `user.name === newUser.name;` // "Arya" "Arya" primitive data type - true
- `user.name == newUser.name;`// true
- `user.sibling == newUser.sibling;` // true - stored at same address
- `user.sibling === newUser.sibling;` // true
- `user.sibling == allBrothers;`// false - different address
- `user.sibling === allBrothers;` // false 
- `brothersCopy === allBrothers;` // false - different address
- `brothersCopy == allBrothers;` // false 
- `brothersCopy == user.sibling;` // true
- `brothersCopy === user.sibling;`// true
- `brothersCopy[0] === user.sibling[0];` // true - primitive datatype
- `brothersCopy[1] === user.sibling[1];` // true
- `user.sibling[1] === newUser.sibling[1];` // true 
