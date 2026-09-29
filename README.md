# Antonio Gray Jr. — Portfolio

Single-page static site: plain HTML, CSS, and JS. No build step.

## Editing
- **Content:** everything is in `index.html`, one commented block per section.
- **Colors / spacing:** tokens at the top of `styles.css` (`--accent` is the one accent color).
- **Resume PDF:** edit `resume/resume.html`, then regenerate the PDF:

  ```powershell
  & "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --headless=new --no-pdf-header-footer --print-to-pdf="resume\Antonio_Gray_Jr_Resume.pdf" "file:///$((Resolve-Path resume\resume.html).Path.Replace('\','/'))"
  ```

## Preview locally
```bash
python -m http.server 4327
```
Then open http://localhost:4327.

## Deploy
GitHub Pages serves the `main` branch root. Push to `main` and the site updates in about a minute.

## Content rules
- The current Accenture client is never named: "a global social media platform (name withheld under NDA)".
- Contact: phone, email, LinkedIn, and GitHub (site and PDF).
