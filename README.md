# LiveMesh

LiveMesh is a real-time classroom sync tool for interactive slide presentations. It allows teachers to present slides that update live on students’ devices, enabling real-time polls, participation, and event tracking. Built with Ruby on Rails 7, Turbo, and ActionCable.

## Ruby version

- Ruby 3.2.x
- Rails 7.x

## System dependencies

- PostgreSQL
- Redis
- Node.js and Yarn

## Configuration

1. Copy `.env.example` to `.env` and configure the required environment variables.
2. Set up `config/database.yml` and `config/cable.yml` according to your local environment.

## Database creation

```sh
bin/rails db:create
bin/rails db:migrate

Database initialization

bin/rails db:seed

How to run the test suite

bin/rails test

Services
	•	ActionCable via Redis for real-time updates
	•	Turbo/Hotwire for instant UI rendering
	•	Optional: Sidekiq (planned for future background jobs)

Deployment instructions
	1.	Ensure Redis and PostgreSQL are available in the target environment.
	2.	Set environment variables accordingly.
	3.	Run:

bundle install
yarn install
bin/rails assets:precompile
bin/rails db:migrate
bin/rails server

License

MIT

