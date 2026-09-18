# Configurator.Build — Showcase Deploy

Live: GitHub Pages (do not attach configurator.build — that hostname is an unrelated AWS Next.js app).

## Repo
- Owner: yegwitty-max
- Name: configurator-build
- Public
- Branch: master

## Publish
```bash
cd /home/mre/Desktop/configurator-showcase
gh repo create yegwitty-max/configurator-build --public --source=. --remote=origin --push
gh api repos/yegwitty-max/configurator-build/pages -X POST -f 'source[branch]=master' -f 'source[path]=/'
```

Site: https://yegwitty-max.github.io/configurator-build/

## Files
- `/` variant picker
- `001-industrial-tactile/` ForgeFrame brand
- `002-editorial/` serif / white space
- `003-awwwards-grade/` dark immersive (featured, includes LGSF-OS coming soon)
