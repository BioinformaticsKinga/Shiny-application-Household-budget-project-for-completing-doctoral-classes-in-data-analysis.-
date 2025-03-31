# Household Budget Management Shiny Application (in Polish, in some projects for crediting a subject in phD studies)
Project Overview
This project implements a Shiny application designed to manage a household budget. The application allows users to track their income, expenses, and savings goals. Users can input data for different categories of expenses (e.g., bills, food, transportation) and visualize the distribution of their spending and savings over time. The application is intuitive and easy to use, offering a simple way to manage personal finances effectively.

# Key Objectives
Track household income and expenses by adding amounts and categorizing them.

Visualize financial data through interactive charts to help identify spending patterns.

Manage savings goals by setting targets and monitoring progress.

Ensure accurate data entry with validation for expenses and income.

# Application Features
1. Income and Expense Tracking
Users can enter income amounts and associate them with a date.

Expenses are added to predefined categories such as Bills, Food, Transport, and more.

Both income and expenses are automatically saved and can be updated in real-time.

2. Savings Goals
Users can set savings goals by specifying a target amount and a name for the goal (e.g., "Vacation Fund").

The application tracks the progress of savings by showing the amount saved and the target.

3. Data Validation and Notifications
The application ensures that amounts entered for both income and expenses are valid, displaying error messages if an amount is 0 or negative.

4. Financial Visualizations
The application generates charts to visualize daily expenses and the breakdown of expenditures by category.

A summary of total income, total expenses, and current savings is displayed on the main interface.

5. Data Reset and File Management
Users can reset all data, clearing expenses, income, and goals from the application.

All data is saved in CSV files for persistent storage and can be easily loaded when the application is restarted.

# Workflow and Tools
1. Data Storage
The application stores financial data in CSV files:

expenses.csv for tracking expenses,

income.csv for recording income,

savings_goals.csv for monitoring savings goals.

The application checks for the existence of these files and loads the data if available. If not, it creates default empty data frames.

2. Shiny User Interface (UI)
The UI is designed with a clean and simple layout using the fluidPage() function. It includes:

Inputs for adding income, expenses, and savings goals.

Buttons for adding data and resetting information.

Outputs for displaying financial summaries and charts.

3. Server Logic
The server part of the application handles data processing, including:

Adding new income, expense, and savings data.

Calculating totals for income, expenses, and savings.

Generating plots for daily expense distribution and category breakdowns.

4. Data Visualization
Daily Expense Chart: A bar chart showing the distribution of expenses by date using ggplot2.

Expense Breakdown by Category: A pie chart or bar graph (if implemented) showing expenses categorized by type.

# Technologies and Libraries Used
Shiny: Framework for building interactive web applications in R.

ggplot2: Used for creating visualizations (graphs and plots).

dplyr: For data manipulation, especially filtering and summarizing data.

lubridate: To handle and manipulate date objects (e.g., income and expense dates).

# Results and Findings
Financial Overview: The application accurately calculates and displays total income, total expenses, and savings in real time.

Expense Tracking: It allows for an in-depth understanding of spending habits with visual charts illustrating daily expenses and expense categories.

Savings Goal Monitoring: Users can easily track the progress of their savings goals, improving financial planning.



