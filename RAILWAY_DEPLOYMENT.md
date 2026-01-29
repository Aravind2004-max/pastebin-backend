# Railway Deployment Guide

## Prerequisites
- Railway account (sign up free at https://railway.app)
- GitHub account with your repository pushed

## Steps to Deploy to Railway

### 1. Sign Up/Login to Railway
- Go to https://railway.app
- Sign in with GitHub or create account
- Allow Railway to access your GitHub repositories

### 2. Create New Project
- Click "New Project" button
- Select "Deploy from GitHub repo"
- Choose your GitHub repository: `Aravind2004-max/paste-bin-lite`

### 3. Configure Environment Variables (If Needed)
Add these environment variables in Railway project settings:
```
SPRING_DATASOURCE_URL=your_database_url
SPRING_DATASOURCE_USERNAME=your_username
SPRING_DATASOURCE_PASSWORD=your_password
SPRING_JPA_HIBERNATE_DDL_AUTO=update
```

### 4. Configure Port
- Railway automatically exposes port 8080
- Your application runs on: `https://{project-name}.up.railway.app`

### 5. Monitor & Manage
- View logs in Railway dashboard
- Monitor metrics and performance
- Configure custom domains if needed

## Railway Free Tier
- Free tier includes: $5/month free credit
- Perfect for hobby projects and testing
- Automatic scaling available
- SSL/TLS certificates included

## Application Configuration
The `Dockerfile` uses Java 21 with:
- Multi-stage build for optimized image size
- 512MB memory allocation
- Automatic port 8080 exposure

## Custom Domain (Optional)
After deployment, you can add a custom domain:
1. Go to Settings in your Railway project
2. Add custom domain (requires DNS configuration)

## Notes
- Database services can be added from Railway marketplace
- Both MySQL and PostgreSQL are available
- Each service gets automatic backups

## Support
- Railway Documentation: https://docs.railway.app
- Community Discord: https://discord.gg/railway
