# JWT Security Scanner

A polished, GitHub-ready JWT analysis project for web/API security workflows.

## What this project does

This project provides a **safe, client-side JWT inspection interface** that helps analysts and developers:
- Decode JWT header and payload locally in the browser
- Flag risky algorithms such as `alg: none`
- Highlight JOSE header abuse indicators like `jku`, `jwk`, `kid`, `x5u`, and `x5c`
- Review claim hygiene issues such as missing `exp`, `iss`, or `aud`
- Generate a copyable JSON report for notes, triage, and documentation

## Important scope note

This version is intentionally defensive and GitHub Pages-friendly.
It **does not** brute-force secrets, exploit targets, probe live endpoints, or attack third-party systems.

## Files

- `jwt-security-scanner.html` — main application
- `README.md` — project documentation
- `LICENSE` — MIT license
- `.gitignore` — standard ignore rules

## Run locally

Because this is a static project, you can open the HTML file directly in your browser.
For a cleaner development workflow, you can also serve it locally:

```bash
python3 -m http.server 8080
```

Then visit:

```text
http://localhost:8080/jwt-security-scanner.html
```

## GitHub upload steps

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/jwt-security-scanner.git
git push -u origin main
```

## GitHub Pages

1. Push the repository to GitHub
2. Open **Settings -> Pages**
3. Set source to the `main` branch
4. Select the root folder
5. Save and wait for deployment

Your live demo URL will look like:

```text
https://YOUR-USERNAME.github.io/jwt-security-scanner/
```

## Suggested next upgrades

- Add a backend API for optional JWKS validation
- Add framework fingerprints for insecure JWT handling
- Add Markdown/PDF export
- Add a lab-only active testing mode with hard scope controls
- Add CI checks for insecure JWT code usage in repos

## Security references that shaped the detection ideas

- PortSwigger Web Security Academy JWT guidance
- JWT algorithm confusion research
- Common JWT verification pitfalls documented by established security tooling and vendor guidance

## License

MIT
