<a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a>
## How it works

The API is built with [Laravel](https://laravel.com/), making the most of the framework's features out-of-the-box.

The application is using a custom JWT auth implementation: [`app/Jwt`](./app/Jwt).

## Getting started

The preferred way of setting up the project is using [Laravel Sail](https://laravel.com/docs/sail),
for that you'll need [Docker](https://docs.docker.com/get-docker/) under Linux / macOS (or Windows WSL2).

### Installation

Clone the repository and change directory:

    git clone https://github.com/ritter4u/laravel-example-app.git
    cd laravel-example-app

Install dependencies (if you have `composer` locally):

    composer create-project

Alternatively you can do the same with Docker:

    docker run --rm -it \
        --volume $PWD:/app \
        --user $(id -u):$(id -g) \
        composer create-project

Start the containers with PHP application and PostgreSQL database:

    ./vendor/bin/sail up -d

(Optional) Configure a Bash alias for `sail` command:

    alias sail='[ -f sail ] && bash sail || bash vendor/bin/sail'

Migrate the database with seeding:

    sail artisan migrate --seed

## Usage

The API is available at `http://localhost:3000/api` (You can change the `APP_PORT` in `.env` file).
''' 
http://localhost:3000/api/articles 
'''

'''
http://localhost:3000/api/articles
'''
## Contributions

Feedback, suggestions, and improvements are welcome, feel free to contribute.

## License

The MIT License (MIT). Please see [`LICENSE`](./LICENSE) for more information.
