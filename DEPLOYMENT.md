# Vercel Deployment Guide

## Files Created for Vercel:

1. **vercel.json** - Vercel configuration file
2. **vercel_app.py** - Entry point for Vercel
3. **.vercelignore** - Files to ignore during deployment
4. **build.sh** - Build script (optional)

## Updated Files:

1. **portfolio/settings.py** - Added Vercel support and environment variables
2. **requirements.txt** - Fixed encoding issues

## Steps to Deploy:

1. **Push to GitHub**: 
   ```bash
   git add .
   git commit -m "Add Vercel deployment configuration"
   git push origin main
   ```

2. **Connect to Vercel**:
   - Go to [vercel.com](https://vercel.com)
   - Sign in with GitHub
   - Click "New Project"
   - Select your repository
   - Click "Deploy"

3. **Environment Variables** (Set in Vercel dashboard):
   - `SECRET_KEY` - Your Django secret key
   - `DEBUG` - Set to `False` for production

## Important Notes:

- The app uses SQLite database (not recommended for production)
- Static files are handled by WhiteNoise
- The app is configured for serverless deployment
- Make sure your domain is added to ALLOWED_HOSTS in settings.py

## Local Development:

```bash
python manage.py runserver
```

## Production Commands:

```bash
python manage.py migrate
python manage.py collectstatic --noinput
```

## Troubleshooting:

- If deployment fails, check the Vercel logs
- Ensure all dependencies are in requirements.txt
- Check that ALLOWED_HOSTS includes your Vercel domain
