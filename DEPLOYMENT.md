# Frontend Deployment Guide - Vercel

## ✅ Code Pushed to GitHub
Repository: https://github.com/Ritika-Bhattia2177/capstone-industry-projF.git

## Deploy to Vercel

### Step 1: Go to Vercel Dashboard
Visit: https://vercel.com/dashboard

### Step 2: Import Project
1. Click **"Add New Project"**
2. Click **"Import Git Repository"**
3. Select: `Ritika-Bhattia2177/capstone-industry-projF`

### Step 3: Configure Project
- **Framework Preset**: Vite
- **Root Directory**: `./` (leave as default)
- **Build Command**: `npm run build`
- **Output Directory**: `dist`
- **Install Command**: `npm install`

### Step 4: Environment Variables
Add this environment variable in Vercel:

**Key**: `VITE_API_URL`  
**Value**: `https://your-backend-url.vercel.app/api`

Replace `your-backend-url` with your actual backend Vercel URL from the backend deployment.

Example:
```
VITE_API_URL=https://backend-bice-theta-52.vercel.app/api
```

### Step 5: Deploy
Click **"Deploy"** button and wait for deployment to complete.

## After Deployment

### Test Your Application
Once deployed, you'll get a URL like: `https://your-frontend.vercel.app`

Test these features:
1. ✅ Login page loads
2. ✅ Doctor search works
3. ✅ Appointments can be viewed
4. ✅ Dashboard shows data
5. ✅ Booking flow works

### Common Issues & Solutions

#### Issue: API calls fail with 404
**Solution**: Make sure `VITE_API_URL` is set correctly in Vercel environment variables with `/api` at the end.

#### Issue: Blank page after deployment
**Solution**: Check browser console for errors. Usually means API URL is incorrect.

#### Issue: Data not loading
**Solution**: 
1. Verify backend is deployed and working
2. Test backend URL directly in browser: `https://your-backend-url.vercel.app/api/doctors`
3. Check CORS is enabled on backend

### Update API URL
If you need to update the backend URL later:
1. Go to Vercel project settings
2. Navigate to **Environment Variables**
3. Edit `VITE_API_URL`
4. Redeploy the project

## Deployment Checklist

- [x] Code pushed to GitHub
- [ ] Vercel project created
- [ ] Environment variables set (VITE_API_URL)
- [ ] Build successful
- [ ] Deployment successful
- [ ] Application tested and working
- [ ] Backend URL configured correctly

## Custom Domain (Optional)

To add a custom domain:
1. Go to project settings in Vercel
2. Navigate to **Domains**
3. Add your custom domain
4. Update DNS records as instructed

## Automatic Deployments

Now configured for automatic deployments:
- Push to `main` branch → Auto deploy to production
- Pull requests → Preview deployments

## Repository Structure
```
frontend/
├── src/              # Source code
├── public/           # Static assets
├── dist/             # Build output (generated)
├── package.json      # Dependencies
├── vite.config.js    # Vite configuration
├── vercel.json       # Vercel configuration
└── README.md         # Documentation
```

## Support

If you encounter issues:
1. Check Vercel deployment logs
2. Check browser console for errors
3. Verify backend is running
4. Verify environment variables are set correctly
