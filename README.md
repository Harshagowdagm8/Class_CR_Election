# Class_CR_Election
Election System | Real-time voting app with secure Voter ID, candidate management, results dashboard &amp; data persistence. Features admin controls, vote tracking, live results, and full system reset options.
# 🗳️ CR Election System

A complete web-based voting system for Class Representative elections with real-time results, candidate management, and secure voting.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## ✨ Features

- **Voter Portal** – Cast votes using any unique Voter ID
- **Admin Dashboard** – Create elections, manage candidates, view results
- **Real-time Results** – Live vote counting with visual charts
- **Data Persistence** – All data saved locally in browser storage
- **Multiple Elections** – Create and manage multiple election cycles
- **Vote Tracking** – Track which voters voted for which candidate
- **Responsive Design** – Works on desktop, tablet, and mobile

## 🚀 Live Demo

Open `index.html` in any modern browser – no server required!

## 🔐 Admin Access

| Credential | Value |
|------------|-------|
| Username | `admin` |
| Password | `admin@123` |

## 📋 How It Works

### For Voters
1. Enter any unique Voter ID
2. Select your preferred candidate
3. Confirm your vote

### For Admins
1. Login with admin credentials
2. Create a new election (set start/end dates)
3. Add candidates (with optional images)
4. Share the election link
5. End election when ready
6. View detailed results with voter lists

## 🛠️ Features in Detail

### Election Management
- Create elections with custom titles and timeframes
- Auto-status (Upcoming / Active / Ended)
- Force end elections manually

### Candidate Management
- Add/delete candidates
- Upload candidate images (base64 stored)
- Track votes per candidate

### Voting System
- No pre-registration required – any ID works
- Prevents duplicate voting
- Records which voter voted for whom

### Results Dashboard
- Visual bar charts showing vote percentages
- Complete list of voters per candidate
- Winner announcement
- Historical election results

### System Reset Options
- Reset current election only
- Delete specific election
- Delete all elections
- Full system reset

## 📁 File Structure
cr-election-system/
├── index.html # Single file application
└── README.md # Documentation


## 💾 Data Storage

All data is stored in browser's `localStorage` under key `crElectionState`:

```javascript
{
  candidates: [],      // List of candidates with votes
  voters: {},          // Voter IDs per election
  elections: {},       // Election metadata
  currentElection: {}, // Active election
  voteRecords: {}      // Voter → Candidate mapping
}

Technologies Used
Technology	Purpose
HTML5	Structure
CSS3	Styling & Animations
JavaScript	Logic & Interactivity
Font Awesome	Icons
LocalStorage	Data persistence


###Responsive Breakpoints
Desktop: > 768px

Tablet/Phone: < 768px (optimized layout)
