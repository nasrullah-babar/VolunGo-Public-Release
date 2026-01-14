# VolunGo  
### Where Intent Meets Action in Real-Time  
**Google Maps Platform Award Submission | Devpost Project:** https://devpost.com/software/volungo-fz1jrv

VolunGo is a real-time, map-based platform designed to close the gap between NGOs in need and volunteers ready to help. Inspired by the efficiency of ride-sharing applications, VolunGo transforms community service into an immediate, engaging, and location-aware experience.

> **Note**  
> This repository serves as a **project showcase**. VolunGo does **not** currently have an open-source release.  
> The source code is not available at this time as it contains personal data and active API keys.



## Inspiration

The idea for VolunGo was born out of personal frustration during a university **Civics and Community Engagement** course. Finding volunteer opportunities was scattered and inefficient, relying on disconnected social media posts and unanswered calls.

Conversations with NGO executives revealed a mirrored issue: organizations frequently needed volunteers for urgent, time-sensitive tasks but lacked a way to broadcast these needs to nearby people in real time.

VolunGo was created as an **“Uber for volunteering”**, using location-based technology to close the gap between **intent** and **action**.



## Features

### For Volunteers

- **Community Impact Hub**  
  Live, interactive map displaying open volunteer opportunities using category-specific markers.

- **Mission Control**  
  Floating navigation bar for searching opportunities by location or filtering by category.

- **Navigation Mode**  
  Full navigation interface activated upon accepting a request, with:
  - Real-time route rendering  
  - Persistent panel showing estimated travel time

- **Gamified Rewards**  
  Dual-point system:
  - **Redeemable Points** for partner offers  
  - **Reputation Points (RP)** for permanent user leveling

- **Story of a Request**  
  Animated task-completion timeline featuring a **Before & After image slider**.



### For NGOs

- **Secure Dashboard**  
  Post volunteer requests with precise locations and assigned point values.

- **Volunteer Roll Call**  
  Attendance verification system to ensure accountability.

- **Task Management**  
  Mark tasks as completed, automatically triggering point distribution to verified volunteers.

- **Impact Documentation**  
  Upload **Before & After** images to visually showcase results.



## Technical Overview

VolunGo is my **first full-stack project**, developed specifically for the **Google Maps Platform Award**.



### Frontend

- **Framework:** React  
- **Styling:** Tailwind CSS (responsive design)  
- **Animations:** Framer Motion  
- **Mapping:** Google Maps Platform via `@react-google-maps/api`
  - Maps JavaScript API
  - Markers Service (custom & animated markers)
  - Places API Autocomplete (NGO location input)
  - Directions Service (real-time route visualization)
  - Geolocation API (user positioning)



### Backend

- **Environment:** Node.js & Express  
- **Database:** MongoDB Atlas with Mongoose (geospatial queries)  
- **Real-Time Layer:** Socket.IO (instant updates without refresh)  
- **Authentication:**  
  - Firebase Client SDK  
  - Firebase Admin SDK (backend token verification)
- **Storage:** ImgBB API for image uploads (via Axios)
