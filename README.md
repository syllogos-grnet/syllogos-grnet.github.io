# Σύλλογος Εργαζομένων και Συνεργατών ΕΔΥΤΕ

#### syllogos.grnet.gr web site

Build with jekyll for GH pages

### Guidelines for local testing

1. Clone/pull https://github.com/github/pages-gem
1. `make image`
1. Run container from this work dir:

```
PORT=4000
docker run -it --rm -p $PORT:$PORT -u `id -u`:`id -g` -v "$PWD":/src/site -e JEKYLL_ENV=production gh-pages jekyll serve -H 0.0.0.0 -P $PORT
```
