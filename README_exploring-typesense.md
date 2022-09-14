Part 1
https://www.youtube.com/watch?v=kwtHOkf7Jdg
Exploring Typesense, a lightning-fast, open source search engine

Part 2
https://www.youtube.com/watch?v=cIU19iA8I7U
Building a Search App in React.js using Typesense, Next.js & Tailwind CSS


First install Typesense
$ brew install typesense/tap/typesense-server@0.23.1

Run it
```
export TYPESENSE_API_KEY=xyz
mkdir /tmp/typesense-data
./typesense-server --data-dir=/tmp/typesense-data --api-key=$TYPESENSE_API_KEY --enable-cors
```
($ ./typesense-server --data-dir=data --api-key=xyz --enable-cors)

Check if okay
$ curl http://localhost:8108/health

doanload data set

Install 
$ pnpm dlx create-instantsearch-app exploring-typesense



Install project
$ pnpm dlx create-next-app --typescript typesense-with-nextjs

Install tailwind
$ pnpm add tailwindcss@latest postcss@latest autoprefixer@latest

Init tailwind
$ pnpm dlx tailwindcss init -p

Add Typesense
$ pnpm add typesense-instantsearch-adapter react-instantsearch-dom
(fix if error)
$ pnpm add @babel/runtime algoliasearch





This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://
github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
