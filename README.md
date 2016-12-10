# Slideshow Template

Allows me to work easily on Linux with my normal development tools to create
and deliver presentations using slideshows generated from markdown.

## Use it

```sh
sudo apt install pandoc rake &&\
  git clone --recursive https://github.com/ahri/slideshow.git &&\
  cd slideshow &&\
  rake -T &&\
  rake
```

## Dependencies

- [Pandoc](http://pandoc.org/)
- [reveal.js](http://lab.hakim.se/reveal-js/)
- [Google Chrome](http://www.google.com/chrome/)
- [Rake](https://ruby.github.io/rake/)

## Optional

- [Guard](http://guardgem.org/)
