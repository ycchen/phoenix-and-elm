# PhoenixAndElm

To start your Phoenix app:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  * Install Node.js dependencies with `npm install`
  * Start Phoenix endpoint with `mix phoenix.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](http://www.phoenixframework.org/docs/deployment).

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: http://phoenixframework.org/docs/overview
  * Docs: https://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix

  mix phoenix.new phoenix_and_elm

  cd phoenix_and_elm

  mix ecto.create

  npm install --save elm-brunch

  mkdir web/elm

  elm package install elm-lang/html -y

  modified brunch-config.js

  added web/elm/Main.elm

  modified web/static/js/app.js

  iex -S mix phoenix.server

  http://localhost:4000

  ## create model

  $ mix phoenix.gen.model Contact contacts first_name last_name gender:integer birth_date:date location phone_number email headline:text picture

  mix ecto.migrate


### seed the contact model

Added faker package for populate Contact model

### use alias in iex
alias PhoenixAndElm.{Repo, Contact, Seeds}

instead of

	alias PhoenixAndElm.Repo
	alias PhoenixAndElm.Contact
	alias PhoenixAndElm.Seeds

## Part 2

### added scrivener_ecto allows you to paginate your Ecto queries with Scrivener.

#### added scrivener_ecto to mix.exs

mix deps.get

modified lib/phoenix_elm_contact/repo.ex for basic configuration for use Scrivener

modified web/router.ex

# web/elm folder
elm package install elm-lang/http -y
elm package install elm-community/json-extra -y
elm package install elm-lang/navigation -y
elm package install evancz/url-parser -y

# project root folder
> npm install --save-dev stylus-brunch nib
