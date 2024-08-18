# Installation Guide

## Table of Contents

- [Local Installation](#local-installation)
- [Installation with Docker](#installation-with-docker)

### Local Installation

#### Prerequisites

- Python 3.11 or higher
- Django 4.2 or higher
- pip (Python package installer)

#### Steps

1. **Clone the repository**:

   ```bash
   git clone https://github.com/khodealib/doctor-booker.git
   cd doctor-booker
   ```

2. **Create and activate a virtual environment**:

   ```bash
   python -m virtualenv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations**:

   ```bash
   python manage.py migrate
   ```

5. **Run the development server**:

   ```bash
   python manage.py runserver
   ```

6. **Open your browser and navigate to**:
   ```
   http://127.0.0.1:8000/
   ```

### Installation with Docker

#### Prerequisites

- Docker
- Docker Compose

#### Steps

1. **Clone the repository**:

   ```bash
   git clone https://github.com/khodealib/doctor-booker.git
   cd doctor-booker
   ```

2. **Build and run the containers**:

   ```bash
   docker-compose up --build
   ```

3. **Create a superuser**:

   ```bash
   docker-compose exec web python manage.py createsuperuser
   ```

4. **Open your browser and navigate to**:
   ```
   http://127.0.0.1:8000/
   ```
