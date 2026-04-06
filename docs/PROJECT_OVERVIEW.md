# Project Overview: Personal Resume/Portfolio with Agentic HR Chatbot

## Project Description

A production-ready single HTML page that serves as a resume and portfolio for software development career, enhanced with an embedded AI-powered HR agent that can answer recruiter questions about capabilities, strengths, weaknesses, interests, philosophy, and values.

---

## Architecture

### Frontend
- **Technology**: Pure HTML/CSS/JavaScript (single file)
- **Hosting**: GitHub Pages / Netlify / Render Static Site
- **Features**:
  - Resume/portfolio content
  - Embedded chatbot UI
  - Responsive design
  - Modern, professional styling

### Backend
- **Technology**: Node.js/Express
- **Hosting**: Render.com Web Service
- **Purpose**: Secure API proxy for OpenAI API
- **Endpoints**:
  - `POST /api/chat` - Handles chat requests with OpenAI

### AI Service
- **Provider**: OpenAI
- **Model**: GPT-4 or GPT-3.5-turbo
- **Knowledge Base**: JSON file containing personal/professional information
- **System Prompt**: Configured to act as an HR agent representing you

---

## Project Structure

```
khanin-ch/
├── docs/
│   ├── PROJECT_OVERVIEW.md          # This file
│   └── KNOWLEDGE_BASE_TEMPLATE.md   # Template for personal info
├── frontend/
│   └── index.html                   # Single page resume/portfolio with chatbot
├── backend/
│   ├── server.js                    # Express server for API proxy
│   ├── package.json                 # Node.js dependencies
│   ├── knowledge-base.json          # Your personal/professional data
│   └── .env.example                 # Environment variables template
└── README.md                        # Project documentation
```

---

## Technical Flow

1. **User visits HTML page** → Sees resume/portfolio content
2. **User opens chatbot** → Chat interface appears
3. **User sends message** → JavaScript sends POST to Render.com backend
4. **Backend receives request** → Loads knowledge base + constructs system prompt
5. **Backend calls OpenAI API** → Sends context + user message
6. **OpenAI responds** → Backend forwards response to frontend
7. **Frontend displays response** → User sees AI agent's answer

---

## Security Considerations

- ✅ OpenAI API key stored in Render.com environment variables (never exposed to client)
- ✅ CORS configured to only allow requests from your domain
- ✅ Rate limiting on backend to prevent abuse
- ✅ Input validation and sanitization
- ✅ HTTPS enforced on both frontend and backend

---

## Cost Estimate

### Hosting
- **Frontend**: Free (GitHub Pages/Netlify)
- **Backend**: Free tier on Render.com (750 hours/month)

### AI API Usage
- **GPT-3.5-turbo**: ~$0.002 per conversation
- **GPT-4**: ~$0.03 per conversation
- **Estimated monthly cost**: $5-20 depending on traffic

---

## Development Phases

### Phase 1: Setup & Documentation ✓
- [x] Define architecture
- [x] Create project structure
- [ ] Create knowledge base template

### Phase 2: Backend Development
- [ ] Set up Express server
- [ ] Implement OpenAI API integration
- [ ] Create knowledge base loader
- [ ] Configure system prompt
- [ ] Add error handling and logging
- [ ] Test API endpoints locally

### Phase 3: Frontend Development
- [ ] Design HTML structure
- [ ] Style with CSS (modern, responsive)
- [ ] Implement chatbot UI
- [ ] Add JavaScript for chat functionality
- [ ] Integrate with backend API
- [ ] Test responsiveness and UX

### Phase 4: Deployment
- [ ] Deploy backend to Render.com
- [ ] Configure environment variables
- [ ] Deploy frontend to hosting platform
- [ ] Update CORS settings
- [ ] End-to-end testing

### Phase 5: Refinement
- [ ] Performance optimization
- [ ] UI/UX improvements
- [ ] Add analytics (optional)
- [ ] SEO optimization

---

## Key Features

### Resume/Portfolio Section
- Professional summary
- Work experience
- Technical skills
- Projects showcase
- Education
- Contact information

### Agentic HR Chatbot
- Natural conversation flow
- Context-aware responses based on knowledge base
- Answers questions about:
  - Technical capabilities and expertise
  - Strengths and achievements
  - Areas for growth (weaknesses)
  - Personal interests and hobbies
  - Professional philosophy
  - Core values and work ethics
  - Career goals and aspirations
- Professional tone aligned with your personality

---

## Environment Variables

### Backend (.env)
```
OPENAI_API_KEY=sk-...
FRONTEND_URL=https://your-domain.com
PORT=3000
NODE_ENV=production
```

---

## Next Steps

1. Fill out `KNOWLEDGE_BASE_TEMPLATE.md` with your information
2. Develop backend API proxy
3. Create HTML resume/portfolio page
4. Integrate chatbot UI
5. Deploy to production
