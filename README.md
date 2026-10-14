# IdeaClient — Development

**DEV:** [linuxofpower/IdeaClient-Dev](https://github.com/linuxofpower/IdeaClient-Dev), branch `main`.

**Source / current production-side repository:** [yaMorozYaroslav/IdeaCliDev-relocate-](https://github.com/yaMorozYaroslav/IdeaCliDev-relocate-), branch `master`. This older repository name remains unchanged; any future production rename requires a separate approved action.

This is the **same application** in two stages. Implement and verify features in DEV. The production owner (`yaMorozYaroslav`) alone accepts/rejects pull requests and merges to production. Do not push directly to production or configure automatic production deployment from DEV. Development and production have separate Git histories.

**Migration:** source snapshot `50dc396a79d2e4e481673df9e38996fa07a69c62`; all 72 non-certificate tracked files match the original SHA-1 Git blobs exactly. Intentionally omitted local TLS files `certificates.backup/localhost-key.pem` and `certificates.backup/localhost.pem`. Do **not** restore them, or commit secrets or private keys.

**DEV CI:** [workflow](.github/workflows/ci.yml), runs on `main` pushes and pull requests. CI must never deploy production.

---

## Original application README

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
