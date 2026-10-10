# 🚀 Deploy to Streamlit Cloud - Step by Step Guide

## Prerequisites
- GitHub account (free)
- Streamlit Cloud account (free - sign up at streamlit.io/cloud)

## Step-by-Step Deployment

### Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Name your repository: `talentscout-ai`
3. Set to Public
4. Click "Create repository"

### Step 2: Upload Files to GitHub

**Option A: Using Git Command Line**
```bash
# Navigate to your project folder
cd /path/to/talentscout-ai

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: TalentScout AI recruitment agent"

# Add remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/talentscout-ai.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Option B: Using GitHub Web Interface**
1. Go to your new repository
2. Click "uploading an existing file"
3. Drag and drop these files:
   - app.py
   - requirements.txt
   - README.md
4. Click "Commit changes"

### Step 3: Deploy on Streamlit Cloud

1. **Sign up for Streamlit Cloud**
   - Go to https://share.streamlit.io/
   - Click "Sign up with GitHub"
   - Authorize Streamlit to access your GitHub

2. **Create New App**
   - Click "New app" button
   - Repository: Select `YOUR_USERNAME/talentscout-ai`
   - Branch: `main`
   - Main file path: `app.py`
   - Click "Deploy!"

3. **Wait for Deployment**
   - Streamlit will install dependencies
   - Takes 2-5 minutes
   - Watch the deployment logs

4. **Get Your Live URL**
   - Your app will be live at:
   - `https://YOUR_USERNAME-talentscout-ai-main.streamlit.app`
   - Or similar URL assigned by Streamlit

### Step 4: Test Your Live App

1. Open the URL in your browser
2. Upload the sample resumes (provided)
3. Paste the sample job description
4. Click "Analyze Candidates"
5. See the magic happen! ✨

## 🎯 Your App is Now Live!

Share your URL with:
- Investors in pitch meetings
- Team members for feedback
- Potential customers for demo
- Anyone with the link can access it!

## 📱 Features of Your Deployed App

✅ Accessible from anywhere (mobile, desktop)
✅ Auto-updates when you push to GitHub
✅ Free SSL certificate (HTTPS)
✅ No server management needed
✅ Built-in analytics
✅ Zero hosting cost

## 🔧 Making Updates

To update your live app:
```bash
# Make changes to app.py
# Then push to GitHub:
git add .
git commit -m "Updated feature X"
git push

# Streamlit will auto-deploy in ~2 minutes!
```

## ⚙️ Advanced Settings (Optional)

In Streamlit Cloud dashboard:
- **Settings** → Secrets: Add API keys (for production AI)
- **Settings** → General: Change app name
- **Analytics**: View usage stats
- **Logs**: Debug issues

## 💡 Pro Tips

1. **Custom Domain**: Upgrade to add your own domain (requires paid plan)
2. **Private Apps**: Make app password-protected (requires paid plan)
3. **Resource Limits**: Free tier has limits, but plenty for demos
4. **Multiple Apps**: Deploy unlimited apps on free tier!

## 🎤 For Your Pitch

**When presenting:**
1. Pull up the live URL
2. Upload resumes in real-time
3. Show the AI analysis happening
4. Demonstrate the dashboard
5. Explain "This is running at $0/month"

**Key Points:**
- ✅ "This is a live, working system"
- ✅ "Deployed on production-grade infrastructure"
- ✅ "Zero hosting costs"
- ✅ "Can scale to 1000s of users"
- ✅ "Built in 2 weeks"

## 🐛 Troubleshooting

**App won't deploy?**
- Check requirements.txt has correct dependencies
- View logs in Streamlit Cloud dashboard
- Ensure all files are in root directory

**App is slow?**
- Free tier has resource limits
- Consider caching with @st.cache_data
- Optimize for production later

**Need help?**
- Streamlit docs: docs.streamlit.io
- Community forum: discuss.streamlit.io

## 🚀 Next Steps After Deployment

1. Share URL with stakeholders
2. Collect feedback
3. Plan production features
4. Get funding
5. Scale with paid infrastructure

---

**Congratulations! Your recruitment AI is live! 🎉**
