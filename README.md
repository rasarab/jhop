# jhop
🏎Create fake REST API in one sec.


## Example
Create a file `recipes.json`:
```json
{
  "recipes": [
    { "id": 1, "prep_time": "1h", "difficulty": "hard" },
    { "id": 1, "prep_time": "15m", "difficulty": "easy" }
  ]
}
```

Passing the JSON file to `jhop`:
```
~ $ jhop recipes.json
```

Now you can go to `localhost:6000/recipes` and get the response:
```json
{
  "recipes": [
    { "id": 1, "prep_time": "1h", "difficulty": "hard" },
    { "id": 1, "prep_time": "15m", "difficulty": "easy" }
  ]
}
```

## CLI usage
```
NAME:
   jhop - Create fake REST API in one sec.

USAGE:
   jhop [global options] command [command options] [arguments...]

VERSION:
   0.0.0

COMMANDS:
     help, h  Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --port value   Set port (default: "6000")
   --host value   Set host (default: "localhost")
   --help, -h     show help
   --version, -v  print the version
```

## TODO
- [ ] Plural routes
- [ ] Custom routes
- [ ] Middleware