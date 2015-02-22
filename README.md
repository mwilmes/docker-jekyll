# Simple Docker Container for Jekyll Work

Based on grahamc/jekyll. Includes additional asciidoc support.

Docker Hub: <https://registry.hub.docker.com/u/mwilmes/docker-jekyll/>

Use example:

```
sudo docker run --rm -v "$PWD:/src" mwilmes/docker-jekyll build
```

or for repeated calls:

```
alias jekyll='sudo docker run --rm -v "$PWD:/src" -p 4000:4000 mwilmes/docker-jekyll'
jekyll build
jekyll serve -H 0.0.0.0
```

run as a background daemon:
```
sudo docker run -d -v "$PWD:/src" -p 4000:4000 mwilmes/docker-jekyll serve -H 0.0.0.0
```

## Goodies
 - Supports pygments syntax highlighting
 - Supports Github Pages
 - Supports Jekyll Redirect From
 - Supports Kramdown
 - Supports RDiscount
 - Supports Rouge
 - Supports Asciidoctor (_plugins/jekyll-asciidoc.rb necessary in project)


# License: Public Domain

Do what you want!
