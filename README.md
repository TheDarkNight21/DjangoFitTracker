Django Fit Tracker

Overview

Fit Tracker is a Django-based fitness tracking web application designed to help users monitor their daily calorie intake, protein, carbohydrates, fats, and weight. It allows users to set nutritional goals, log daily meals and their nutritional information, and track progress over time through detailed visualizations and data summaries.

The application provides a user-friendly interface for creating and managing daily logs, setting fitness goals, and visualizing data using graphs and progress bars.

Features

	•	Basic Dashboard: Overview of current nutritional goals and progress.
	•	Daily Logs: Track meals, calories, proteins, carbs, and fats on a daily basis.
	•	Goal Management: Set and monitor nutritional and fitness goals.
	•	Data Visualization: Graphical representation of daily consumption and weight progress.
	•	Progress Indicators: Visual progress bars to track how close the user is to reaching their goals.

Project Structure

	•	views.py: Contains the core logic for rendering views, handling user inputs, and managing goals and logs.
	•	forms.py: Defines the forms used to capture user input, such as meals, weight, and dates.
	•	dashboard.html: The main dashboard view where users can track their goals and daily progress with various metrics and visual charts.
	•	logs.html: Displays a table of daily logs for meals, weight, and calories. Users can also navigate through the logs via pagination.

Setup and Installation

Prerequisites

	•	Python: Ensure you have Python 3 installed on your system.
	•	Django: Install Django using pip.
	•	SQLite: Default Django database (already set up).
	•	Chart.js: For rendering progress charts.

Installation Steps

	1.	Clone the repository: git clone https://github.com/yourusername/django-fit-tracker.git
	2.	Navigate to the project directory: cd django-fit-tracker
	3.	Install the required dependencies: pip install -r requirements.txt
	4.	Apply migrations: python manage.py migrate
	5.	Run the development server: python manage.py runserver
	6.	Access the application: Open your browser and go to http://127.0.0.1:8000/.

Usage

Dashboard

The dashboard provides an overview of the user’s fitness goals and their current progress toward reaching them. It displays:

	•	Calories, Proteins, Carbs, and Fats: Visual progress bars showing how close the user is to meeting their daily goals.
	•	Weight Tracking: Line chart displaying weight changes over time.

Daily Logs

The logs page allows users to record meals, weight, and calories consumed each day. It displays logs in a table format and allows pagination to navigate through previous entries.

Users can add meals and their respective nutritional values by filling out the daily log form. Each log tracks:

	•	Meal type: Breakfast, Lunch, Dinner, or Snack.
	•	Calories, Proteins, Carbs, and Fats: Nutritional values of the food consumed.
	•	Weight: Daily weight entry.
	•	Date: Date of the log.

Setting a Goal

Users can set a new nutritional goal by filling out the goal form, which includes:

	•	Calorie Goal
	•	Protein Goal
	•	Carbohydrates Goal
	•	Fats Goal
	•	Start and End Date

The goal form can be accessed from the dashboard if no active goal exists, or a user can update their goal at any time.

Data Visualization

The application utilizes Chart.js to render interactive graphs for:

	•	Calories, Proteins, Carbs, and Fats: Line graphs that display daily consumption trends.
	•	Weight: A graph to track weight changes over the course of the goal period.

Key Code Snippets

Adding Daily Logs: The user can log daily meals and nutritional values by submitting the log form.

Visual Progress: Progress indicators are dynamically generated based on user input and displayed on the dashboard.

Chart.js Data Visualization: Each nutrition category (calories, protein, carbs, and fats) is visualized using a line graph.

Future Enhancements

	•	Exercise Tracking: Add functionality to log daily exercises and display their impact on nutritional goals.
	•	Custom Notifications: Implement reminders for users to log their meals and update their weight.
	•	Multi-User Support: Extend the app to support multiple users with separate dashboards and logs.

License

This project is licensed under the MIT License.
