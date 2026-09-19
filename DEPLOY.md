# Configurator.Build — Deploy

Gallery: PEMB, Post Frame (was Econo), LumberCladding, LGSF-OS coming soon.
WCBS Configurator and WCBS PostFrame are removed.

Do not bind configurator.build — that hostname is an unrelated AWS Next.js app.

## Live now (GitHub Pages)

https://yegwitty-max.github.io/configurator-build/
Repo: https://github.com/yegwitty-max/configurator-build

## Cloudflare Pages (created, first upload pending)

Project: configurator-build
Account: fa37875d2f3c2cc1347b7ae709cbd6e6 (Yegwitty)
Target: https://configurator-build.pages.dev/

This host times out on POST /pages/assets/upload (ETIMEDOUT). Project create succeeded.
From a clean network:

```bash
cd /home/mre/Desktop/configurator-showcase
rm -rf dist && mkdir dist
cp index.html dist/ && cp -r 001-industrial-tactile 002-editorial 003-awwwards-grade dist/
CLOUDFLARE_API_TOKEN=… wrangler pages deploy dist --project-name configurator-build --branch master
```

Or Cloudflare dashboard → Workers & Pages → configurator-build → Direct Upload.

Post Frame demo still at https://econo.vercel.app/design until that app is moved off Vercel.
