# Caveat — product website

The rich Caveat homepage, design chooser, six example publications, component catalogue, comparison, and documentation. Extracted from the full application with its existing design and typography.

The homepage / displays “Start with a look. Make room for your words.” The same page is also available at /create. /why-caveat, /examples, /components, /compare, and /docs are included.

This repository is the public product website. It does not run an owner dashboard, store posts, or send email. The publication application and npm initializer remain separate.

## Local development

Use Node.js 22.12 or newer.

    npm ci
    npm run dev

## Deploy to Vercel

Import jonas-kgomo/caveat-home, choose the main branch, keep the root directory ./, and select the Next.js preset. The checked-in vercel.json uses npm ci and npm run build.

No database, auth secrets, or email account are required to deploy this website. Your existing publication deployment can remain a separate Vercel project.

Optional: set CAVEAT_TEMPLATE_REPOSITORY to the public HTTPS GitHub repository containing the application you want the “Deploy default Caveat” link to install. Its default is https://github.com/CaveatJS/site; this points to the published template, which may lag local application development. The destination application has its own database and authentication setup requirements.

## Checks

    npm run typecheck
    npm run build

Source application: https://github.com/CaveatJS/site
