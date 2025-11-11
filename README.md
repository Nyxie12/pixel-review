# Pixel 10 Executive Review Website

An interactive single-page website reviewing the Pixel 10 smartphone from an executive perspective, comparing it to the iPhone 15 Pro.

## Features

- **Interactive Dashboard**: Radar chart showing issue severity
- **Visual Comparisons**: Battery life bar chart, video quality comparisons
- **Organized Content**: Tabbed interface for software vs. hardware failures
- **Accordion Sections**: Expandable details for each failure point
- **Responsive Design**: Works on desktop, tablet, and mobile devices

## File Structure

```
PixelReview/
├── index.html          # Main HTML file
├── videos/            # Video files directory (create and add your videos here)
│   ├── Iphone.MOV     # iPhone video comparison
│   └── pxl.mp4        # Pixel 10 video comparison
└── README.md          # This file
```

## Video Files

The website references two video files:
- `videos/Iphone.MOV` - iPhone 15 Pro video sample
- `videos/pxl.mp4` - Pixel 10 video sample

**Note**: You'll need to add these video files to the `videos/` directory for the video comparison section to work properly.

## Running the Website

### Option 1: Simple HTTP Server (Python)
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then open: http://localhost:8000

### Option 2: Node.js HTTP Server
```bash
npx http-server -p 8000
```

### Option 3: VS Code Live Server
If using VS Code, install the "Live Server" extension and right-click `index.html` → "Open with Live Server"

### Option 4: Direct File Open
Simply double-click `index.html` to open in your browser (some features may be limited due to CORS restrictions)

## Technologies Used

- **HTML5**: Structure
- **Tailwind CSS**: Styling (via CDN)
- **Chart.js**: Data visualization (via CDN)
- **Vanilla JavaScript**: Interactivity

## Browser Support

Works on all modern browsers (Chrome, Firefox, Safari, Edge).

