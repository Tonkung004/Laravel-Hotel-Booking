# Laravel-Hotel-Booking

> [!NOTE]  
> Hotel Booking System is an open-source project designed for managing hotel reservations. Built with modern web technologies, it provides an intuitive platform for both administrators and customers.

## Features

- Easy-to-use interface for hotel booking and management.
- Key functionalities include:
  - Room management
  - Reservation tracking
  - Customer account management
- Scalable architecture suitable for small to medium-sized hotels.

## Installation [Development Mode]

> [!IMPORTANT]  
> Ensure you have the required environment set up (e.g., PHP, MySQL). Clone the repository and follow the steps below:

```bash
git clone [repository-url]
cd Hotel-Booking-master
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve
```

## Usage Instructions

1. Launch the development server:
   ```bash
   php artisan serve
   ```
2. Open your browser and navigate to `http://localhost:8000`.
3. Log in with the default admin credentials (if provided in the seed data):
   - **Email**: `admin@example.com`
   - **Password**: `password`

## Example Usage

- **Administrator**:
  - Add, edit, or remove room details.
  - View all reservations.
  - Manage customer accounts.

- **Customer**:
  - Browse available rooms.
  - Make a reservation.
  - Manage personal booking history.

## Requirements

- PHP 8.0 or higher
- Composer
- MySQL or other supported database

## Optimize for Production Mode

1. Set the environment to production:
   ```bash
   nano .env
   # Set APP_ENV=production and APP_DEBUG=false
   ```
2. Optimize the application:
   ```bash
   php artisan optimize
   composer install --no-dev --optimize-autoloader
   ```

## Project Structure

```
Hotel-Booking-master/
├── app/                # Application logic
├── public/             # Public-facing files
├── resources/          # Views and assets
├── routes/             # Application routes
├── database/           # Migrations and seeders
├── .env.example        # Environment configuration example
├── composer.json       # PHP dependencies
└── README.md           # Project documentation
```

## Future Improvements

- Add payment gateway integration.
- Support for multi-language functionality.
- Enhanced reporting and analytics.
- Mobile-friendly design.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

<p align="center">
    Developed With ❤️ by [Your Name or Team Name]
</p>

