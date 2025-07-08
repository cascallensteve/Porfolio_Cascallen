# AGENT.md

## Commands
- **Run Django dev server**: `python manage.py runserver`
- **Run migrations**: `python manage.py makemigrations && python manage.py migrate`
- **Install dependencies**: `pip install -r requirements.txt`
- **Collect static files**: `python manage.py collectstatic`
- **Run tests**: `python manage.py test cascallen`

## Architecture
- **Django 5.2** portfolio project with single `cascallen` app
- **Database**: SQLite3 (db.sqlite3)
- **Static files**: Handled by WhiteNoise, collected to `staticfiles/`
- **Templates**: Located in `cascallen/templates/`
- **Deployment**: Configured for Render (porfolio-cascallen.onrender.com)

## Code Style
- **Colors**: Use blue/dark blue and white color scheme - **NO GREEN colors anywhere**
- **CSS**: TailwindCSS for styling, custom gradients using blue shades (#1e3a8a, #1e40af, #1d4ed8, #2563eb, #3b82f6)
- **Templates**: Django templates with `{% load static %}` for assets
- **Python**: Follow Django conventions, use class-based or function-based views
- **Static files**: Store in `cascallen/static/` directory
- **Responsive**: Mobile-first design with Tailwind classes
