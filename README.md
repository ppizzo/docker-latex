# docker-latex
Tex Live LaTeX distribution.

[![](https://images.microbadger.com/badges/version/ppizzo/latex.svg)](https://microbadger.com/images/ppizzo/latex "Get your own version badge on microbadger.com")
[![](https://images.microbadger.com/badges/image/ppizzo/latex.svg)](https://microbadger.com/images/ppizzo/latex "Get your own image badge on microbadger.com")

# Build
You don't need help to build a Docker image with Dockerfile and docker-compose.yaml available, do you? ;)

# Usage
Enter the directory containing your LaTeX source code and issue the following command:

```
docker run -ti -u $(id -u):$(id -g) --rm -v `pwd`:/src ppizzo/latex latex yourfile.tex
```

The image also contains the `make` command, to be used if needed.
