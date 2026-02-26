# 🟣 UW Quiet Study Spots Map
**Benni Wang | University of Washington**
GEOG 458 – Participatory Mapping Project

---
## 🤖 AI Disclosure

This project was developed with assistance from AI tools (ChatGPT) for:

- Debugging backend and database integration
- Structuring SQL queries and Express routes
- Refining frontend JavaScript logic
- Improving README documentation clarity
- Formatting Markdown documentation

All architectural decisions, project concept development, implementation, testing, and final design choices were completed and verified by the author.

AI was used as a supportive development and learning tool, similar to documentation references or coding forums, while maintaining full responsibility for the final submitted work.

---

## 🌐 Web Map URL

**GitHub Pages (Frontend):**
https://benjaminwang123.github.io/participatory-mapping/

**Heroku API (Backend):**
https://lab5-3484e28b9e28.herokuapp.com/

---

## Project Overview

The **UW Quiet Study Spots Map** is a participatory mapping project designed for the University of Washington community.

This map allows students to:

- Share their favorite quiet study locations on or near campus
- View crowdsourced study spots submitted by other UW students
- Discover study-friendly environments based on noise level

The project aims to support academic success and student well-being by building a collaborative resource for finding productive study environments.

---

## Target Group

This project specifically targets:

**University of Washington students**

The language, design, and examples reference campus locations such as:

- Odegaard Undergraduate Library
- Suzzallo Library
- Allen Library
- Other UW study spaces

The overall map style is designed to reflect a clean, academic campus environment.

---

## Data Collected

When users click on the map, they can submit:

- **Study Spot Name** (e.g., “Suzzallo 3rd Floor”)
- **Noise Level** (quiet / medium / loud)
- **Contributor Name** (optional)
- **Email Address** (optional, not displayed publicly)
- **Comment** (outlets, Wi-Fi quality, best time of day)
- Automatically recorded latitude & longitude

All contributions are stored in a PostgreSQL database and dynamically visualized on the map.

---

## Visual Design

### Basemap
The project uses a MapTiler vector basemap for a clean and campus-friendly appearance.

### Dot Styling
Dots are symbolized according to noise level:

- 🟢 Green = Quiet
- 🟡 Yellow = Medium
- 🔴 Red = Loud

Dot size varies slightly to reinforce the noise category visually.

---

## 🗄️ Database Structure

Table: `"tblRecord"`

Fields include:

- `id` (serial primary key)
- `contributor` (text)
- `email` (text)
- `spot` (text)
- `noise` (text)
- `content` (text)
- `lat` (double precision)
- `lng` (double precision)
- `created_at` (timestamp)

---

## Technical Stack

**Frontend**
- HTML
- CSS
- JavaScript
- MapLibre GL JS

**Backend**
- Node.js
- Express
- PostgreSQL
- Heroku deployment

---

## 🚀 How to Contribute

1. Open the web map
2. Click anywhere on campus
3. Fill in the study spot information
4. Submit the form
5. Refresh the page to see your contribution

---

## Last Updated

Feb 25 2026

---