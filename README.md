# 🎯 TalentScout AI - Recruitment Agent Demo

An intelligent AI-powered recruitment pre-screening system that automates candidate evaluation.

## ✨ Features

- 📄 **Resume Parsing**: Upload multiple resumes (TXT, PDF, DOCX)
- 🎯 **Smart Matching**: AI-powered job matching algorithm
- 📊 **Candidate Ranking**: Automatic scoring and ranking
- 💡 **Detailed Insights**: Strengths, concerns, and recommendations
- 📈 **Dashboard**: Visual analytics and metrics
- 💾 **Export**: Download results as JSON

## 🚀 Zero-Cost Deployment

### Option 1: Streamlit Cloud (Easiest - 5 minutes)

1. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/talentscout-ai.git
   git push -u origin main
   ```

2. **Deploy on Streamlit Cloud:**
   - Go to https://streamlit.io/cloud
   - Click "New app"
   - Connect your GitHub repo
   - Select `app.py` as main file
   - Click "Deploy"
   - **Done! Your app is live at:** `https://YOUR_APP.streamlit.app`

### Option 2: Local Testing

```bash
# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

Your app will open at `http://localhost:8501`

## 📦 Files Included

```
talentscout-ai/
├── app.py              # Main Streamlit application
├── requirements.txt    # Python dependencies
└── README.md          # This file
```

## 🎯 How to Use

1. **Enter Job Description**: Paste the job requirements
2. **Upload Resumes**: Upload one or more candidate resumes
3. **Click Analyze**: AI agent processes and ranks candidates
4. **Review Results**: See detailed analysis, scores, and recommendations
5. **Export**: Download results for your records

## 🔧 Production Upgrade Path

This demo uses simulated AI analysis. For production:

### Free AI APIs:
- **Groq** (Recommended): 14,400 requests/day free
  ```bash
  pip install groq
  ```
  
- **Google Gemini**: 15 requests/min free
  ```bash
  pip install google-generativeai
  ```

### Add Real AI (Example with Groq):

```python
from groq import Groq

client = Groq(api_key="YOUR_API_KEY")

def analyze_resume(resume_text, job_description):
    response = client.chat.completions.create(
        model="llama-3.1-70b-versatile",
        messages=[{
            "role": "user",
            "content": f"Analyze this resume against the job description...\n\nResume: {resume_text}\n\nJob: {job_description}"
        }]
    )
    return response.choices[0].message.content
```

## 💰 Cost Breakdown

| Component | Service | Cost |
|-----------|---------|------|
| Hosting | Streamlit Cloud | $0 |
| AI API | Groq (Free tier) | $0 |
| Database | SQLite | $0 |
| Domain | .streamlit.app subdomain | $0 |
| **Total** | | **$0/month** |

## 📈 Scalability

**Free Tier Limits:**
- Groq: 14,400 requests/day (~600/hour)
- Streamlit Cloud: Unlimited apps
- Processing: 50-100 resumes/batch

**Perfect for:**
- Startup demos
- MVP validation
- Small-scale hiring (100-500 candidates/month)

## 🎓 For Startup Pitch

**Key Talking Points:**
- ✅ Working prototype (live demo link)
- ✅ Zero infrastructure cost
- ✅ Proven AI technology
- ✅ 80% time savings vs manual screening
- ✅ Scalable architecture ready
- ✅ Fast time-to-market (2-4 weeks to production)

**Monetization Strategy:**
- Freemium: 50 resumes/month free
- Pro: $49/month (500 resumes)
- Enterprise: Custom pricing (unlimited + integrations)

## 🔮 Roadmap

**Phase 1 (Current):** ✅ Demo with core functionality

**Phase 2 (Post-funding):**
- Real AI API integration (Groq/Claude/Gemini)
- Email automation
- ATS integrations (Greenhouse, Lever)
- Advanced analytics

**Phase 3 (Scale):**
- Video interview analysis
- Multi-language support
- Custom AI models
- White-label solution

## 🤝 Contributing

This is a demo for startup pitch. For production deployment:
1. Add proper authentication
2. Integrate real AI APIs
3. Add database (PostgreSQL)
4. Implement email notifications
5. Add ATS integrations

## 📄 License

This is a demo project for startup pitch purposes.

## 📞 Support

For questions or investment inquiries, please contact the development team.

---

**Built with ❤️ for the future of recruitment**
