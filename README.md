# Sports Event Recaps

A static website showcasing detailed game highlights and analysis from memorable sports events. Each event page features embedded video highlights with timestamps and comprehensive game summaries.

## 🏠 Landing Page

The main `index.html` file serves as the landing page, featuring:
- Modern, responsive design with gradient background
- Event cards with sport-specific badges
- Quick game summaries and final scores
- Direct links to individual event pages

## 📁 Project Structure

```
sports-synonpsis-demo/
├── index.html                 # Landing page
├── duke_unc_basketball.html   # Duke vs UNC basketball recap
├── nd_osu_football.html       # Notre Dame vs Ohio State football recap
├── dj_ua_lacrosse.html        # Dublin Jerome vs Upper Arlington lacrosse recap
└── README.md                  # This file
```

## 📝 Adding New Events

To add a new sports event recap:

1. **Create the HTML file** following the existing template structure:
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Game Highlights: [Event Title]</title>
       <style>
           /* Copy existing CSS from any event page */
       </style>
   </head>
   <body>
       <div class="email-container">
           <div class="game-summary">
               <div class="summary-header">Game Summary: [Event Title]</div>
               <div class="summary-field">
                   <span class="field-label">Winning Team:</span>
                   <span class="field-value">[Team Name]</span>
               </div>
               <!-- Add other summary fields -->
           </div>
           
           <div class="highlights-section">
               <div class="highlights-header">Top Highlights</div>
               <!-- Add highlight items with embedded videos -->
           </div>
       </div>
   </body>
   </html>
   ```

2. **Update the landing page** (`index.html`) by adding a new event card:
   ```html
   <div class="event-card" onclick="window.location.href='[filename].html'">
       <div class="event-image" style="background-image: url('[sport-image-url]');">
           <div class="sport-badge">[Sport Emoji] [Sport Name]</div>
       </div>
       <div class="event-content">
           <div class="event-title">[Team A vs. Team B]</div>
           <div class="event-teams">[Team A Nickname] vs. [Team B Nickname]</div>
           <div class="event-score">[Team A] [Score] - [Score] [Team B]</div>
           <div class="event-summary">
               [Brief game summary]
           </div>
           <a href="[filename].html" class="event-link">View Highlights</a>
       </div>
   </div>
   ```

## 🎨 Customization

The design can be easily customized by modifying the CSS in each HTML file:
- Change colors by updating the gradient values
- Modify card layouts by adjusting grid properties
- Update typography by changing font-family declarations
- Add new animations by extending the transition properties