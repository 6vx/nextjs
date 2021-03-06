# deathMetta version Next.js

### don't forget to comment your code more often in this version :P

### todo
## Changes from Svelte version

1. **Backend must be serverless** instead of EC2 instances with CRON jobs that executed RCLONE commands and other POWERSHELL file copying/moving/renaming commands. 
2. **Build script should contain a data fetch** I'd prefer to have a larger serverside footprint than load these things from firebase/s3 when the page needs them. They should **BE** the page. Huge mistake in the way you built first version.

I don't think the way I'm doing this right now makes any sense it just kind of happened while in the midst of a flurry of learning about EC2/Powershell/Bash/Rclone/etc. The pieces just all made sense together for what I was trying to accomplish. However I think that there are better/easier/cheaper ways to accomplish the same jobs. 

The EC2 instances seem to occasionally crash when using the lowest tier machines, so I've been using a more expensive one. Changing this to a cloudwatch/lambda is probably first priority, and rclone might actually be best suited only to local machines.


## Objective

Gain familiarity with React. React is one of the most commonly used web frameworks and most jobs will be expecting some basic understanding of this material. 

By rewriting my project in this I can learn some of the ins and outs while I'm adjusting my app.

## Timeline

Expecting to spend less than a week on this, hopefully 20 hours. Most of the work necessary for a full rewrite of this idea is actually on the back end. Since my intent is to fully decouple front and back ends for my future projects, I think that swapping out front end framework builds will become a trivial expenditure of time as the goal is pursued.

## RIP Svelte

I enjoyed the simplicity of Svelte, and it helped clarify for me some of the patterns I need to keep track of in my head while making a project. It would be nice to continue using it; having simple one-file-components is delightful. I want to work someday, though. So. ttyl.

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/import?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
