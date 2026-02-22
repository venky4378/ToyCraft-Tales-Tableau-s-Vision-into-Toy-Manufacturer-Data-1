# ToyCraft Tales - Tableau Dashboard with Flask

A professional Flask web application integrating Tableau dashboards with a modern, responsive UI for visualizing toy manufacturer data across the United States.

## Project Overview

**ToyCraft Tales** is a data visualization platform that showcases toy manufacturing insights through interactive Tableau dashboards embedded in a beautiful web interface. The application provides comprehensive analysis of toy manufacturers by state, annual trends, and market metrics.

### Features

- 🏠 **Home Page** - Attractive hero section with call-to-action
- 📖 **About Page** - Industry information with relevant imagery
- 📊 **Dashboard Page** - Embedded Tableau interactive visualizations
- 📈 **Story Page** - Data-driven narrative and insights
- 🎨 **Responsive Design** - Works seamlessly on all devices
- 🎯 **Professional UI** - Purple gradient theme with modern styling

## Technology Stack

- **Backend**: Python 3.11 with Flask 2.3.3
- **Frontend**: HTML5, CSS3, Jinja2 templating
- **Visualization**: Tableau Public (embedded)
- **Deployment**: Gunicorn, Procfile (Heroku-ready)

## Project Structure

```
tableau-project/
├── app.py                    # Flask application with routes
├── requirements.txt          # Python dependencies
├── Procfile                  # Heroku deployment configuration
├── README.md                 # This file
├── .gitignore                # Git ignore rules
├── package.json              # Project metadata
├── templates/                # HTML templates
│   ├── base.html            # Base template (navigation & footer)
│   ├── index.html           # Home page
│   ├── about.html           # About page
│   ├── dashboard.html       # Dashboard page
│   └── story.html           # Story page
└── static/                  # Static assets
    └── css/
        └── style.css        # Complete application styling
```

## Installation & Setup

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Git

### Local Development

1. **Clone the repository:**
```bash
git clone https://github.com/YOUR_USERNAME/tableau-project.git
cd tableau-project
```

2. **Create a virtual environment (recommended):**
```bash
python -m venv venv

# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Run the application:**
```bash
python app.py
```

5. **Access the application:**
Open your browser and visit: `http://localhost:5000`

## Usage

### Navigation

- **Home** - Introduction and overview
- **About** - Toy manufacturing industry information
- **Dashboard** - Interactive Tableau visualizations
- **Story** - Data narrative and key insights

### Tableau Integration

The dashboard page includes an embedded Tableau visualization. The current dashboard displays:

- Top 10 state toy manufacturers in the US
- Analysis of manufacturer count by year (2004-2016)
- Regional distribution metrics
- Industry performance indicators

**Tableau Dashboard Link:** 
https://public.tableau.com/views/toymanufacturerdashboard/Dashboard3?:language=en-GB&publish=yes

## Deployment

### Deploy to Heroku

1. Install Heroku CLI
2. Login to Heroku:
```bash
heroku login
```

3. Create a new app:
```bash
heroku create your-app-name
```

4. Deploy:
```bash
git push heroku main
```

5. View logs:
```bash
heroku logs --tail
```

### Deploy to Other Platforms

- **PythonAnywhere**: Upload files and configure web app settings
- **AWS**: Use Elastic Beanstalk with the provided Procfile
- **Azure**: Use App Service with Python runtime
- **DigitalOcean**: Deploy with Gunicorn and Nginx

## File Descriptions

| File | Purpose |
|------|---------|
| `app.py` | Main Flask application with 4 routes (Home, About, Dashboard, Story) |
| `requirements.txt` | Python dependencies (Flask, Werkzeug, Jinja2, Gunicorn) |
| `Procfile` | Configuration for Heroku deployment |
| `templates/base.html` | Base template with navigation bar and footer |
| `templates/index.html` | Home page with hero section |
| `templates/about.html` | About section with industry information |
| `templates/dashboard.html` | Tableau dashboard integration |
| `templates/story.html` | Data narrative page |
| `static/css/style.css` | Complete application styling |
| `.gitignore` | Files to exclude from Git |
| `README.md` | Project documentation |

## Development Notes

### Color Scheme

- Primary Gradient: Purple (#667eea) to Magenta (#764ba2)
- Accent Color: Coral Red (#ff6b6b)
- Dark Text: Navy (#1a365d)
- Light Text: White (#ffffff)

### Responsive Breakpoints

- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: < 768px

## Testing the Application

1. **Home Page**: Should display hero section with manufacturing facility image
2. **About Page**: Should display purple gradient background with toy manufacturing info
3. **Dashboard Page**: Should display Tableau visualization
4. **Story Page**: Should display data narrative with insights
5. **Navigation**: All links should work across pages
6. **Mobile**: Should be responsive on all screen sizes

## Troubleshooting

**Images not loading:**
- Check internet connection (external URLs are used)
- Clear browser cache (Ctrl+F5)

**Tableau dashboard not displaying:**
- Verify internet connection
- Check that Tableau Public is accessible
- Ensure embedding is enabled on Tableau dashboard

**Port 5000 already in use:**
```bash
# Windows
netstat -ano | findstr :5000

# macOS/Linux
lsof -i :5000
```

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Optimization

- CSS minification ready
- Image optimization via Pexels
- Efficient Tableau embedding
- Fast page load times

## Security Considerations

- HTTPS recommended for production
- Environment variables for sensitive data
- CORS configuration if needed
- SQL injection prevention (no database used)

## Future Enhancements

- Database integration for dynamic data
- User authentication
- Additional Tableau dashboards
- Data export functionality
- Advanced analytics

## License

MIT License - Feel free to use for educational and commercial purposes.

## Support & Questions

For issues or questions, please contact your instructor or create an issue in the repository.

## Project Submission Details

**Created**: February 2026
**Technology**: Flask, Python, Tableau, HTML5, CSS3
**Deployment**: Heroku-ready
**Status**: Production-ready

---

**Note for Lecturer**: This project is fully functional and ready for testing. All dependencies are listed in `requirements.txt`. Simply follow the installation steps above to run locally or deploy to a hosting platform.
