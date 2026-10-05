> **Moved 2026-10-04 (import done; do not archive until source PR #3 is closed/merged).** Canonical copy lives in the kk-kb monorepo at [`content/projects/01-vancouver-ai-community/special-features/hackathons/rival-2024-2025/round-4-music/vanai-hackathon-004/`](https://github.com/WalksWithASwagger/kk-kb/tree/main/content/projects/01-vancouver-ai-community/special-features/hackathons/rival-2024-2025/round-4-music/vanai-hackathon-004) (source commit `3cd45ed7bf74`). Large media is in private Drive — see PROVENANCE.md there. This repo stays open for PR #3.

# Vancouver AI Hackathon Round 4: The Soundtrack of Us

## 🎵 What This Is
A dataset with **1,000+ survey responses** about how people discover music, what formats they use, and how they feel about AI-generated music. Perfect for creating data visualizations, apps, or insights about music and technology.

## 🚀 New to GitHub? Start Here

### Getting the Data (3 Easy Ways)

**Option 1: Download ZIP (Easiest)**
1. Click the green "Code" button at the top of this page
2. Click "Download ZIP"
3. Unzip the file on your computer
4. Open `data/raw/music_survey_data.csv` in Excel, Google Sheets, or any data tool

**Option 2: Clone with Git**
```bash
git clone https://github.com/WalksWithASwagger/vanai-hackathon-004.git
cd vanai-hackathon-004
```

**Option 3: Individual Files**
- Right-click any file → "Save As" to download individual files
- Main dataset: `data/raw/music_survey_data.csv`

## What's In The Dataset

### The Data
- **1,000+ complete responses** from music listeners across Canada
- **19 core questions** covering music discovery, format evolution, and AI attitudes
- **Rich demographics**: Age, location, education, income, household composition
- **3,000+ text responses** with sentiment analysis scores
- **Geographic distribution**: Ontario (40%+), BC (20%+), Alberta, Quebec, and more

### Question Categories
- **Music Discovery**: How people find new music (radio, streaming, social media, etc.)
- **Format Evolution**: Personal experiences with vinyl, cassettes, CDs, downloads, streaming
- **Listening Habits**: When and how people consume music in daily life
- **AI Music Attitudes**: Responses to AI-generated music and voice cloning
- **Social Sharing**: How people share music and their guilty pleasures
- **Personal Connection**: Life theme songs and meaningful lyrics

## 💡 Quick Start Ideas

### Just Want to Browse?
- Open `data/raw/music_survey_data.csv` in Excel or Google Sheets
- Check out `data/raw/survey_questions.txt` to see what was asked
- Run `python scripts/explore_data.py` for a quick data overview

### Ready to Code?

**Python Users**
```python
import pandas as pd

# Load the data
df = pd.read_csv('data/raw/music_survey_data.csv')
print(f"Total responses: {len(df)}")

# Check out some life theme songs
print(df['Q18_Life_theme_song'].dropna().head())
```

**R Users**
```r
library(tidyverse)
music_survey <- read_csv("data/raw/music_survey_data.csv")
glimpse(music_survey)
```

**Excel/Google Sheets Users**
Just open the CSV file - no coding required!

## Data Structure

### Key Columns
- `Q1_Relationship_with_music`: Music engagement level
- `Q2_Discovering_music`: Primary music discovery method
- `Q4_Music_format_changes`: Experience with format transitions
- `Q7_New_music_discover_*`: Multiple discovery methods
- `Q8_Music_listen_time_GRID_*`: Listening habits by activity
- `Q10_Songs_by_AI`: Attitudes toward AI-generated music
- `Q11_Use_of_dead_artists_voice_feelings`: AI voice cloning opinions
- `Q12_Music_bingo_*`: Music-related behaviors
- `Q13_Share_the_music_you_love_*`: Music sharing methods
- `Q15_Music_guilty_pleasure`: Musical guilty pleasures
- `Q18_Life_theme_song`: Personal theme songs
- `Q19_Lyric_that_stuck_with_you`: Meaningful lyrics

### Demographics
- `AgeGroup_Broad`: 18-34, 35-54, 55+
- `Province`: Geographic distribution
- `Education`: Education level
- `HH_Income_Fine_23`: Household income
- `Gender`: Gender distribution

### Sentiment Analysis
- Sentiment scores included for open-ended responses
- Polarity and subjectivity measures available
- Percentage scores for emotional content

## 📁 What's in This Repository

```
vanai-hackathon-004/
├── 📄 README.md                        # You are here!
├── 📊 data/
│   ├── raw/
│   │   ├── music_survey_data.csv      # 🎯 THE MAIN DATASET (start here!)
│   │   └── survey_questions.txt       # What questions were asked
│   ├── processed/                     # Your cleaned data goes here
│   └── analysis/                      # Your analysis results go here
├── 🔧 scripts/
│   ├── explore_data.py                # Quick data peek script
│   └── data_preprocessing.py          # Data cleaning helpers
├── 💻 src/                            # Your code goes here
├── 🎯 submissions/                    # Hackathon projects go here
└── 📚 docs/                          # Extra documentation
```

**The Important Files:**
- `data/raw/music_survey_data.csv` - This is your main dataset!
- `data/raw/survey_questions.txt` - Explains what each question means
- `scripts/explore_data.py` - Run this for a quick data overview

## 🔧 Helpful Scripts

### Want a Quick Data Overview?
```bash
python scripts/explore_data.py
```
This shows you basic info about the dataset - how many responses, what columns exist, sample data, etc.

### Need to Clean the Data?
```bash
python scripts/data_preprocessing.py
```
This helps clean up responses, handle missing data, and prepare data for analysis.

## Hackathon Challenge

Using this dataset, create an experience that's **interactive, visual, or narrative-driven**. The goal is to transform raw survey data into compelling insights about music, technology, and human behavior.

### Submission Requirements
- **Format Freedom**: Visual display, interactive demo, live performance, or unconventional approach
- **Bite-Sized Impact**: Engaging experience within 2-5 minutes
- **Technical Details**: Include all software, hardware, and instructions needed
- **Data Grounding**: Story must be grounded in the actual data
- **AI Integration**: Incorporate AI tools to enhance your narrative

### Judging Criteria
- **Creativity & Innovation (25%)**: Fresh, original approach
- **Clarity & Effectiveness (25%)**: Clear communication of insights
- **Engagement & Impact (20%)**: Compelling and memorable experience
- **Technical Execution (20%)**: Well-implemented solution
- **Community Value (10%)**: Open-source tools, shared methodologies

## 📅 Important Dates
- **Dataset Released**: September 15, 2025
- **Submission Deadline**: October 15, 2025
- **Award Date**: October 29, 2025

## 📦 Submission Requirements

**Your final folder of deliverables should include:**

- **PDF Document** containing:
  - Team member information (names, contact information)
  - Project title and description (max 300 words)
  - Brief explanation of your technical approach and tools used (max 300 words)
- **Link to working prototype/demo**, or the file itself
- **3-minute video walkthrough** (strongly encouraged, especially for interactive projects)

## 🛠️ Toolkit

Suggested tools, not requirements:

- **Cline, RooCode, Cursor, Claude Code** - AI copilots to jam with
- **v0 by Vercel, Lovable** - interfaces at speed
- **Udio, Suno, ElevenLabs** - sound experiments
- **Pika, Runway, Google Veo** - video riffs
- **p5.js, Processing, Observable** - data paintings
- **Seedream 4 (ByteDance), Midjourney, Stable Diffusion** - visual generation

## ❓ Need Help?

### New to Data Analysis?
- **Excel/Google Sheets**: Just open the CSV file and start exploring
- **Python**: Install pandas (`pip install pandas`) and use the code examples above
- **R**: Install tidyverse (`install.packages("tidyverse")`) and use the R code above

### New to GitHub?
- **Download**: Click green "Code" button → "Download ZIP"
- **Questions**: Check the Issues tab or create a new issue
- **Sharing**: Fork this repository to make your own copy

### Getting Stuck?
- Look at `data/raw/survey_questions.txt` to understand the questions
- Run `python scripts/explore_data.py` to see what's in the data
- Check the Issues tab for common questions

## 📋 License & Usage

This dataset is provided for hackathon use. Please respect participant privacy and use data responsibly.

---

**🎯 Ready to start?** Download the data and explore 1,000+ music stories from across Canada!
