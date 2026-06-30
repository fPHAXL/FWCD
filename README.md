# FWCD
My attempt in aggregating historical and current FIFA Tournament data and presenting it in clean, detailed, and interactive dashboard. I don't know what I am doing; help, guide, and work with me. 

Here's a slop README.md for you entertainment...


🌍 FIFA World Cup Dashboard - Interactive Map & Bracket
An immersive, real-time visualization of the 2026 FIFA World Cup featuring a live match timeline, interactive knockout bracket, and historical data exploration. Built with Leaflet.js, D3.js, and modern vanilla JavaScript.

Main dashboard showing the live timeline, bracket, and interactive map. 

✨ Features
📅 Live Match Timeline: Horizontal scrollable timeline with real-time score updates, match status (Live/HT/FT), and dynamic team flags.
🏆 Knockout Bracket: Dual-side bracket (Left/Right) displaying Round of 32 through Final. Click to pin brackets open for comparison.
🗺️ Interactive Map:
Historical Mode: Explore past World Cup data (1930–2022) with glowing D3 circles and host connection lines.
2026 Mode: View all 16 host stadiums with match schedules, capacities, and venue details.
Infinite Scroll: Seamless world repetition for both data points and stadium markers.
🎨 Fisheye Year Filter: Smooth, dynamic year selection with color-matched glow effects.
⚡ Real-Time Updates: Auto-refreshes every 60 seconds; calculates live match minutes based on kickoff time (ignoring API delays).
📱 Responsive UI: Auto-hiding side brackets, glassmorphism design, and mobile-friendly optimizations. 


                  Jumping in here, NOT ready yet, but you can see the screenshots of current progress in /Current.State                  ***********************************************************************************************************************************

🚀 Quick Start
Clone the repository:
git clone https://github.com/fPHAXL/FWCD/
cd FWCD

Open in Browser: Since this is a static single-page application, simply open allin.html in any modern browser.
# macOS
open allin.html

# Windows
start allin.html

# Linux
xdg-open allin.html

(Optional) Local Server: For best performance with external data fetching, run a local server:
# Using Python 3
python3 -m http.server 8000

# Using Node.js (npx)
npx http-server -p 8000

Then navigate to http://localhost:8000.
🛠️ Tech Stack
Map Engine: Leaflet.js (v1.9.4)
Data Visualization: D3.js (v7)
Data Sources:
Live Matches: GitHub Raw JSON (matches.json)
Venues: Local venues.js
Historical Data: Local data.js
Styling: Vanilla CSS with Glassmorphism (backdrop-filter)
Icons: FlagCDN for team flags


                  Jumping in here, NOT ready yet, but you can see the screenshots of current progress in /Current.State                  *************************************************************************************************************************************

📁 Project Structure
FWCD/
├──           # Main application (single-file)
├──            # 2026 Stadium data (lat, lon, capacity)
├──              # Historical World Cup participants (1930-2022)
├── /        # Add your screenshots here
│   ├── 
│   ├── 
│   └── 
├── LICENSE             # MIT License
└── README.md           # This file

🎮 Usage Guide
Timeline Controls
Scroll: Use mouse wheel or trackpad to scroll through matches. 
Click Card: Centers the timeline on a specific match.
Red Marker: Click the center red line to jump to the current live/recent match. 
Year Filter (Bottom Center)
Scroll: Hover over the year bar and scroll to change years.
Click: Click a specific year to filter the map to that World Cup.
Reset: Click the container background to show all years.
Bracket (Side Panels)
Auto-Hide: Brackets hide when idle to maximize map view. Move mouse to screen edges to reveal.
Pin: Click anywhere on a bracket to pin it open.  Click again to unpin.
View Both: Pin the left bracket, then hover the right edge to compare both sides.
Map Interactions
Hover Stadium: Shows popup with match schedule, capacity, and city.
Hover Historical Dot: Shows team name, result, and host nation(s) with glow effect.
Zoom/Pan: Standard map controls. Stadium markers repeat across world copies.
📸 Screenshots
(Add your screenshots to the screenshots/ folder and update the links below)

Main Dashboard	Bracket Pinned	Stadium Popup

🤝 Contributing
Contributions are welcome! Since this is a visualization project, feel free to:

Report Bugs: Found a match with incorrect data? Open an issue.
Suggest Features: Want penalty shootout stats on the timeline? Let me know.
Improve Design: CSS tweaks for better mobile responsiveness are appreciated. 

## 📄 License

This project is licensed under the **GNU General Public License v3.0 (GPLv3)**.

**Why GPLv3?**
- ✅ **Share-Alike (Copyleft)**: Any derivative works, modifications, or projects that incorporate this code **must also be open-sourced** under GPLv3.  This ensures improvements are shared back with the community.
- ✅ **Patent Protection**: Includes an explicit patent grant from contributors to users. 
- ✅ **Frontend Enforcement**: Since this code runs in the browser, it is considered "distributed" to the user, triggering the open-source requirement immediately. 
- ❌ **No Proprietary Forks**: Companies cannot take this code, modify it, and sell it as a closed-source product. 

See the [LICENSE](./LICENSE) file for the full legal text.   

🙏 Acknowledgments
Match data provided by the open-source FIFA World Cup community.
Flag icons courtesy of FlagCDN.
Map tiles by OpenStreetMap & CARTO.
Built with ⚽ and 🗺️ for the 2026 FIFA World Cup.
