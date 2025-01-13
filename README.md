# Puppeteer Cookie Tracker

## Overview
This project is a Puppeteer-based tool to automate browser interactions and extract cookies from websites. It enables the analysis of cookies across different domains, providing insights into third-party cookies and shared cookie domains.

## Features
- Extracts cookies from websites programmatically using Puppeteer.
- Provides JSON data for third-party cookies and shared domains.
- Visualizes cookie origins using a D3.js-powered interactive graph.
- Includes scripts for advanced cookie analysis and visualization.

## File Structure
```
puppeteer-cookie-tracker/
│
├── analyze.js                      # Script for cookie extraction and analysis
├── analyze2.js                     # Additional cookie analysis script
├── package.json                    # Node.js project configuration
├── package-lock.json               # Lock file for dependencies
├── thirdPartyCookies.json          # JSON file listing extracted third-party cookies
├── sharedCookiesDomains.json       # JSON file listing shared cookie domains
├── cookieOriginsGraph.json         # Data source for visualization
├── trackCookies.js                 # Script for tracking and analyzing cookies
├── tracking.js                     # Utility script for tracking cookies dynamically
├── visualize.py                    # Python script for data visualization
├── web.html                        # Visualization page using D3.js
```

## Setup

### Clone the Repository
```bash
git clone https://github.com/edwjlr/puppeteer-cookie-tracker.git
cd puppeteer-cookie-tracker
```

### Install Dependencies
```bash
npm install
```

### Run Cookie Extraction Scripts
- To extract cookies from websites:
  ```bash
  node analyze.js
  ```
- For advanced analysis:
  ```bash
  node analyze2.js
  ```

### Run Visualization Interface
1. Open `web.html` in your browser to view the interactive graph visualization.
2. Ensure `cookieOriginsGraph.json` is in the same directory for proper data loading.

## Documentation
- **`thirdPartyCookies.json`**: Contains details about extracted third-party cookies.
- **`sharedCookiesDomains.json`**: Lists domains that share cookies.
- **`cookieOriginsGraph.json`**: Data source for visualization using `web.html`.

## Challenges
- Automating consistent cookie extraction across varying website architectures.
- Visualizing large datasets effectively using D3.js.

## Future Features
- Integrate tracking pixel detection and visualization.
- Add browser fingerprinting analysis.
- Include historical cookie tracking for trend analysis.

## License
This project is licensed under the MIT License. See [LICENSE](./LICENSE) for more details.
