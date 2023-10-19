This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started
Setup database
```bash
docker pull mysql

docker run --name {{container_name}} -e MYSQL_ROOT_PASSWORD={{password}} -p {{port}}:3306 -v {{url_db: /Users/laptoptt/Documents/Knowledge/blog-fullstack/db}} -d mysql

npx prisma genarate

npx prisma migrate dev
```

env
```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY={{https://clerk.com/}}
CLERK_SECRET_KEY={{https://clerk.com/}}
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL="mysql://root:root@127.0.0.1:33061/discord?sslaccept=strict;trustServerCertificate=true"
UPLOADTHING_SECRET={{https://uploadthing.com/}}
UPLOADTHING_APP_ID={{https://uploadthing.com/}}

LIVEKIT_API_KEY={{https://docs.livekit.io/realtime/quickstarts/nextjs-13/}}
LIVEKIT_API_SECRET={{https://docs.livekit.io/realtime/quickstarts/nextjs-13/}}
NEXT_PUBLIC_LIVEKIT_URL={{https://docs.livekit.io/realtime/quickstarts/nextjs-13/}}
```

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
# discord-clone-full
