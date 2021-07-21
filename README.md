### **For setting up a docker development environment for Elixir & Phoenix.**

* Set `PHOENIX_DOCKER_GENERATOR` to the path of this folder, for example if it's at `$HOME/repos/phx-docker-gen`, then put this in your .{z,bash}rc file:
`export PHOENIX_DOCKER_GENERATOR=$HOME/repos/phx-docker`
* Then stick the file `gen-phx` in your path.

Alternatively, just copy the files yourself from this directory to your phoenix project base directory.

* In config/dev.exs change `"hostname"` from `"localhost"` to `"db"`, or whatever you named the db service in docker-compose.yml, if you changed that.

https://96codes.dev/elixir-phoenix-development-using-docker-and-docker-compose

https://dev.to/hlappa/development-environment-for-elixir-phoenix-with-docker-and-docker-compose-2g17

Different than the above 2:
https://medium.com/swlh/use-docker-to-create-an-elixir-phoenix-development-environment-e1a81def1d2e
