# Rally Scoreboard

## Purpose
Live pep rally scoreboard for the Strake Jesuit House Cup Spring Rally. Displays real-time scores for all eight houses, pulling data from a public Google Sheet and rendering on a TV via Safari + AirPlay.

## Houses
Bellarmine, Campion, Claver, Faber, Gonzaga, Jogues, Regis, Xavier

## Data source
- Google Sheet ID: `13NeOVLRPSjXxUIHdiwiKhcjPsggC_-3Y8VRi4AVMc0`
- Expected columns: Team, Pre-Rally, Rally
- Rows 2-9: one row per house
- Polls every 5 seconds via the Google Sheets CSV export URL

## Views
1. **Full leaderboard** - ranked 1-8 with pre-rally, rally, and total scores
2. **Winner cards** - House Cup Winner (by total) and Rally Champion (by rally score only)
3. **Hold screen** - header only, used between events

## Technical details
- Self-contained single HTML file with all house crests and the school cross embedded as base64
- Falls back to dummy data if the sheet is unreachable
- Hosted on GitHub Pages, displayed in Safari via AirPlay to TV

## Files
- `scoreboard.html` - the complete application (HTML, CSS, JS, images all embedded)
