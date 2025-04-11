# Data Analyst Portfolio

A clean, minimalist portfolio template designed specifically for data analysts. Showcase your skills, projects, and experience with beautiful data visualizations.

## Features

- 📊 Built-in data visualizations (bar chart, pie chart)
- 🎨 Modern, responsive design
- 🔧 Easy customization via JSON
- 🚀 Quick deployment to GitHub Pages
- 📱 Mobile-friendly layout

## Demo

[View Demo](https://holasoymalva.github.io/data-analyst-portfolio/)

## Getting Started

### Prerequisites

- Node.js (v14.0.0 or later)
- npm or yarn

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/holasoymalva/data-analyst-portfolio.git
   cd data-analyst-portfolio
   ```

2. Install dependencies:
   ```
   npm install
   ```
   or
   ```
   yarn install
   ```

3. Start the development server:
   ```
   npm start
   ```
   or
   ```
   yarn start
   ```

4. Open your browser and navigate to `http://localhost:3000`

## Customization

### Edit Your Information

All your personal information is stored in `public/data.json`. Edit this file to update your portfolio with your information:

```json
{
  "profile": {
    "name": "Your Name",
    "title": "Data Analyst",
    "bio": "Your short bio...",
    "email": "your.email@example.com",
    "github": "https://github.com/yourusername",
    "linkedin": "https://linkedin.com/in/yourusername",
    "resume": "link-to-your-resume.pdf"
  },
  "skills": [
    { "name": "SQL", "level": 90 },
    { "name": "Python", "level": 85 },
    ...
  ],
  ...
}
```

### Change Colors and Styling

The portfolio uses Tailwind CSS for styling. You can modify the colors and styles in the `src/App.js` file.

To change the main color scheme, update the gradient colors in the header section and the chart colors in the `COLORS` array.

## Deployment to GitHub Pages

1. Update the `homepage` field in `package.json`:
   ```json
   "homepage": "https://your-username.github.io/data-analyst-portfolio"
   ```

2. Install GitHub Pages package as a dev dependency:
   ```
   npm install --save-dev gh-pages
   ```
   or
   ```
   yarn add --dev gh-pages
   ```

3. Add deployment scripts to `package.json`:
   ```json
   "scripts": {
     "predeploy": "npm run build",
     "deploy": "gh-pages -d build",
     ...
   }
   ```

4. Deploy your site:
   ```
   npm run deploy
   ```
   or
   ```
   yarn deploy
   ```

5. Navigate to Settings > Pages in your GitHub repository and ensure the site is being built from the `gh-pages` branch.

## Project Structure

```
data-analyst-portfolio/
├── public/
│   ├── data.json         # Your personal data
│   ├── index.html
│   └── ...
├── src/
│   ├── App.js            # Main portfolio component
│   ├── index.js
│   └── ...
├── package.json
└── README.md
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [React](https://reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Recharts](https://recharts.org/)
- [Lucide React](https://lucide.dev/)
