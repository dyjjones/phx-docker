### **For setting up a docker development environment for Elixir & Phoenix.**

1. Set `PHOENIX_DOCKER_GENERATOR` to the path of this folder, for example if it's at `$HOME/repos/phx-docker-gen`, then put this in your .{z,bash}rc file:
`export PHOENIX_DOCKER_GENERATOR=$HOME/repos/phx-docker`
2. Then stick the file `gen-phx` in your path.
3. Run `gen-phx appname`; appname should be underscore-case format. The script changes `"hostname"` from `"localhost"` to `"db"` in config/dev.exs; it needs to match the database service named in docker-compose.yml, in this case it is `db`.

For an existing project, follow steps 1 and 2 above and run `gen-phx-existing` inside the project folder. It will add the 3 Docker files (or overwrite them if they exist, adjust the script per your needs), set up the containers and run migrations.

https://96codes.dev/elixir-phoenix-development-using-docker-and-docker-compose

https://dev.to/hlappa/development-environment-for-elixir-phoenix-with-docker-and-docker-compose-2g17

Different than the above 2:
https://medium.com/swlh/use-docker-to-create-an-elixir-phoenix-development-environment-e1a81def1d2e


See this for options to pass to `mix phx.new`: https://hexdocs.pm/phoenix/Mix.Tasks.Phx.New.html