# 🗣️ CommentLens

**"Explore Public Perspectives. Analyze Feedback. Combat Online Toxicity."**  
*A web-first solution for understanding audience sentiment across YouTube and Reddit.*

---

## 📌 Submitted for: **Call2Code – 24-Hour Hackathon**  
### 🧩 Chosen Problem Statement: **PS 7 – Reality Check**

> **"Build an application that helps users explore different perspectives on the same topic or event using public APIs. Combine multiple data sources such as news, social platforms, or trend analytics to highlight contrasts, overlaps, or hidden insights."**

---

## 🚀 Solution Overview

**CommentLens** helps creators and businesses gain deep insights into audience sentiment by analyzing comments from **YouTube** and **Reddit** using public APIs. It filters noise, flags toxic language (including **Hindi** abuse), highlights trending topics, and even delivers **voice-based summaries** through automated calls.

The platform helps tackle online toxicity, information overload, and blind spots in audience perception—empowering safer, more responsive digital engagement.

---

## 🛠️ Tech Stack

| Layer           | Tools & Frameworks                                      |
|----------------|----------------------------------------------------------|
| Backend         | Python, Flask                                           |
| Frontend        | HTML, Bootstrap, CSS (Dark Themed UI)                   |
| NLP & ML        | Scikit-learn, NLTK, Sumy (LexRank), Custom Hindi Filter |
| Visualization   | Matplotlib                                              |
| Database        | SQLite + Flask-SQLAlchemy                               |
| Authentication  | Google OAuth (OAuth 2.0 / IDX)                          |
| Voice Call Agent| OmniDimension Voice API                                 |

---

## 🌐 Public API Integration

| API                             | Purpose                                                         | Rate Limit (Free Tier)                   |
|--------------------------------|------------------------------------------------------------------|------------------------------------------|
| YouTube Data API (v3)          | Fetches video metadata & up to 180,000 comments daily           | 10,000 units/day (~180k comments)        |
| Reddit API via AsyncPRAW       | Retrieves post content & user comments                          | 60–600 requests/min (depending on auth)  |
| Google OAuth API               | Authenticates users & links creators to their YouTube channels  | No hard limit, governed by user consent  |
| OmniDimension Voice API        | Sends automated voice call summaries of comment analysis        | 100–500 calls/day (based on plan)        |
| Sumy (LexRank)                 | Generates concise comment summaries                             | Local processing – No request limits     |

---

## 💡 Core Features

- Multi-platform input: YouTube URL or Reddit Post ID
- Sentiment classification: Positive, Negative, Neutral, Questions, Abusive
- 95% accurate **Hindi abusive content detection**
- Real-time topic and keyword extraction
- Smart summarization of comment threads (LexRank)
- Visual feedback dashboard with pie charts and bar graphs
- Direct deletion of toxic comments + reply to questions
- **Automated voice call** delivery of feedback summaries
- Fast processing: 1,000 comments in under 10 seconds
- Secure data storage using SQLite

---

## 🧠 Methodology

1. User inputs a YouTube link or Reddit Post ID
2. System fetches comments via public APIs
3. Text is preprocessed using NLTK (tokenization, stopword removal)
4. Sentiment and toxicity are classified using Scikit-learn models
5. Hindi abuse is flagged via a custom lexicon
6. LexRank (Sumy) generates summaries of top feedback
7. Visualizations are created using Matplotlib
8. Results are displayed via a Flask + Bootstrap frontend
9. Optional voice summary is delivered using OmniDimension API

---

Screenshots

![Screenshot 2025-02-20 184829](https://github.com/user-attachments/assets/c713c013-4b09-41ea-8031-51ef6edc8644)

![Screenshot 2025-02-20 184912](https://github.com/user-attachments/assets/b2e628ce-8f21-4c62-9e93-8a6c2656ce2e)

![Screenshot (84)](https://github.com/user-attachments/assets/477151be-2ca4-4038-a7fe-9f94fdcec70e)

![Screenshot (80)](https://github.com/user-attachments/assets/63506e17-9c7a-4382-a71c-f940cf33a005)

![Screenshot (81)](https://github.com/user-attachments/assets/f9759a62-0239-407a-adbf-cb37deb7dd82)

![Screenshot (82)](https://github.com/user-attachments/assets/92bfc518-d012-4e60-b4a9-66d6410843f2)


![Screenshot (83)](https://github.com/user-attachments/assets/a420e492-dc83-4548-9072-a9038c218720)



---

## 🌱 Future Scope

- Add support for Instagram, Twitter, and Facebook public comments
- Real-time monitoring & alerting for new toxic comments
- Dashboard analytics for brands (time-series sentiment tracking)
- Multilingual abusive comment detection with regional language support
- Integration with Google Trends and NewsAPI for cross-data correlation

---

## 👥 Team

- Tarun Goel  
- Shubh Singhal

---


