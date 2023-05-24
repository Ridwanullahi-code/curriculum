# Deployment to Render

In this **step-by-step** guide you’ll learn how to deploy your application to: [Render](https://www.render.com).

<img src="./images/render.png" alt="Render logo" />

Render is a unified cloud to build and run all your apps and websites with free TLS certificates, a global CDN, DDoS protection, private networks, and auto deploys from Git.

## Render deployment guide

> If you'd like to know how to deploy a service using a specific language or framework, we encourage to look at the [documentation](https://render.com/docs)!

You will deploy your application to Render in 5️⃣ steps:

1. Create a new account
2. Deploy codebase to Render
3. Add environmental variables
4. Start the deployment process
5. Visit your deployed application

To follow along you can make use of [this repository](https://github.com/NoerGitKat/rails-sample-project).

### Step 1️: Create a new account at Render

Let’s start by creating a new account using your personal GitHub account!

<img src="./images/signup-render.png" alt="Login Page" width="400"/>

1. Navigate to [Render](https://www.render.com)
2. Create a new account using [GitHub](https://github.com/)

### Step 2️: Deploy codebase to Render

Now that you’ve set up your Render account, it’s time to start deploying your projects!

<img src="./images/dashboard-render.png" alt="Dashboard"/>

3. Navigate to the [dashboard](https://dashboard.render.com/)
4. Choose **New Web Service**
5. Connect a GitHub repository

<img src="./images/connect-repo-render.png" alt="Connect Repository to Render"/>

6. Configure your deployment. Here you can specify your application’s **name**, **root directory**, **build** and **start commands**.

<img src="./images/configure-deployment-render.png" alt="Configure deployment"/>

### Step 3️: Add environmental variables

7. Navigate to the `Environment` tab
8. Add your key-value pairs over to the Render project dashboard
   - If you're using **Rails**, check out [this resource](https://render.com/docs/deploy-rails#deploy-manually) from the official docs
   - If you're using **React**, check out [this article](https://render.com/docs/deploy-create-react-app#environment-variables) from the official docs

<img src="./images/env-variables-render.png" alt="Environmental variables"/>

### Step 4️: Start the deployment process

9. Once you’ve added your environmental variables, you should **manually redeploy** your application.

<img src="./images/redeploy-render.png" alt="Redeploy Render"/>

While the application is being deployed, it’s useful to keep watch of the logs. If anything goes wrong you can find out why here!

_Hint: it often has to do with setting up the correct build commands in [Render](https://render.com) or your application’s configuration (i.e. `package.json` or `render-build.sh`) Check the [documentation](https://render.com/docs) or [StackOverflow](https://stackoverflow.com/search?q=Render.app&s=af496ed1-3ae6-4209-8230-d72d51749c5b) for more information._

### Step 5️: Visit your deployed application

After the deployment has succeeded you can find the URL in the header

<img src="./images/url-deployment-render.png" alt="Deployment URL"/>

10. Click on the URL and visit your freshly deployed application!

<img src="./images/deployed-app-render.png" alt="Deployed application"/>

It’s beautiful! 🎉

1. As a final step, you should update the **live demo link** in your project's README file.

### [optional] Step 6️: Do a victory dance because you did it!

And there we have it: your application is now live on Render!

<section style="display:flex; flex-direction:column; align-items: center;">
   <img src="./images/jumping-parrot.gif" alt="Jumping Parrot" width="300"/>
</div>

## FAQ

**What do I do when my app doesn’t deploy successfully?**
First of all, take a deep breath in and try to relax.

When a build fails, you can find out why in the **logs**. It will give you hints why something went wrong.

_Hint: it often has to do with setting up the correct build commands in [Render](https://render.com) or your application’s configuration (i.e. `package.json` or `render-build.sh`) Check the [documentation](https://render.com/docs) or [StackOverflow](https://stackoverflow.com/search?q=Render.app&s=af496ed1-3ae6-4209-8230-d72d51749c5b) for more information._

**Where can I find the URL of my deployed application?**

The moment your application is deployed, you can find the URL in the header of your deployed project.

<img src="./images/url-deployment-render.png" alt="Deployment URL"/>

**How do I do X in Render?**

You might want to play around with other features on the platform. The developers of Render have written excellent documentation about various use cases, which you can find it [here](https://render.com/docs).

**How does the free tier work in Render?**

([source](https://render.com/docs/free#free-web-services))

- You have access to **750 hours of running time per month**.
- Web Services on the free plan are automatically spun down after **15 minutes of inactivity**. (when inactive it **doesn't** affect your allotted free running time).
- It can take up to **30 seconds** for an inactive web service to become active again.
- PostgreSQL databases in Render are **automatically removed after 90 days**. You would have to create a new one and connect it to your application to keep it functional.

**Help! My PostgreSQL database on Render is going to be deleted. What now?**
Unfortunately, this is one of the limitations to the free plan of Render. We can only recommend to **create a new database** and **replace the environmental variable**.

Alternatively, we recommend [ElephantSQL](https://www.elephantsql.com/plans.html) ("Tiny Turtle" plan) as a permanent solution. _Keep in mind it can only store about 20 MB of data!_

**How do I reach out for help when I’m stuck?**

You have many bright and helpful peers at your disposal for any challenges you might have. Just drop a message in [#full-time-students **💬**](https://microverse-students.slack.com/archives/GA812K2TC) or [StackOverflow](https://stackoverflow.com/search?q=Render.app&s=af496ed1-3ae6-4209-8230-d72d51749c5b) and help will be on the way.

If you still don’t manage to solve your issue, you can reach out to us via the [Student Dashboard](https://dashboard.microverse.org/). Our Student Success team is always ready to help you out!
