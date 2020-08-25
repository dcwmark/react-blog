[https://www.youtube.com/watch?v=RlAf28FYJRE](https://www.youtube.com/watch?v=RlAf28FYJRE)

[https://github.com/rivera1294/reactblog](https://github.com/rivera1294/reactblog)

> npm i concurrently json-server react-router-dom


---

Added to package.json

```js
  "scripts": {
    ...
        "json-server": "json-server --watch db.json --port 5000",
        "dev": "concurrently \"npm start\" \"npm run json-server",
    ...
```

---

Before any other changes:

> npm run dev

json-server would have created db.json

Browser > localhost:5000/posts

```json
[
  {
    "id": 1,
    "title": "json-server",
    "author": "typicode"
  }
]
```
