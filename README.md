# Cascallen Portfolio Website

A modern, responsive portfolio website built with Django and TailwindCSS, featuring a beautiful blue color scheme.

## Features

- **Modern Design**: Clean, professional layout with blue/dark blue color scheme
- **Responsive**: Mobile-first design that works on all devices
- **Project Showcase**: Display of various projects including:
  - SmartStudy Assistant (Education/AI-ML)
  - Complimentary Fashions (Fashion/React)
  - Dream2 Homes (Real Estate/Next.js)
  - And more...
- **Interactive Elements**: Smooth animations and hover effects
- **Contact Form**: Easy way for clients to get in touch

## Technologies Used

- **Backend**: Django 5.2.1
- **Frontend**: TailwindCSS, HTML5, JavaScript
- **Database**: SQLite3
- **Static Files**: WhiteNoise
- **Deployment**: Vercel-ready configuration

## Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/cascallensteve/cascallen_Portfolio-web-updated.git
   cd cascallen_Portfolio-web-updated
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run migrations:
   ```bash
   python manage.py migrate
   ```

4. Collect static files:
   ```bash
   python manage.py collectstatic
   ```

5. Start the development server:
   ```bash
   python manage.py runserver
   ```

## Deployment

This project is configured for Vercel deployment. See [DEPLOYMENT.md](DEPLOYMENT.md) for detailed instructions.

## Project Structure

```
├── cascallen/           # Main Django app
│   ├── templates/       # HTML templates
│   ├── static/         # Static files (images, CSS, JS)
│   └── ...
├── portfolio/          # Django project settings
├── staticfiles/        # Collected static files
├── vercel.json         # Vercel configuration
├── vercel_app.py       # Vercel entry point
└── requirements.txt    # Python dependencies
```

## Featured Projects

- **SmartStudy Assistant**: An intelligent study companion with AI-powered assistance
- **Complimentary Fashions**: Modern fashion e-commerce platform built with React
- **Dream2 Homes**: Real estate platform with intuitive property search
- **AI Content Generator**: Intelligent content creation tool
- **Blockchain Voting**: Secure voting system ensuring transparency
- **AR Shopping Experience**: Immersive augmented reality shopping platform

## Contact

For inquiries or collaboration opportunities, please use the contact form on the website.

## License

This project is for portfolio purposes. All rights reserved.
