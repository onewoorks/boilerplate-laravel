# Boilerplate for Laravel Web Application

This Boilerplate include basic front end library such as jQuery, Bootstrap and Font Awesome.

Other than that, Laravel package included is Laratrust - used for ACL, Collective - a Form Helpers.

## Installation

Run the following command

	composer create-project nasrulhazim/boilerplate-laravel your-project-name

If you were asked to remove Git history, just choose `Y`.

## Configuration

Open `.env` and configure your database name, username and password

Run the following command to setup the database tables and seeding default ACL

	php artisan migrate && php artisan db:seed

You may run `php artisan serve` to start using the Boilerplate for Laravel Web Application

## Others

You may use `js/delete.js` if you want to have prompt message upon delete a record.

Include the `js/delete.js` in your view

	<script type="text/javascript" src="{{ url('js/delete.js') }}"></script>

Usage example

	<a href="posts/2" data-method="delete" data-token="{{csrf_token()}}"> 

Or, request confirmation in the process

	<a href="posts/2" data-method="delete" data-token="{{csrf_token()}}" data-confirm="Are you sure?">

