# Parks Project Guidelines

## Project Overview
Simple web app that tracks visited parks in San Francisco with ratings and comments.


## Build/Test Commands
- Run locally: Run `python -m http.server 8000` then open `localhost:8000` in browser
- Validate JSON: `jq < data/*.json`
- Mark visited: Add entry to `data/done.json` with rating and remarks

## Code Style
- HTML: Use 2-space indentation, semantic markup
- CSS: Follow BEM naming for new classes
- JavaScript:
  - Use ES6+ features (arrow functions, Promises, etc.)
  - Maintain clean async/Promise-based approach
  - Descriptive variable names (parkName vs name)
  - Keep UI updates separate from data fetching

## Project Structure
- `/data/maps/`: HTML files for each park
- `/data/done.json`: Visited parks with ratings (1-5) and remarks
- `/data/park_sizes.json`: Complete park list with sizes in acres
- `index.html`: Main application with UI and JS logic. All current and future logic is in here.
