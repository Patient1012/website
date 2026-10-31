# cgit Interface Recreation

This is a static recreation of the [cgit](https://git.zx2c4.com/cgit/) web interface, created without any Git functionality.

## What is this?
This project recreates the look and feel of cgit's standard web interface as a standalone static website. It includes mockups of:
- Repository listing page
- Repository summary page  
- Commit log view
- File tree view
- Commit details
- Diff view
- References view

## Running locally
Since this is a static website, you can run it with any HTTP server:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then open http://localhost:8000 in your browser.

## Attribution & License
This project is derived from [cgit](https://git.zx2c4.com/cgit/) which is licensed under GPL v2.
See ATTRIBUTION.md and COPYING.cgit for details. The CSS and JavaScript are based on cgit's original files.
