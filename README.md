# Flask App

This is a simple Flask application with:
- Template Inheritance
- Static Files (CSS & Images)
- Form Handling
- In-Memory Data Storage
- API Endpoint
- Custom Error Handling

## How to Install Dependencies and Run the App

1. Clone the repository:
   ```bash
   git clone https://github.com/Bavani1125/flaskapp
   cd flaskapp
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   venv\Scripts\activate    # On Windows
   ```

3. Run the Flask application:
   ```bash
   python app.py
   ```

5. Open in your browser:
   - Home: [http://127.0.0.1:5000/](http://127.0.0.1:5000/)
   - Feedback Form: [http://127.0.0.1:5000/feedback]
   - API JSON: GET /api/feedback

## Advanced and Optional Features

### 1. Template Inheritance
- All HTML pages extend `base.html`, ensuring a consistent layout with a header, footer, and navigation bar.

### 2. Static Files
- Uses a `static/css/style.css` file for styling.
- Allows the addition of images and other static assets in the `static/images/` directory.

### 3. Form Handling
- Users submit feedback through a form in `feedback.html`.
- The data is captured and displayed in `form_result.html`.

### 4. In-Memory Data Storage
- Feedback data is stored in a list and displayed on the `/all_feedback` page.
- Future enhancement: Connect to a database (e.g., SQLite or PostgreSQL) for persistent storage.

### 5. API Endpoint
- JSON data is served at `/api/feedback`, allowing external applications to fetch feedback data.
- Example API response:
  ```json
  [
      {"username": "jason", "comments": "Great app!"},
      {"username": "mark", "comments": "Needs more features."}
  ]
  ```

### 5. Custom Error Handling
- A `404.html` template provides a user-friendly error page when an invalid URL is accessed.

### 7. Future Enhancements
- **Database Integration**: Use SQLite/PostgreSQL for persistent data storage.
- **Authentication**: Implement user login/logout functionality.
- **Deployment**: Deploy on AWS/GCP/Heroku for public access.

---

**Author:** [Bavani1125](https://github.com/Bavani1125/flaskapp)



