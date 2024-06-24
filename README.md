# Community Chef

**Community Chef** is an innovative platform designed to connect local chefs, home cooks, and food enthusiasts in Australia. By providing a space for chefs to showcase their culinary talents and for users to discover personalized dining experiences, Community Chef addresses the challenge of limited dining options and high startup costs for aspiring chefs.

## Features

- **Chef Profiles:** Create and customize profiles, upload recipes, and manage availability.
- **Customer Accounts:** Create profiles, view chef calendars, book appointments, and make payments.
- **Communication:** Built-in chat feature for seamless interaction between chefs and customers.
- **SousChef:** An AI chatbot that suggests recipes based on listed ingredients.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Django, Python
- **Database:** PostgreSQL
- **Deployment:** Docker, AWS
- **Real-time Features:** Redis, Django Channels

## Getting Started

### Prerequisites

- Python 3.8+
- Docker (Latest)
- PostgreSQL

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/username/community-chef.git
    cd community-chef
    ```

2. **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    pip install -U 'channels[daphne]'
    pip install --upgrade openai
    pip install Pillow
    ```

4. **Set up Docker and Redis:**
    - **Install Docker:** Follow the instructions [here](https://docs.docker.com/engine/install/).
    - **Run Redis in Docker:**
      ```bash
      docker run --rm -p 6379:6379 redis:7
      ```

5. **Set up the PostgreSQL database:**
    ```bash
    docker-compose up -d
    ```

6. **Apply migrations:**
    ```bash
    python manage.py migrate
    ```

7. **Create a superuser:**
    ```bash
    python manage.py createsuperuser
    ```

8. **Run the development server:**
    ```bash
    python manage.py runserver
    ```

9. **Access the application:**
    Open your browser and go to `http://127.0.0.1:8000`

## Contributing

We welcome contributions! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.
