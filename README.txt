=======================================
DUSTIN JUN MENDOZA — PORTFOLIO WEBSITE  
=======================================

This is a personal portfolio website developed using HTML, CSS, JavaScript, and Flask (Python), with content dynamically loaded from an XML file (`data.xml`). It showcases Dustin Jun Mendoza's skills, talents, projects, services, organizations, and professional background in an interactive, animated, and responsive layout.

---------------------------------------
SECTION DESCRIPTIONS
---------------------------------------

1. HOME
-------
Displays the user's full name, profile photo, personal tagline, and location. Includes quick links to social media platforms like Facebook, Instagram, and Twitter. This serves as the welcoming banner of the website.

2. SKILLS & TALENTS
-------------------
Divided into two parts:
- **Technical Skills**: Lists programming and web development skills such as Python, HTML, CSS, and JavaScript.
- **Talents**: Highlights creative talents including Video Editing, Choreography, and Graphic Designing, with associated media previews (images and videos) shown on hover.

3. ORGANIZATIONS
----------------
Showcases participation in organizations with roles and years, including:
- TXT FANBASE – Admin (2018–2021)
- Dance Club – Member (2019–2021)

4. SERVICES
-----------
Details professional offerings such as:
- Web Design: Creating responsive and modern websites tailored to client needs.
- Tutoring: Personalized tutoring sessions in programming and web development.

5. PROJECTS
-----------
Highlights selected projects with descriptions, technologies used, links, and images. Example:
- PAIMON: A financial management system automating expenses, savings, and budget planning using HTML, CSS, and PHP.

6. TESTIMONIALS
---------------
Displays peer and client feedback with names and relationships, emphasizing professionalism and skill.

7. CONTACT
----------
Provides contact information and a contact form for visitors to reach out.

---------------------------------------
FLASK (PYTHON) BACKEND OVERVIEW
---------------------------------------
- The `app.py` file uses Flask to serve the `index.html` page and static assets.
- The application runs a local development server at `http://127.0.0.1:5000`.
- The `static/` directory contains all CSS, JavaScript, images, and XML data files.
- The frontend dynamically loads content from `data.xml` using JavaScript.
- Interactive UI features include navigation underline animation, burger menu toggle, media previews on talents, and testimonial animations on scroll.

Sample Python code (app.py):
```python
from flask import Flask, render_template
app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')

if __name__ == '__main__':
    app.run(debug=True)
```

---------------------------------------
HOW TO RUN LOCALLY?
---------------------------------------
1. Install Flask (if not already installed):
    pip install flask

2. Project Structure

    /project-root
    ├── app.py
    ├── /templates
    │   └── index.html
    └── /static
        ├── css
        │   └── style.css
        ├── js
        │   └── main.js
        ├── data
        │   └── data.xml
        └── images
            ├── anata.jpg
            ├── choreo.mp4
            ├── kyubi.jpg
            └── ... (other media files)

3. Run the app:
    python app.py

4. Visit http://127.0.0.1:5000 in your browser.

CREDITS:
Developed by: Dustin Jun Mendoza
Location: Silago, Southern Leyte, Philippines
