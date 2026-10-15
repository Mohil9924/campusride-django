# CampusRide

A Django web application that connects college students who need rides with students who have empty seats.

## Features
- User registration, login, and logout (Django auth)
- Post rides with route, date, time, seats, and price
- Search rides by source, destination, and date
- Request seats with overbooking prevention
- Driver dashboard to approve / reject requests
- My Rides & My Requests history pages
- Django admin panel for all models

## Tech Stack
| Area | Technology |
|------|-----------|
| Language | Python 3 |
| Framework | Django 6 |
| Database | SQLite |
| Frontend | HTML, CSS, Bootstrap 5 |

## Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Apply migrations
python manage.py migrate

# Run the development server
python manage.py runserver
```

Then open http://127.0.0.1:8000

## Admin Panel
URL: http://127.0.0.1:8000/admin  
Username: `admin`  
Password: `admin123`

## Project Structure
```
CampusRide/
├── campusride/         # Project settings & root URLs
├── rides/              # Main app
│   ├── models.py       # Profile, Ride, RideRequest
│   ├── forms.py        # RegisterForm, RideForm, RideRequestForm
│   ├── views.py        # All views
│   ├── urls.py         # App URL patterns
│   ├── admin.py        # Admin registrations
│   └── templates/rides/
│       ├── base.html
│       ├── home.html
│       ├── register.html
│       ├── login.html
│       ├── post_ride.html
│       ├── ride_detail.html
│       ├── dashboard.html
│       ├── my_rides.html
│       └── my_requests.html
├── db.sqlite3
├── manage.py
└── requirements.txt
```
