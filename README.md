# docker-latex
Full Tex Live LaTeX distribution based on Alpine Linux.

# Build
You don't need help to build a Docker image with Dockerfile and docker-compose.yaml available, do you? ;)

# Usage
Enter the directory containing your LaTeX source code and issue the following command:

```
docker run -ti -u $(id -u):$(id -g) --rm -v `pwd`:/src ppizzo/latex latex yourfile.tex
```

The image also contains the `make` command, to be used if needed.
