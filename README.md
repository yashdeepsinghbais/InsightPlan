# InsightPlan 📊 - AI-Powered Student Performance Suggestions

**InsightPlan** is an intelligent backend API that uses Groq's LLaMA3 model to analyze student performance (in CSV format) and generate personalized, subject-wise study suggestions with improvement tips.

This is designed for use in personalized education tools such as student dashboards, teacher-assist platforms, or educational analytics software.

---

## 🚀 Features

- 📁 Accepts CSV student performance data (supports both numeric and rating-based formats).
- 🧠 Uses Groq’s LLaMA3 model to generate subject-wise study tips dynamically.
- 📋 Skips subjects with no valid data (no placeholder or empty sections).
- 📝 Returns well-formatted, markdown-style study tips with bold titles, emojis, and pro tips.
- 💪 Adds a final general improvement tips section for all students.
- ⚡️ Built with **Node.js** and **Next.js API routes** (`/pages/api/suggest.js`).

---

## 📂 Example Input (CSV)

| Name     | Math | Science | English | Social Studies | Computer | Hindi | Pass |
|----------|------|---------|---------|----------------|----------|-------|------|
| John     | 70   | Good    | 75      | Average        | 60       | 65    | Yes  |
| Priya    | 55   | Average | 71      | Good           | 58       | 66    | Yes  |
| Ayaan    | 60   | Bad     | 73      | Average        | Bad      | 64    | Yes  |

This will be parsed into a JSON array and sent to the API.

---

## 📦 API Usage

### 🔗 Endpoint


This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/pages/api-reference/create-next-app).

## Getting Started

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

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/pages/building-your-application/routing/api-routes) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/pages/building-your-application/routing/api-routes) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/pages/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn-pages-router) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/pages/building-your-application/deploying) for more details.
