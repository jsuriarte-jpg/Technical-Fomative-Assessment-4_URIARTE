# CodeIgniter POS — TFA4

A CodeIgniter 4 POS project with customer and user accounts, forms,
avatar upload, staff login, sessions, protected routes, and logout.

## Local setup

1. Run `composer install`.
2. Copy `env` to `.env`.
3. Set the base URL, MySQL credentials, and a private
   `POS_DEMO_PASSWORD` of at least 12 characters in `.env`.
4. Import `database/pos_tfa4.sql` into MySQL once.
5. Run `php spark db:seed PosDemoSeeder` once.
6. Run `php spark serve --port 8084`.
7. Visit `http://localhost:8084/`.

The seeder creates five customers and five staff accounts. To sign in,
use `admin01` and the password you set in `.env`.

Home and About are public. Customer and User pages require login.
Do not commit `.env` or real passwords to the repository.