# Organization Chart Maker

A web-based tool to visualize organization charts from CSV files. Upload a CSV with employee data and see an interactive org chart powered by D3.js.

## Features

- **CSV Upload** - Upload any CSV file with org data
- **Interactive Visualization** - Pan, zoom, and explore the org structure
- **Rich Node Info** - Display name + 3 additional columns on each node
- **Hover Details** - Hover over any node to see all additional columns (6-15) in a floating tooltip
- **Auto-load Sample** - Comes with sample data to get started immediately

## CSV Format

Your CSV must have at least these columns:

| Column | Description |
|--------|-------------|
| `name` | Employee's full name (required) |
| `mentor` | Manager's name - who this person reports to (leave empty for top-level) |

**Optional Columns (3-5):** Displayed on the node itself
- Column 3 (e.g., title, position)
- Column 4 (e.g., department)
- Column 5 (e.g., email, location)

**Optional Columns (6-15):** Shown on hover tooltip
- Any additional employee data (phone, start date, skills, etc.)

### Example CSV

```csv
name,mentor,title,department,email,location,phone
Sarah Chen,,CEO,Executive,sarah@company.com,New York,+1-555-0100
Mike Johnson,Sarah Chen,VP Engineering,Engineering,mike@company.com,San Francisco,+1-555-0101
Tom Brown,Mike Johnson,Engineering Manager,Engineering,tom@company.com,Austin,+1-555-0102
```

## Getting Started

1. Open `index.html` in a web browser
2. The sample org chart loads automatically
3. Upload your own CSV using the "Upload CSV" button

## Controls

- **Pan** - Click and drag to move around
- **Zoom** - Scroll to zoom in/out
- **Hover** - Hover over any node to see detailed info

## Tech Stack

- HTML5, CSS3, JavaScript
- [D3.js v7](https://d3js.org/) for visualization

## Browser Support

Works in modern browsers (Chrome, Firefox, Safari, Edge).

---

Open `index.html` to start visualizing your organization!