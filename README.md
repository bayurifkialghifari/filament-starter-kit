# Library

This Filament Starter Kit includes the following packages:

-   🚀 **[filament/filament](https://filamentphp.com/docs/3.x/admin/installation):** The core Filament admin panel for building modern, beautiful admin interfaces in Laravel.
-   🛡️ **[bezhansalleh/filament-shield](https://github.com/bezhansalleh/filament-shield):** Robust role and permission management for fine-grained access control.
-   📦 **[filament/spatie-laravel-media-library-plugin](https://filamentphp.com/docs/3.x/media-library/installation):** Integrates Spatie's Media Library for advanced file and media management.
-   📜 **[rmsramos/activitylog](https://github.com/rmsramos/activitylog):** Adds activity logging to track changes and user actions.
-   📂 **[saade/filament-laravel-log](https://github.com/saade/filament-laravel-log):** User-friendly interface for viewing Laravel logs directly from Filament.
-   🗂️ **[tomatophp/filament-media-manager](https://github.com/tomatophp/filament-media-manager):** Powerful media manager UI for handling files and folders.

This starter kit helps you quickly build secure, feature-rich admin panels with advanced media and activity management. ✨

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
