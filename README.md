# daytona-test

Daytona repository: https://github.com/daytonaio/daytona

- `daytona server`
- select VSCode - Browser in `daytona ide`
- `ssh-keygen -t ed25519 -C "your_email@example.com"`
- try `https://github.com/daytonaio/go-devcontainer` in `daytona create`

or

```
curl -X "POST" "http://127.0.0.1:3000/workspace/" \
     -H 'Content-Type: application/json; charset=utf-8' \
     -d $'{
  "name": "sample-go",
  "target": "local",
  "repositories": [
    {
      "url": "https://github.com/daytonaio/sample-go"
    }
  ]
}'
```