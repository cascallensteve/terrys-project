# Gamezone - Peer-to-Peer Gaming Equipment Rental Platform

Gamezone is a web platform that enables gamers to rent out their gaming equipment to other gamers. The platform facilitates secure transactions, provides insurance options, and implements a rating system to build trust within the gaming community.

## Features

- User registration and profile management
- Equipment listing and search functionality
- Booking and reservation system
- Secure payment processing
- Geolocation services
- Basic insurance integration
- Customer support system
- User reviews and ratings
- Transparent pricing

## Tech Stack

- Django 5.0.2
- Python 3.x
- PostgreSQL
- HTML/CSS/JavaScript
- Bootstrap 5
- Stripe Payment Integration
- Leaflet Maps

## Setup Instructions

1. Clone the repository
```bash
git clone https://github.com/yourusername/gamezone.git
cd gamezone
```

2. Create and activate virtual environment
```bash
python -m venv gamezone_env
source gamezone_env/bin/activate  # On Windows use: gamezone_env\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Create .env file and set up environment variables
```bash
SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=your_database_url
STRIPE_PUBLIC_KEY=your_stripe_public_key
STRIPE_SECRET_KEY=your_stripe_secret_key
```

5. Run migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

6. Create superuser
```bash
python manage.py createsuperuser
```

7. Run the development server
```bash
python manage.py runserver
```

## Contributing

Please read CONTRIBUTING.md for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details 