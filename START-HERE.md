# Rally Scoreboard

## Purpose
Live pep rally scoreboard for Strake Jesuit house rallies. Displays real-time scores for all eight houses, pulling data from a public Google Sheet and rendering on a TV via Safari + AirPlay.

## Houses
Bellarmine, Campion, Claver, Faber, Gonzaga, Jogues, Regis, Xavier

## Current event: September 2026 House Game Day Rally
- Google Sheet tab: `2026_09_28`
- Single view: full leaderboard ranked 1-8 with pre-rally, rally, and total scores

## Data source
- Google Sheet ID: `13NeOVLRPSjXxUUIHdiwiKhcjPsggC_-3Y8VRi4AVMc0`
- Expected columns: Team, Pre-Rally, Rally
- Rows 2-9: one row per house
- Polls every 5 seconds via the Google Sheets CSV export URL
- Falls back to dummy data if the sheet is unreachable

## Technical details
- Self-contained single HTML file with all house crests and the school cross embedded as base64
- Hosted on GitHub Pages, displayed in Safari via AirPlay to TV

## Deployment
- GitHub Pages: https://jjmfhtx.github.io/rally-scoreboard/
- GitHub repo: https://github.com/jjmfhtx/rally-scoreboard

## Files
- `scoreboard.html` - the current application (HTML, CSS, JS, images all embedded)
- `index.html` - redirect to scoreboard.html for hosting platforms
- `archive/2026-04-spring-rally.html` - original Spring Rally version (3 views: leaderboard, winner cards, hold screen)
