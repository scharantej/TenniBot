## Flask Application Design for Tennis Scoring App

### HTML Files

- **`index.html`**: Main page for the app, allowing users to create a new match or view existing matches.

- **`match.html`**: Page for recording and displaying the details of a specific match, including the players' names, score, and points won by each player.

### Routes

- **`/`**: Home page, renders `index.html`.

- **`/create_match`**: Route to create a new match, accepts player names and redirects to `match.html`.

- **`/match/<match_id>`**: Route to access a specific match, renders `match.html` and passes the match details to the template.

- **`/record_point`**: Route to record a point won by a player, accepts the match ID, player name, and point type (e.g., serve, volley, etc.).

- **`/get_insights`**: Route to generate insights about the match from the recorded points, such as the number of points won by each player, the most common point types, and the overall winner.