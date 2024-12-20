# Django-Task-Intern
# Django Inventory Management System

A comprehensive inventory management system built with Django that handles products, orders, and user management.

## Features

- User Authentication & Authorization
- Product Management
- Order Tracking
- Customer Management
- Staff Dashboard
- Profile Management

## Database Schema

### Core Models

| Model | Field | Description |
|-------|--------|-------------|
| Product | name | Product name (CharField) |
| Product | quantity | Available stock (PositiveIntegerField) |
| Product | category | Product category (CharField) |

| Model | Field | Description |
|-------|--------|-------------|
| Order | product | Foreign key to Product |
| Order | staff | Foreign key to User |
| Order | order_quantity | Quantity ordered (PositiveIntegerField) |


## Installation

1. Clone the repository
```bash
git clone https://github.com/Soumilgit/Django-Task-Intern.git
```

2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Run migrations
```bash
python manage.py migrate
```

5. Create superuser
```bash
python manage.py createsuperuser
```

6. Run the development server
```bash
python manage.py runserver
```

## Usage

1. Access the admin interface at `/admin`
2. Login with your credentials
3. Manage inventory through the dashboard
4. Track orders and stock levels
5. Generate reports

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Django Framework
- Bootstrap for frontend styling
- Contributors and maintainers
