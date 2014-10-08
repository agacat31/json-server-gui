JSON Server GUI
===============

What?
-----

The `json-server` module starts a server exposing a dynamic REST API: any call to `/somethings` on your server will act like a standard REST API with no schema constraint. Checkout [the project](https://github.com/typicode/json-server) for more information.

`JSON Server GUI` just adds a GUI on top, based on `node-webkit`.

Why?
----

During JavaScript trainings you may want your trainees to work with a REST API (let's say, when you talk about Ajax :)). The best way would be to provide a single executable they can click on, and start experiments.

With this very simple GUI they can see the data in real time, and the requests they played. They have a direct feedback, without the need to tell them how to install a server, use a CLI, or even host your own server.

How?
----

Clone the repository, then run `make`. The project will build for Linux (32 & 64 bits), Windows (32 bits), and Max OSX.

It can last about a century first time as it will download all corresponding `node-webkit` distributions.

To build specific for a specific platform:

```sh
make build-linux32
make build-linux64
make build-windows
make build-osx
```