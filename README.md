# doco-cd example 

This repo demonstrates the minimum needed ot use doco to deloy a Docker Compose stack.

It comprises three files:
- `.doco-cd.yml` this file controls the behaviour of doco-cd and what is deployed
- `compose.yaml` this is a standard docker compose file
- `index.html` this is a dummy file for testing the push webhook triggering

## Example commit

To force a dummy update:

```bash
echo "<h1>$(uuidgen)</h1>" > index.html && git add index.html && git commit -m "Update index.html" && git push
```

You can then view the updated service on `localhost:8080`
