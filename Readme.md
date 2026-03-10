# Rally

![Quad](https://github.com/chrishulbert/rally/raw/main/readme/quad.png)

A builder and player for rally challenges. Eg multiple teams in multiple cars, in real life, driving around, following clues between waypoints to a final destination.

Work in progress!

## HTTPS

![Trike](https://github.com/chrishulbert/rally/raw/main/readme/trike.png)

To use Geolocation, HTTPS is essential. When developing, use Caddy to get https, like so:

* Install caddy: brew install caddy
    * Downloads from the caddyserver.com site/github don't seem to work.
* To host locally with https, run this from the same folder as index.html:
    * caddy file-server --domain localhost
    * It might ask for password for setting up the certs
* To get the browser to accept the certificate:
    * sudo caddy trust
    * It might whinge about not reaching "http://localhost:2019/pki/ca/local" but should still work.
* Then open https://localhost in browser, should be ok
* The Makefile has a target to automate this:
    * `make serve`

## Etc

![Tank](https://github.com/chrishulbert/rally/raw/main/readme/tank.png)

[What are these images?](https://en.wikipedia.org/wiki/Dune_II)
