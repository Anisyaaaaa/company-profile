# DigiSign Company Profile

DigiSign is a modern, responsive company profile website for a secure digital signature solution provider. This project showcases DigiSign's features, solutions, pricing, team, and more, using a clean and professional design powered by [Tailwind CSS](https://tailwindcss.com/) and [Font Awesome](https://fontawesome.com/).

## Features

- **Responsive Design:** Looks great on all devices.
- **Modern UI:** Built with Tailwind CSS for rapid, utility-first styling.
- **Feature Highlights:** Showcases security, speed, legal compliance, workflow automation, mobile support, and integrations.
- **Industry Solutions:** Tailored solutions for legal, real estate, healthcare, and financial services.
- **About & Team:** Company story, mission, timeline, and leadership profiles.
- **Testimonials:** Customer reviews and ratings.
- **Pricing Plans:** Simple, transparent pricing for Personal, Business, and Enterprise users.
- **Contact Form:** Users can send messages directly from the site.
- **FAQ Section:** Accordion-style frequently asked questions.
- **Footer:** Social links and company resources.

## Getting Started

### Local Development

1. **Clone or Download the Repository**

2. **Open `index.html` in your browser**

   No build steps or dependencies are required. All styles and icons are loaded via CDN.

### Docker Deployment

You can run this site using Docker and Nginx:

1. **Build the Docker image:**
   ```
   docker build -t digisign-company-profile .
   ```

2. **Run the Docker container:**
   ```
   docker run -p 8080:80 digisign-company-profile
   ```

3. **Open your browser and visit:**  
   [http://localhost:8080](http://localhost:8080)

## Customization

- **Branding:** Update the logo, company name, and images as needed.
- **Content:** Edit text, testimonials, pricing, and FAQ in `index.html`.
- **Styling:** Modify Tailwind classes or add custom CSS in the `<style>` block.

## Technologies Used

- [Tailwind CSS CDN](https://cdn.tailwindcss.com/)
- [Font Awesome CDN](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css)
- Google Fonts ([Poppins](https://fonts.google.com/specimen/Poppins))
- [Nginx Docker Image](https://hub.docker.com/_/nginx)

## Folder Structure

```
index.html
README.md
Dockerfile
```

## License

This project is for demonstration and educational purposes. Replace content and images as needed for your own use.

---

**Demo:**  
Open `index.html` in your browser or run with Docker to view the DigiSign company profile website.
