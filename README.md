# doco-cd example 

This repo demonstrates the minimum needed ot use doco to deloy a Docker Compose stack.

It comprises three files:
- `.doco-cd.yml` this file controls the behaviour of doco-cd and what is deployed
- `compose.yaml` this is a standard docker compose file
- `test.md` this is a dummy file for testing the push webhook triggering

## Example commit

To force a dummy update:

```bash
uuidgen > test.md && git add test.md && git commit -m "Update test.md" && git push
```

You can then view the updated service on `localhost:8080`
