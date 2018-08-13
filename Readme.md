# HydraConsole as a Docker container

> [HydraConsole](https://github.com/lanthaler/HydraConsole) is an implementation of a generic API client for Hydra-based Web APIs in the form of a single-page application.


## Start HydraConsole container

```bash
docker run --rm -p 8000:80 aveltens/hydra-console
```

Visit `http://localhost:8000` to reach the HydraConsole.

## Reach local APIs during development

To be able to reach locally started APIs, e.g. `http://localhost:8080` you need to start the container in the `host` network mode:

```bash
docker run --rm --network host aveltens/hydra-console
```

Now visit `http://localhost` to reach the HydraConsole and enter `http://localhost:8080/` as an URL there.