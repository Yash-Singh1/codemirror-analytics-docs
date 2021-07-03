# Rest API

This is the Rest API docs that is used internally.

## `/api/push`

- Method: POST
- Content-Type: application/json
- Body Schema:

```js
{
  "id": "YOUR_ID",
  "...": "... (other event keys and values)"
}
```

This route takes a JSON as the body which contains the id and other event information.

Here are the events used internally:

```js
{
  "type": "OPEN"
}
```

or

```js
{
  "type": "MODE_CHANGE",
  "mode": "string or null"
}
```

or

```js
{
  "type": "THEME_CHANGE",
  "theme": "string or null"
}
```

## `/api/events`

- Method: POST
- Content-Type: application/json
- Body Schema:

```js
{
  "id": "YOUR_ID"
}
```

Takes an id in the JSON and returns the events as an array that are stored.
