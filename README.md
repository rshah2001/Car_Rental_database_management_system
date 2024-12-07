# Car Rental Management System

This project is a **Streamlit-based Car Rental Management System** designed for managing various aspects of a car rental business. It includes features for reservations, vehicle management, customer analytics, maintenance tracking, and more. The app is built using Python, PostgreSQL, and several data visualization components to provide a user-friendly and functional interface.

## Features

### 1. **Reservations**
- Create, view, update, and cancel reservations.
- Display available vehicles and calculate costs based on rental duration and customer type.
- Apply discounts for premium customers.

### 2. **Vehicle Management**
- View details of all vehicles.
- Add, update, or delete vehicle information.
- Assign vehicles to specific locations or employees.

### 3. **Customer Analytics**
- Customer overview with rental history and spending analysis.
- Loyalty scoring and insights into customer feedback.
- Visualizations of preferred vehicle categories and spending by account type.

### 4. **Support Tickets**
- Create, view, and manage support tickets.
- Highlight urgent and overdue tickets.
- Analyze ticket trends and common issues.

### 5. **Maintenance Management**
- View vehicles requiring maintenance.
- Schedule maintenance tasks and assign technicians.
- Track maintenance history and costs.

### 6. **Reports and Analytics**
- Generate reports on rental performance, high-value customers, and vehicle maintenance.
- Visualize revenue trends and category-based analytics.

### 7. **Location Analytics**
- Analyze performance metrics for different locations.
- Compare revenue, fleet composition, and maintenance costs across locations.

## Requirements

- Python 3.8 or later
- PostgreSQL database
- Required Python packages (install using `pip install -r requirements.txt`):
  - `streamlit`
  - `pandas`
  - `numpy`
  - `sqlalchemy`
  - `psycopg2-binary`

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/car-rental-system.git
   cd car-rental-system
   ```

2. **Configure the database:**
   - Update the `engine` variable in `CarRentalUI.py` with your PostgreSQL connection details.

3. **Run the application:**
   ```bash
   streamlit run CarRentalUI.py
   ```

4. **Access the application:**
   - Open the link generated in the terminal (typically `http://localhost:8501`) in your web browser.

## Database Schema

- The system interacts with several database tables, including:
  - `app_user` (user details)
  - `vehicle` (vehicle details)
  - `reservation` (reservation records)
  - `vehicle_category` (vehicle categorization)
  - `car_care` (maintenance tracking)
  - `support` (support tickets)
  - Additional views for analytics, such as `high_value_customers`.

## Key Notes

- The application uses a PostgreSQL database and requires stored procedures and views for some operations (e.g., `calculate_customer_loyalty`).
- Modify the SQL queries in `CarRentalUI.py` as needed to adapt to your specific database schema.

## Contributing

Contributions are welcome! Feel free to submit issues or create pull requests.
