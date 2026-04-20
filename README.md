# JWT Security Scanner

A polished, GitHub-ready JWT analysis project for web/API security workflows.

<img width="1569" height="882" alt="image" src="https://github.com/user-attachments/assets/4d89d8b2-60f9-4f50-9cb9-cfb2890ab50f" />
<br></br>
<img width="1456" height="886" alt="image" src="https://github.com/user-attachments/assets/094cbd26-419b-4400-ab28-8fd3c9893dfb" />

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

## License

MIT
