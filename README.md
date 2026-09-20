# PM Vishwakarma Portal

Static single-page site. No build step, no dependencies.

## Structure

```
.
├── public/
│   └── index.html    # the entire site (self-contained: HTML + CSS + JS)
├── vercel.json       # static deploy config
└── .vercelignore
```

## Local preview

```bash
python3 -m http.server 8000 --directory public
# http://localhost:8000
```

## Deploy

Vercel picks this up with zero configuration — `vercel.json` pins the framework
preset to "Other" and serves `public/` as-is.

```bash
npx vercel        # preview deployment
npx vercel --prod # production
```

Or import the repo at vercel.com; leave every build setting blank.
