# NexusPay Admin - Netlify Deployment Guide

## Environment Variables
Set these in your Netlify dashboard under Site Settings > Environment Variables:

### Supabase Configuration
```
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url_here
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key_here
```

### Email Configuration (for report sending)
```
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_email_app_password
```

### Twilio Configuration (for WhatsApp alerts)
```
TWILIO_ACCOUNT_SID=your_twilio_account_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_WHATSAPP_NUMBER=whatsapp:+your_twilio_whatsapp_number
```

## Deployment Steps

1. **Push your code to a Git repository** (GitHub, GitLab, or Bitbucket)
2. **Connect your repository to Netlify**
3. **Set environment variables** in Netlify dashboard
4. **Deploy** - Netlify will automatically build and deploy your site

## Build Configuration
- **Build Command**: `npm run build`
- **Publish Directory**: `.next`
- **Node Version**: 18

## Features
- ✅ Static site generation for optimal performance
- ✅ Serverless API routes for email and SMS functionality
- ✅ Responsive design with Tailwind CSS
- ✅ Modern React components with Radix UI
- ✅ Real-time database integration with Supabase

## Notes
- API routes are automatically converted to Netlify Functions
- Environment variables are securely handled by Netlify
- The site is optimized for production with Next.js best practices
