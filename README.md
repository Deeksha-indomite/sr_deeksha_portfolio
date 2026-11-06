
# S.R. Deeksha | Portfolio

An interactive, single-page portfolio for **S.R. Deeksha**, a second-year Robotics and AI student, AWS Student Builder Group Leader and open-source contributor. It covers projects, hackathons, certifications, LeetCode stats, events I have conducted, and a resume, with a few surprises hidden inside.

**Live site:** <paste your AWS Amplify URL here>

## Highlights

- **Superpower terminal:** open it from the green button under my intro and type `help`. Visitors can explore my work like a command line, and there are hidden commands to find.
- **Ask my assistant:** a built-in Q&A assistant that answers questions about me from a fact sheet. It runs entirely in the browser, with no external API and no keys.
- **Command menu:** press `Ctrl/Cmd + K` for quick navigation, and use the icon dock at the bottom of the screen.
- **Moving galleries:** certifications, anime, books and event photos scroll sideways on their own (they pause on touch or hover).
- **Resume viewer:** view my one-page resume and download it as a PDF.
- **Light and dark themes** with a manual toggle, and a responsive layout built for phones first.
- **Respects accessibility settings:** animations switch off when `prefers-reduced-motion` is on.

## Sections

Highlights, Events Conducted, Experience, Projects, Hackathons, Licenses and Certifications, DSA and Competitive Programming (LeetCode), Skills, Education, and Anime and Favourites.

## Tech stack

- Plain **HTML, CSS and JavaScript** in a single `index.html`, with no framework and no build step
- Inline SVG artwork for the cover and icons
- Web fonts from Google Fonts (Inter)
- Hosted on **AWS Amplify Hosting**

## Project structure

```
.
├── index.html     # the whole site
├── resume.pdf     # one-page resume
├── amplify.yml    # Amplify build settings (static site, nothing to build)
└── README.md
```

## Run locally

Open `index.html` in any modern browser. To serve it instead:

```bash
python3 -m http.server 4173
# then open http://127.0.0.1:4173/
```

## Deploy on AWS Amplify Hosting

1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/Deeksha-indomite/portfolio.git
   git push -u origin main
   ```
2. In the AWS Console, open **AWS Amplify** and choose **Create new app**.
3. Pick **GitHub**, authorise access, then select the repository and the `main` branch.
4. Keep the default build settings (`amplify.yml` is included) and choose **Save and deploy**.
5. When the build turns green, open the `https://main.<id>.amplifyapp.com` URL.

To deploy without Git, zip `index.html`, `resume.pdf` and `amplify.yml` and use **Deploy without Git provider** in Amplify.

## Contact

- Email: deekshastalwart07@gmail.com
- LinkedIn: [linkedin.com/in/deeksha-sr](https://www.linkedin.com/in/deeksha-sr)
- GitHub: [@Deeksha-indomite](https://github.com/Deeksha-indomite)
- LeetCode: [Deeksha_sr](https://leetcode.com/u/Deeksha_sr)
