A Python-based football analytics engine that transforms raw tracking data into tactical, physical, and spatial match insights.

Built using the SkillCorner Open Tracking Dataset, the project demonstrates how player and ball tracking coordinates can be converted into meaningful performance metrics used by analysts, coaches, and scouting departments.

# Project Overview

This project processes tracking data from an entire football match and automatically generates:

Match statistics
Physical performance metrics
Team tactical shape metrics
Space control analysis
Executive match dashboard
Automated match report

The engine is designed as a modular analytics pipeline, making it easy to extend with additional football analytics models.

# Features
📊 Match Statistics
Match Possession Analysis
Space Control Analysis
🏃 Physical Performance
Distance Covered
Sprint Detection
Sprint Leaderboard
Team Sprint Totals
Top Speed Analysis
Team Top Speed
Match Top Speed
🧠 Tactical Analytics
Team Width
Team Length
Convex Hull Area
Team Compactness
📈 Reporting
Match Dashboard
Automatic Match Report
# Project Structure
Football-Match-Analytics-Engine/
│
├── data/
│   ├── metadata.json
│   ├── tracking.jsonl
│
├── notebooks/
│   └── Match_Analytics_Engine.ipynb
│
├── modules/
│   ├── possession.py
│   ├── distance.py
│   ├── sprint_analysis.py
│   ├── top_speed.py
│   ├── team_shape.py
│   ├── space_control.py
│   ├── dashboard.py
│   └── report.py
│
├── images/
│
├── README.md
├── requirements.txt
└── LICENSE
# Technologies Used
Python
NumPy
Pandas
SciPy
Matplotlib
mplsoccer
# Analytics Modules
Module	Description
Match Possession	Calculates team possession percentages from tracking data
Distance Covered	Computes total distance covered by every player
Sprint Analysis	Detects sprint events using speed thresholds
Top Speed	Finds maximum speed for every player and team
Team Width	Measures horizontal team spread
Team Length	Measures vertical team spread
Convex Hull Area	Calculates the total area occupied by the team
Team Compactness	Measures how efficiently a team occupies space
Space Control	Estimates territorial dominance using player positions
Match Dashboard	Produces a consolidated match summary
Automatic Match Report	Generates a written tactical summary
# Example Dashboard
============================================================
# MATCH DASHBOARD
============================================================

Possession
Auckland FC                    57.45%
Newcastle Jets                 42.55%

Space Control
Auckland FC                    57.34%
Newcastle Jets                 42.66%

Distance Covered
Auckland FC                    97.29 km
Newcastle Jets                 97.80 km

Top Speed
J. Brimmer                     38.1 km/h

Team Width
37.27 m vs 36.28 m

Team Length
24.15 m vs 22.14 m

Convex Hull Area
595.3 m² vs 513.9 m²

Compactness
0.640 vs 0.634
# Example Match Insight

Auckland FC controlled the match with 57.45% possession and 57.34% space control, indicating superiority both on the ball and territorially. The team maintained a slightly wider (37.27 m) and longer (24.15 m) structure, resulting in a larger Convex Hull Area (595.3 m²). Despite this, both teams exhibited very similar compactness, suggesting comparable defensive organization. Physically, both sides covered approximately 97 km, highlighting an evenly matched work rate.

# Future Improvements
Tactical Analytics
Voronoi Diagrams
Pitch Control Model
Defensive Line Height
Team Centroid
Stretch Index
Passing Networks (requires event data)
Pressure Maps
Physical Analytics
High-Intensity Runs
Accelerations & Decelerations
Heat Maps
Fatigue Index
Ball Analytics
Ball Speed
Ball Progression
Ball Recovery Time
AI Features
AI Match Summary
Tactical Insights Generator
Team Style Classification
Match Comparison Engine
# Dataset

SkillCorner Open Tracking Dataset

Includes:

Match metadata
Player tracking coordinates
Ball tracking coordinates
Match timestamps
# Author

Stephen Yaw Ayamah

Data Analyst | Football Analytics | Python | Machine Learning | Sports Analytics

# About This Project

This project demonstrates how raw tracking coordinates can be transformed into actionable football intelligence. By combining physical metrics, tactical shape analysis, territorial control, and automated reporting, it showcases an end-to-end analytics workflow that mirrors the type of analysis used in modern professional football.
