# Income and Expense Calculator

A fully functional web application to track income and expense transactions, built with HTML, CSS, and JavaScript. This project implements CRUD operations, local storage for data persistence, and a responsive design for both desktop and mobile devices. It includes features like filtering, searching, charting, exporting, and a dark/light theme toggle.

## Features

- *Add Transactions*: Input income/expense details (description, amount, type, category, date) with real-time validation.
- *Edit/Delete Transactions*: Modify or remove entries via modals, with a 5-second undo option for deletions.
- *Filter and Search*: Filter transactions by "All", "Income", or "Expense" using radio buttons, and search by description or category.
- *Balance Overview*: Displays total income, total expenses, and net balance, with negative balances highlighted in red.
- *Monthly Summary*: Shows a breakdown of income and expenses by month, with a customizable chart (bar, pie, line, doughnut, radar, polar area).
- *Export Options*: Export transactions as CSV, PNG, PDF, or Word within a selected date range.
- *Local Storage*: Persists transaction data and theme preference across sessions.
- *Dark/Light Mode*: Toggle between themes with styles adapting dynamically.
- *Responsive Design*: Optimized for desktop and mobile devices with media queries.
- *Accessibility*: Includes ARIA attributes and focus trapping for modals.
- *Pagination*: Limits transaction display to 10 per page for performance.
- *Animations*: Smooth transitions for adding, deleting, and filtering transactions.

## Tech Stack

- *HTML*: Semantic structure for the application.
- *CSS*: Custom styles with CSS variables for theming and responsive design.
- *JavaScript*: Core logic for CRUD operations, local storage, chart rendering, and export functionality.
- *External Libraries*:
  - [Chart.js](https://www.chartjs.org/) for visualizing monthly summaries.
  - [jsPDF](https://github.com/parallax/jsPDF) and [jspdf-autotable](https://github.com/simonbengtsson/jsPDF-AutoTable) for PDF export.
  - [docx](https://github.com/dolanmiu/docx) for Word document export.
  - [FileSaver.js](https://github.com/eligrey/FileSaver.js/) for file downloads.

## Installation

1. Clone the repository or download the source code.
2. Open index.html in a web browser to run the application locally.
3. No additional setup is required as all dependencies are loaded via CDN.

## Usage

1. *Add a Transaction*:
   - Fill in the form with description, amount, type, category, and date.
   - Click "Add Transaction" to save. The transaction appears in the list, and totals/chart update.
2. *Edit/Delete*:
   - Click "Edit" to modify a transaction in a modal.
   - Click "Delete" to confirm deletion via a modal, with an undo option for 5 seconds.
3. *Filter and Search*:
   - Use radio buttons to filter by "All", "Income", or "Expense".
   - Type in the search bar to filter by description or category.
4. *View Summary*:
   - Check the balance section for total income, expenses, and net balance.
   - View the monthly summary and select a chart type to visualize data.
5. *Export Data*:
   - Select a date range and export format (CSV, PNG, PDF, Word).
   - Click "Export" to download the file.
6. *Reset Data*:
   - Click "Reset All Data" to clear all transactions (with confirmation).
   - Use "Clear Form" to reset the input form.
7. *Toggle Theme*:
   - Click "Toggle Dark Mode" to switch between light and dark themes.

## Project Structure

- index.html: Main HTML file with structure and CDN links.
- style: CSS with variables, responsive design, and animations.
- script: JavaScript for CRUD operations, local storage, chart rendering, and exports.
- No external assets are required.

## Notes

- The application uses localStorage to persist data. Ensure your browser allows local storage.
- The chart is hidden when no transactions exist to avoid clutter.
- Error handling is implemented for local storage issues and invalid inputs.
- The PNG export includes the chart (if transactions exist) and a table of transactions.

## Future Improvements

- Add user authentication to manage multiple users' data.
- Implement advanced filtering (e.g., by category or date range).
- Integrate a backend (e.g., Node.js) for cloud storage.
- Replace custom CSS with TailwindCSS for faster styling.
- Add more chart customization options (e.g., colors, labels).

## License

This project is open-source and available under the [MIT License](LICENSE).
