# Suleman Awais - Portfolio (Static Version)

This is the static version of my portfolio website, designed to be deployed on GitHub Pages.

## Features

- 🎨 Modern, professional UI with smooth animations
- 📱 Fully responsive design
- ⚡ Dynamic experience calculation (updates automatically based on start date: Aug 2023)
- 💼 Work experience section with dynamic duration calculation
- 🚀 Projects showcase
- 🛠️ Skills display with proficiency bars
- 📬 Contact form (requires integration with a backend service)

## How to Deploy to GitHub Pages

1. Create a new GitHub repository
2. Push this folder to the repository
3. Go to Settings > Pages
4. Select the branch (usually `main`) and root folder
5. Save and your site will be live at `https://yourusername.github.io/repository-name/`

## Updating Content

All content is managed in the `<script>` section at the bottom of `index.html`:

### Update Experience Start Date
```javascript
const START_DATE = new Date('2023-08-01'); // Your start date
```

### Add Work Experience
```javascript
const EXPERIENCES = [
    {
        position: "Your Position",
        company: "Company Name",
        companyUrl: "https://company.com/",
        location: "Remote/Hybrid/On-site",
        startDate: new Date('2025-03-01'),
        endDate: null, // null for current position
        description: "Your job description...",
        technologies: ["Tech1", "Tech2", "Tech3"]
    }
];
```

### Add Projects
```javascript
const PROJECTS = [
    {
        title: "Project Name",
        description: "Project description...",
        technologies: ["Tech1", "Tech2"],
        liveUrl: "https://project-url.com/",
        githubUrl: "https://github.com/username/repo"
    }
];
```

### Update Skills
```javascript
const SKILLS = {
    "Category Name": [
        { name: "Skill Name", proficiency: 90 }
    ]
};
```

## Contact Form Integration

For the contact form to work, integrate with one of these services:

- **Formspree**: https://formspree.io/
- **EmailJS**: https://www.emailjs.com/
- **Netlify Forms**: https://www.netlify.com/products/forms/
- **getform.io**: https://getform.io/

## Local Development

Simply open `index.html` in your browser. No build process required!

## License

MIT License - Feel free to use this template for your own portfolio.
