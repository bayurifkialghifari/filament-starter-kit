# Library

This project uses [Filament Shield](https://github.com/bezhanSalleh/filament-shield) for role and permission management, and [Filament Media Library](https://github.com/ralphjsmit/filament-media-library) for file and media uploads within the Filament admin panel.

# SETUP

1. **Clone the repository:**

    ```bash
    git clone
    cd filament-starter
    ```

2. **Install dependencies:**

    ```bash
    composer install
    ```

3. **Copy and configure environment file:**

    ```bash
    cp .env.example .env
    php artisan key:generate
    ```

4. **Set up the database:**

    - Update your `.env` file with your database credentials.
    - Run migrations and seeders:
        ```bash
        php artisan migrate
        ```

5. **Set up the filament shield:**

    - Publish the Filament Shield configuration:

    ```bash
    php artisan shield:generate --all
    ```

    - Configure the shield by editing `config/filament-shield.php` as needed.

6. **Create an admin user:**

    - You can create an admin user using the following command:

    ```bash
    php artisan shield:super-admin
    ```

    - Follow the prompts to set up your admin user.

7. **Serve the application:**

    ```bash
    php artisan serve
    ```

8. **Access the Filament admin panel:**
    - Visit `http://localhost/admin` and log in with your admin credentials.
