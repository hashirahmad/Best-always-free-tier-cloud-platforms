# Best 'always' free tier cloud platforms

- [Best 'always' free tier cloud platforms](#best-always-free-tier-cloud-platforms)
  - [A word of caution](#a-word-of-caution)
  - [What are my (_maybe yours too_) needs and wants?](#what-are-my-maybe-yours-too-needs-and-wants)
  - [Eliminating useless choices](#eliminating-useless-choices)
    - [Heroku](#heroku)
    - [AWS](#aws)
    - [Azure](#azure)
    - [Google Cloud](#google-cloud)
    - [Oracle Cloud](#oracle-cloud)
  - [Finding more choices](#finding-more-choices)
    - [IBM Cloud](#ibm-cloud)
    - [Cloudflare workers](#cloudflare-workers)
    - [Fly.io](#flyio)
    - [Other odd choices](#other-odd-choices)
      - [Netlify](#netlify)
      - [Vercel](#vercel)
  - [Ideal choice](#ideal-choice)
    - [Fly.io](#flyio-1)
    - [Cloudflare workers (_in future_)](#cloudflare-workers-in-future)
  - [Links for *further reading*](#links-for-further-reading)
    - [Fly.io](#flyio-2)
    - [Cloudflare Workers](#cloudflare-workers-1)
    - [IBM Cloud](#ibm-cloud-1)
    - [Heroku](#heroku-1)
    - [Serverless](#serverless)
    - [Comparisons between cloud providers](#comparisons-between-cloud-providers)
    - [Google cloud](#google-cloud-1)
    - [AWS](#aws-1)
    - [Oracle cloud](#oracle-cloud-1)
    - [Alibaba Cloud](#alibaba-cloud)
    - [Azure](#azure-1)
    - [Misc. Useful links](#misc-useful-links)

**From** developer; **for** developer(s).

This consists of all the reading I did to find **'always' free** cloud platforms **most suitable** for side projects so you and I do not have to pay when unnecessary. The purpose is **not** to *list* relevant **'always' free** services but make the reader aware of **who** is providing them and **where** to read for further information.

## A word of caution

- ***EVERYTHING*** mentioned here is **from my reading** (*links at the bottom*)
- Obviously this is all **an opinion** ~ *not some professional advice*

## What are my (_maybe yours too_) needs and wants?

- Suitable for Node.js Express
- No debit card required (*unless necessary*)
- Be as **vendor free** as possible so migration is relatively straight forward
- As little **Dev Ops** as necessary i.e. *managed Dev Ops*
- Scalable (inc. price) so upgrading to paid services is not crazy 🚀
- Has 'usable enough' domain name i.e. **`myApp`**`.company.app` and not ~~**`myApp1234.sd27s3de.eu-west1`**`.company.app`~~ (_yikes_)

## Eliminating useless choices

### Heroku

- It's perfect.
- Exactly the sort of product I am after.
- Best thing: generous free tier and paid plans not so generous
- Just one issue: Pricing 🚀 when upgrading to paid plans
- Platform as as Service (PaaS)
- [Heroku 'always' free services](https://www.heroku.com/free)

### AWS

- AWS has pretty generous free tier. Unfortunately capped at 12 months.
- Always free services are mostly utilities i.e. not good on their own.
- DynamoDB **always free** `25GB` is exceptional yet it is **vendor locked**
- Lastly it requires debit card
- More of Infrastructure as a Service (IaaS)
- [AWS 'always' free services](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=tier%23always-free&awsf.Free%20Tier%20Categories=*all)

### Azure

- I really want to avoid Microsoft services.
- Just do not like them.

### Google Cloud

- Google's Cloud functions, App engine and Cloud run are generous.
- Yes there is Google's free `f1-micro`. Still its a VM to manage.
- Google cloud is **expensive** in terms of upgrading and is most expensive in relation of AWS and others.
- Lastly it requires debit card
- Mixed services including PaaS and IaaS
- [Google Cloud 'always' free services](https://cloud.google.com/free/docs/gcp-free-tier?hl=fi#free-tier)

### Oracle Cloud

- **Extremely generous** 'always' free tier like 2 VM machine `1GB` RAM each
- It has only **2% market share** ~ this means less people so less answers on `Stackoverflow` and less support
- It is behind competition at least in terms of the big players
- Lastly it requires debit card
- [Oracle Cloud 'always' free services](https://www.oracle.com/uk/cloud/free/#always-free)

## Finding more choices

Heroku is the only **reasonable** option at this point. All other services conflict with the **needs and wants**.

### IBM Cloud

- No debit card required
- **Generous** 'always' free services ~ about **`40`+** of 'always' free services
- [IBM Cloud 'always' free services](https://www.ibm.com/cloud/free) ~ (_you will need to click **always free** tab_)

### Cloudflare workers

- Extremely generous 'always' free tier
- Extremely affordable paid services (_something which Heroku lacks_)
- Free tier has **`10`ms** CPU limit (_sounds trivial yet its decent amount and does not include the time where `app` is waiting for other APIs_)
- No support for Mongodb at the moment (_the only negative! although they are planning on it_)
- No debit card required
- [CloudFlare Workers 'always' free services](https://developers.cloudflare.com/workers/platform/limits#worker-limits)
- [CloudFlare Workers 'always' free request limits](https://developers.cloudflare.com/workers/platform/limits#request-limits)
- [CloudFlare Workers 'always' free account plan limits](https://developers.cloudflare.com/workers/platform/limits#account-plan-limits)

### Fly.io

- `3` shared-cpu-1x VMs with 256MB RAM full time.
- `160GB` bandwidth per month (_Google cloud and others cap this usually and no where as generous_)
- 10 active certificates (_in Heroku this is paid service_)
- Super easy to deploy like Heroku CLI
- [Fly.io 'always' free services](https://fly.io/docs/about/pricing/#free-tier)

### Other odd choices

These are odd services because they have **generous** 'always' free tier. They are intended for website hosting so their free tier (_which to our interest_) really is mostly cloud functions. These are useful for hosting your web app after your have build your API or depending on needs, it may be more appropriate to skip the API all together and just use provided serverless functions for any backend functionality.

#### Netlify

- `125k` serverless functions every month with no expiry date
- 100GB /month bandwidth
- [Netlify 'always' free services](https://www.netlify.com/pricing/) ~ (_you will need to scroll down to see free plans_)

#### Vercel

- Up to 100 GB-Hrs on cloud functions every month with no expiry date
- Serverless function timeout limit to `5` seconds (_in some cases not enough_)
- 100GB /month bandwidth
- [Vercel 'always' free services](https://vercel.com/pricing) ~ (_you will need to scroll down to see free plans_)
- [Vercel 'always' free general limits](https://vercel.com/docs/platform/limits#general-limits)

## Ideal choice

### Fly.io

- Is like Heroku. Just a lot more affordable
- For example (_for surface level comparison_):
  - `1GB` shared cpu is **$0.0000022/s ($5.70/mo)** (_In Heroku, `1GB` it is **$50 per month**_)
  - 1 dedicated 2GB is **$0.0000120/s ($31.00/mo)** (_In Heroku, `2GB` it is **$100 per month**_)

### Cloudflare workers (_in future_)

- Super fast and it is **100,000 requests per day** (_yes, per day!_)
- Once it supports **Mongodb** and possibly the ability to run **Node.js express.js** although `express.js` can be done by other means too

## Links for *further reading*

I have **listed** pretty much all the articles I read. So just pick whichever suitable or feel useful to your needs. *Listed in the order of first reading*

### Fly.io

- [Fly App Pricing · Fly](https://fly.io/docs/about/pricing/)
- [Build, Deploy and Run a Node Application · Fly](https://fly.io/docs/getting-started/node/)

### Cloudflare Workers

- [Limits · Cloudflare Workers docs](https://developers.cloudflare.com/workers/platform/limits)
- [Known issues · Cloudflare Workers docs](https://developers.cloudflare.com/workers/platform/known-issues)
- [Pricing · Cloudflare Workers docs](https://developers.cloudflare.com/workers/platform/pricing)
- [Environment variables · Cloudflare Workers docs](https://developers.cloudflare.com/workers/platform/environment-variables)
- [Cloudflare Workers Introduction - DEV Community](https://dev.to/fllstck/cloudflare-workers-introduction-14mo)
- [My misadventure with Cloudflare Workers and Vue Serverless Side Rendering - DEV Community](https://dev.to/divporter/my-misadventure-with-cloudflare-workers-and-vue-serverless-side-rendering-22f7)
- [Deploy your first Serverless function in 5 minutes with Cloudflare Workers - DEV Community](https://dev.to/harrisgeo88/deploy-your-first-serverless-function-in-5-minutes-with-cloudflare-workers-29mm)
- [What is CPU time and Wall time in the context of Cloudflare Worker request? - Stack Overflow](https://stackoverflow.com/questions/68720436/what-is-cpu-time-and-wall-time-in-the-context-of-cloudflare-worker-request)
- [Cloudflare Worker times out for the client, but all the work completes and no timeout error given (inspected with console.log/ `wrangler tail`) - Stack Overflow](https://stackoverflow.com/questions/67756143/cloudflare-worker-times-out-for-the-client-but-all-the-work-completes-and-no-ti)
- [webpack 2 - How do I query in MongoDB with Cloudflare workers? - Stack Overflow](https://stackoverflow.com/questions/58249069/how-do-i-query-in-mongodb-with-cloudflare-workers)
- [Hi, I'm the tech lead of Workers. Note that the core point here is multi-tenancy... | Hacker News](https://news.ycombinator.com/item?id=18418120)
- [Workers KV - free to try, with increased limits!](https://blog.cloudflare.com/workers-kv-free-tier/)
- [Cloudflare Workers KV vs. MongoDB Comparison](https://db-engines.com/en/system/Cloudflare+Workers+KV%3BMongoDB)
- [Cloudflare Workers KV vs. CockroachDB vs. MongoDB Comparison](https://db-engines.com/en/system/Cloudflare+Workers+KV%3BCockroachDB%3BMongoDB)
- [How to locally run my cloudflare worker serverless function, during development? - Stack Overflow](https://stackoverflow.com/questions/53901880/how-to-locally-run-my-cloudflare-worker-serverless-function-during-development)
- [Cloudflare Workers + MongoDB : CloudFlare](https://www.reddit.com/r/CloudFlare/comments/p3iv5s/cloudflare_workers_mongodb/)
- [Cloudflare Workers KV Introduction - DEV Community](https://dev.to/fllstck/cloudflare-workers-kv-introduction-1oo)
- [cloudworker-router - npm](https://www.npmjs.com/package/cloudworker-router)
- [Node.js support in Cloudflare Workers](https://blog.cloudflare.com/node-js-support-cloudflare-workers/)
- [Delivering APIs at the edge with Cloudflare Workers - DEV Community](https://dev.to/peasey/delivering-apis-at-the-edge-with-cloudflare-workers-225i)
- [Introducing Sunder: A framework for Cloudflare Workers - DEV Community](https://dev.to/gzuidhof/introducing-sunder-a-framework-for-cloudflare-workers-1hdg)
- [cloudflare/worker-examples: Examples of Javascript you can run on Cloudflare’s worldwide network](https://github.com/cloudflare/worker-examples)
- [gzuidhof/sunder-worker-template: Template for Sunder in Cloudflare worker with Typescript, ESBuild and Jest](https://github.com/gzuidhof/sunder-worker-template)
- [Why use serverless computing? | Pros and cons of serverless | Cloudflare](https://www.cloudflare.com/en-gb/learning/serverless/why-use-serverless/)
- [Getting started with Fauna and Cloudflare Workers](https://fauna.com/blog/getting-started-with-fauna-and-cloudflare-workers)
- [Going Serverless with Cloudflare Workers - DEV Community](https://dev.to/semaphore/going-serverless-with-cloudflare-workers-452k)

### IBM Cloud

- [Why use serverless computing? | Pros and cons of serverless | Cloudflare](https://www.cloudflare.com/en-gb/learning/serverless/why-use-serverless/)
- [Getting started with Fauna and Cloudflare Workers](https://fauna.com/blog/getting-started-with-fauna-and-cloudflare-workers)
- [Going Serverless with Cloudflare Workers - DEV Community](https://dev.to/semaphore/going-serverless-with-cloudflare-workers-452k)
- [IBM Cloud Functions - Pricing](https://cloud.ibm.com/functions/learn/pricing)
- [IBM Cloud Private on Amazon Web Services - IBM Cloud Architecture Center](https://www.ibm.com/cloud/architecture/architectures/ibm-cloud-private-aws/)
- [Build a cloud-ready Express.js application on IBM Cloud – IBM Developer](https://developer.ibm.com/tutorials/deploy-cloud-native-expressjs-app-to-a-hosted-kubernetes-cluster/)
- [IBM/nodejs-express-app: Start building your next Node.js Express app on IBM Cloud.](https://github.com/IBM/nodejs-express-app)
- [IBM-Cloud/get-started-node: Sample and tutorial to help you get started with Express, REST API and a database.](https://github.com/IBM-Cloud/get-started-node)
- [Deploying your Node.js Application on IBM Cloud – SIA Innovations](https://www.siainnovations.com/blog/deploying-your-node-js-application-on-ibm-cloud/)
- [Adding extra npm modules to IBM Cloud Functions with Docker | by Glynn Bird | Weekly Webtips | Medium](https://medium.com/weekly-webtips/adding-extra-npm-modules-to-ibm-cloud-functions-with-docker-fabacd5d52f1)
- [Deploy a NodeJS app to IBM Cloud Container Registry - DEV Community](https://dev.to/ibmdeveloper/deploy-a-nodejs-app-to-ibm-cloud-container-registry-46m2)
- [deployment - How to deploy a docker image from docker hub to ibm cloud free tier - Stack Overflow](https://stackoverflow.com/questions/64020892/how-to-deploy-a-docker-image-from-docker-hub-to-ibm-cloud-free-tier)
- [Deploy a microservices app on IBM Cloud by using Kubernetes - IBM Cloud Architecture Center](https://www.ibm.com/cloud/architecture/tutorials/microservices-app-on-kubernetes/)

### Heroku

- [Deploying Node.js Apps on Heroku | Heroku Dev Center](https://devcenter.heroku.com/articles/deploying-nodejs)
- [Best Practices for Node.js Development | Heroku Dev Center](https://devcenter.heroku.com/articles/node-best-practices#hook-things-up)
- [Why We Moved from Heroku to Google Kubernetes Engine | Rainforest QA](https://www.rainforestqa.com/blog/2019-04-02-why-we-moved-from-heroku-to-google-kubernetes-engine)
- [Does upgrading Heroku from standard 1x dyno to standard 2x dyno actually improve performance for Node.js apps? - Stack Overflow](https://stackoverflow.com/questions/67028131/does-upgrading-heroku-from-standard-1x-dyno-to-standard-2x-dyno-actually-improve)
- [ruby - Why are my basic Heroku apps taking two seconds to load? - Stack Overflow](https://stackoverflow.com/questions/2606190/why-are-my-basic-heroku-apps-taking-two-seconds-to-load)
- [Heroku Pricing Explained | Low-code backend to build modern apps](https://blog.back4app.com/heroku-pricing/)
- [Top 10 Alternatives to Heroku | Low-code backend to build modern apps](https://blog.back4app.com/top-10-heroku-alternatives/)
- [Heroku Alternatives and Free Competitors | Buddy: The DevOps Automation Platform](https://buddy.works/actions/heroku/alternatives)
- [Heroku Alternatives — Top 5 Picks | by Brenda Clark | Medium](https://medium.com/@brenda.clark/heroku-alternatives-top-5-picks-9095cef91d91)
- [Heroku alternative for web app hosting and development | Platform.sh](https://platform.sh/alternative-to-heroku/)
- [Top Heroku Competitors and Alternatives - Gartner 2021](https://www.gartner.com/reviews/market/application-platforms-reviews/vendor/salesforce/product/heroku/alternatives)

### Serverless

- [Firebase Pricing](https://firebase.google.com/pricing)
- [Deploy a Node.js Application With the App Engine in 10 Minutes! | by Andrew Didinchuk | Towards Data Science](https://towardsdatascience.com/deploy-a-node-js-application-with-app-engine-in-10-minutes-69b03e4d54f0?gi=269cd3490680)
- [Serverless Cost Calculator](http://serverlesscalc.com/)
- [Top 10 Serverless Hosting Providers | Low-code backend to build modern apps](https://blog.back4app.com/serverless-hosting-providers/)
- [8 Serverless Computing Platform to Run Your Application Code](https://geekflare.com/serverless-computing-platform/)
- [Serverless is more expensive than you'd expect](https://webapp.io/blog/the-hidden-costs-of-serverless/)
- [choosing-a-database-with-serverless](https://www.serverless.com/blog/choosing-a-database-with-serverless/)

### Comparisons between cloud providers

- [Cloud Pricing Comparison 2021: AWS vs Azure vs Google Cloud](https://www.simform.com/blog/compute-pricing-comparison-aws-azure-googlecloud)
- [AWS vs Azure vs Google Cloud: which free tier is best?](https://cloudwith.me/posts/aws-vs-azure-vs-google-cloud-which-free-tier-is-best)
- [AWS vs Azure vs Google Free Tier Comparison | by Jay Chapel | Medium](https://jaychapel.medium.com/aws-vs-azure-vs-google-free-tier-comparison-19b68578e7f)
- [AWS Vs Azure Vs Google Cloud Free Tier Comparison 2021 - Mindmajix](https://mindmajix.com/aws-vs-azure-vs-google-cloud-free-tier)
- [Google Cloud vs Azure in 2021 (Comparing the Giants)](https://kinsta.com/blog/google-cloud-vs-azure/#billing-and-pricing)
- [Compare AWS and Azure services to Google Cloud](https://cloud.google.com/free/docs/aws-azure-gcp-service-comparison)
- [Google App Engine vs Heroku | Low-code backend to build modern apps](https://blog.back4app.com/google-app-engine-vs-heroku/)
- [Google Cloud Run vs. Heroku | Iron.io](https://blog.iron.io/google-cloud-run-vs-heroku/)
- [Google Cloud Platform vs Heroku - 2021 Comparison - Software Advice](https://www.softwareadvice.com/app-development/google-cloud-platform-profile/vs/heroku/)
- [Heroku Alternatives : AWS, Azure, and Google Cloud Platform | by Michael Rockford | Medium](https://medium.com/@GoRadialspark/heroku-alternatives-aws-azure-and-google-cloud-platform-870ae316527e)
- [Google Cloud Platform vs Heroku Enterprise 2021 Comparison | FinancesOnline](https://comparisons.financesonline.com/google-cloud-platform-vs-salesforce-app-cloud-heroku-enterprise)
- [(21) How does Google App Engine compare to Heroku? - Quora](https://www.quora.com/How-does-Google-App-Engine-compare-to-Heroku)
- [Firebase vs Heroku|What are the Differences? | Low-code backend to build modern apps](https://blog.back4app.com/firebase-vs-heroku/#:~:text=Unlike%20Firebase%2C%20Heroku%20developers%20can,many%20other%20server%2Drelated%20functions.&text=In%20comparison%2C%20Firebase%20allows%20the,in%20working%20with%20the%20backend.)
- [Firebase vs Netlify | Secrets unlocked | Low-code backend to build modern apps](https://blog.back4app.com/firebase-vs-netlify/)
- [Heroku vs AWS - Why Costs and Scale are Secondary Considerations](https://trifinlabs.com/heroku-vs-aws/)
- [Heroku vs AppEngine | UpGuard](https://www.upguard.com/blog/heroku-appengine)
- [Random Thoughts: GAE vs Heroku](https://kmilo0.blogspot.com/2013/02/gae-vs-heroku.html)
- [AWS vs Azure vs Google Free Tier Comparison | by Jay Chapel | Medium](https://jaychapel.medium.com/aws-vs-azure-vs-google-free-tier-comparison-19b68578e7f)
- [AWS vs Azure vs GCP: Difference Between Cloud Platforms](https://k21academy.com/amazon-web-services/aws-solutions-architect/aws-vs-azure-vs-gcp/)
- [Google vs Oracle: Gartner Peer Insights 2021](https://www.gartner.com/reviews/market/public-cloud-iaas/compare/google-vs-oracle)
- [AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba | A detailed comparison and mapping between various cloud services](https://comparecloud.in/)
- [AWS vs. Google vs. Azure vs. Oracle: Cloud Service Comparison • Sky.One](https://skyone.solutions/en/hub/cloud/aws-vs-google-vs-azure-vs-oracle-cloud-service-comparison/)
- [Cloud Run vs App Engine: a head-to-head comparison using facts and science - DEV Community](https://dev.to/pcraig3/cloud-run-vs-app-engine-a-head-to-head-comparison-using-facts-and-science-1225#:~:text=Overview%3A%20Cloud%20Run&text=Cloud%20Run%20runs%20containers%2C%20so,you%20focus%20on%20during%20development.)
- [Google Cloud Run vs. AWS Lambda: Performance Benchmarks (Part 2) - IOD](https://iamondemand.com/blog/google-cloud-run-vs-aws-lambda-performance-benchmarks-part-2/)
- [Google Cloud Functions vs App Engine vs Cloud Run vs GKE - Tutorials Dojo](https://tutorialsdojo.com/google-cloud-functions-vs-app-engine-vs-cloud-run-vs-gke/)
- [AWS App Runner VS Google Cloud Run](https://www.kloia.com/blog/aws-app-runner-vs-google-cloud-run)
- [Google Cloud Run vs. Heroku | Iron.io](https://blog.iron.io/google-cloud-run-vs-heroku/)
- [Google Cloud Run vs Heroku](https://www.linkedin.com/pulse/google-cloud-run-vs-heroku-fer-oliveira)
- [Cloud Run VS Cloud Functions: What’s the lowest cost? | by guillaume blaquiere | Google Cloud - Community | Medium](https://medium.com/google-cloud/cloud-run-vs-cloud-functions-whats-the-lowest-cost-728d59345a2e)
- [Serverless Architecture Providers: AWS vs Azure vs IBM vs Google | AltexSoft](https://www.altexsoft.com/blog/cloud/comparing-serverless-architecture-providers-aws-azure-google-ibm-and-other-faas-vendors/)
- [Serverless showdown: AWS Lambda vs Azure Functions vs Google Cloud Functions | A Cloud Guru](https://acloudguru.com/blog/engineering/serverless-showdown-aws-lambda-vs-azure-functions-vs-google-cloud-functions)
- [A Comparison of Serverless Function (FaaS) Providers](https://fauna.com/blog/comparison-faas-providers)
- [Serverless showdown: AWS Lambda vs Azure Functions vs Google Cloud Functions | A Cloud Guru](https://acloudguru.com/blog/engineering/serverless-showdown-aws-lambda-vs-azure-functions-vs-google-cloud-functions#h-the-tl-dr)
- [AWS Vs. Azure Vs. Google Cloud: Comparison Guide [2021]](https://sam-solutions.us/aws-vs-azure-v-s-google-cloud-which-is-better/)
- [12 BEST Cloud Hosting Provider In 2021 (Compared for Service and Cost)](https://www.softwaretestinghelp.com/best-cloud-hosting/)
- [Top Cloud Platform Comparison: 2021 Edition | Hacker Noon](https://hackernoon.com/top-cloud-platform-comparison-2021-edition-t7n35xd)

### Google cloud

- [google cloud platform - GCP GCE F1-micro not free? - Stack Overflow]()<https://stackoverflow.com/questions/58937320/gcp-gce-f1-micro-not-free#:~:text=It>'s%20f1%2Dmicro%20is%20always,charging%20you%20at%20that%20rate.
- [Exploring the Google Cloud f1-micro Instance - OpsDash](https://www.opsdash.com/blog/google-cloud-f1-micro.html)
- [F1-Micro Free Tier 1gb Network egress - what does this mean? : googlecloud](https://www.reddit.com/r/googlecloud/comments/l8l70v/f1micro_free_tier_1gb_network_egress_what_does/)
- [How Much Google Cloud Platform Charge You on F1-Mirco VM - Cybersecurity Memo](http://blog.51sec.org/2018/09/google-cloud-platform-hosting-charges.html)
- [google cloud platform - GCP GCE F1-micro not free? - Stack Overflow](https://stackoverflow.com/questions/58937320/gcp-gce-f1-micro-not-free)
- [Google Cloud Platform Pricing Calculator](https://cloud.google.com/products/calculator)
- [How to get a free Google server forever - DEV Community](https://dev.to/phocks/how-to-get-a-free-google-server-forever-1fpf)
- [virtual machine - Google cloud platform free tier limits from compute engine - Stack Overflow](https://stackoverflow.com/questions/63186893/google-cloud-platform-free-tier-limits-from-compute-engine)
- [Deploying Go App with HAProxy + Docker to Google Compute Engine | by Bismo Baruno | Easyread | Medium](https://medium.com/easyread/deploying-go-app-with-haproxy-docker-to-google-compute-engine-f7e01693b645)
- [Setting f1-micro resource limits in app.yaml for google cloud compute node.js app without vm_settings - Stack Overflow](https://stackoverflow.com/questions/31273834/setting-f1-micro-resource-limits-in-app-yaml-for-google-cloud-compute-node-js-ap)
- [gcloud - Cheapest way to host a simple node server and website with very few daily views on Google Cloud Platform - Stack Overflow](https://stackoverflow.com/questions/57828204/cheapest-way-to-host-a-simple-node-server-and-website-with-very-few-daily-views)
- [google app engine free tier and cloud platform - Stack Overflow](https://stackoverflow.com/questions/26632011/google-app-engine-free-tier-and-cloud-platform)
- [billing - How to run app on App Engine for free - Stack Overflow](https://stackoverflow.com/questions/35589951/how-to-run-app-on-app-engine-for-free)
- [Is there any free tier in Google compute engine - Stack Overflow](https://stackoverflow.com/questions/22706014/is-there-any-free-tier-in-google-compute-engine)
- [kubernetes - GKE Insufficient CPU for small Node.js app pods - Stack Overflow](https://stackoverflow.com/questions/56191553/gke-insufficient-cpu-for-small-node-js-app-pods)
- [google cloud platform - How can I run f1-micro instances on App Engine Flexible as of May 2017? - Stack Overflow](https://stackoverflow.com/questions/43807419/how-can-i-run-f1-micro-instances-on-app-engine-flexible-as-of-may-2017)
- [How I added a custom domain name to my Google Compute Engine VM | by Damilare D. Adekunle | Medium](https://medium.com/@ddadekunle/how-i-added-a-custom-domain-name-to-my-google-compute-engine-vm-6c42260ad8e6)
- [Upgraded free tier F1-micro VM to an E2-Micro?? : googlecloud](https://www.reddit.com/r/googlecloud/comments/oo55s1/upgraded_free_tier_f1micro_vm_to_an_e2micro/)
- [Are the E2-micro machines free? : googlecloud](https://www.reddit.com/r/googlecloud/comments/lh9a9o/are_the_e2micro_machines_free/)
- [Deploy a Node.js Application With App Engine in 10 Minutes!](http://www.theappliedarchitect.com/deploy-a-node-js-application-with-app-engine-in-10-minutes/)
- [Under the Hood with GCP’s App Engine](http://www.theappliedarchitect.com/under-the-hood-with-gcps-app-engine/)
- [App engine instances - what's the difference between instance sizes with same mem and cpu? - Stack Overflow](https://stackoverflow.com/questions/39261121/app-engine-instances-whats-the-difference-between-instance-sizes-with-same-me#:~:text=Historically%2C%20%22F%22%20stood%20for,in%20manual%20and%20basic%20scaling.)
- [Google app engine or amazon web services - Stack Overflow](https://stackoverflow.com/questions/15599210/google-app-engine-or-amazon-web-services)
- [google app engine - What is the equivalent of AWS elastic beanstalk in GCP? - Stack Overflow](https://stackoverflow.com/questions/23324517/what-is-the-equivalent-of-aws-elastic-beanstalk-in-gcp)
- [node.js - Please suggest Google Cloud App Engine's smallest configuration - Stack Overflow](https://stackoverflow.com/questions/49472727/please-suggest-google-cloud-app-engines-smallest-configuration)
- [An Overview of App Engine](https://cloud.google.com/appengine/docs/standard/nodejs/an-overview-of-app-engine)
- [How Instances are Managed](https://cloud.google.com/appengine/docs/standard/nodejs/how-instances-are-managed)
- [Beginners Guide To Google Cloud Compute Services](https://k21academy.com/google-cloud/google-cloud-compute-services/)
- [Introduction To Google Cloud Run | Steps To Deploy | Use Cases](https://k21academy.com/google-cloud/google-cloud-run/)
- [Google Cloud Platform Services And Tools For Beginners](https://k21academy.com/google-cloud/google-cloud-services-tools-for-beginners/)
- [Introduction To Google Cloud Run | Steps To Deploy | Use Cases](https://k21academy.com/google-cloud/google-cloud-run/#Pricing)
- [How to deploy your Node.js app with Google | by Kris Mason | Level Up Coding](https://levelup.gitconnected.com/how-to-deploy-your-node-js-app-with-google-2cd3771d5b21)
- [Google Cloud Run: the best hosting platform for dynamic apps - DEV Community](https://dev.to/pcraig3/google-cloud-run-the-best-host-platform-for-dynamic-apps-4ma6)
- [Kubernetes: Deploy a Node Express Application](https://docs.oracle.com/en-us/iaas/developer-tutorials/tutorials/node-on-k8s/01oci-node-k8s-summary.htm)
- [Building a “Serverless” RESTful API with Cloud Functions, Firestore and Express | by Dale Nguyen | ITNEXT](https://itnext.io/building-a-serverless-restful-api-with-cloud-functions-firestore-and-express-f917a305d4e6)
- [Building a REST API with Firebase cloud functions, TypeScript, and Firestore - LogRocket Blog](https://blog.logrocket.com/rest-api-firebase-cloud-functions-typescript-firestore/)
- [Building a REST API with Google Cloud Functions | by Andy Hume | Medium](https://medium.com/@andyhume/building-a-rest-api-with-google-cloud-functions-e0acdf1b2620)
- [Serverless node.js REST API with Google Cloud Function & Firestore | by Alfian Losari | Medium](https://alfianlosari.medium.com/serverless-node-js-rest-api-with-google-cloud-function-firestore-d7b422f58511)
- [Beginner's Guide for Creating a Serverless REST API using NodeJS over Google Cloud Functions - DEV Community](https://dev.to/levivm/creating-a-serverless-rest-api-using-google-cloud-functions-firebasefirestore-in-10-min-37km)
- [Express Routing with Google Cloud Functions | by Grant Timmerman | Google Cloud - Community | Medium](https://medium.com/google-cloud/express-routing-with-google-cloud-functions-36fb55885c68)
- [Express.js on Cloud Functions for Firebase | by James Hegedus | codeburst](https://codeburst.io/express-js-on-cloud-functions-for-firebase-f76b5506179)
- [Cloud Function and Cloud Run comparison - Google Sheets](https://docs.google.com/spreadsheets/d/1LiN8dNG5jB93KR-Km6UyNvvqXlBRjV9Brs1xIFoHI_Y/edit?usp=sharing)
- [Get on the Node.js Express to Google Cloud Functions](https://www.linkedin.com/pulse/get-nodejs-express-google-cloud-functions-doug-rehnstrom)
- [gcloud.tips: deploy cloud function from a Google Cloud Repository](https://gist.github.com/manekinekko/131820e3c9c9261a56595b5065d2ea76)
- [Firebase Cloud Functions Tutorial — Creating a REST API | by Diligent Dev | JavaScript in Plain English](https://javascript.plainenglish.io/firebase-cloud-functions-tutorial-creating-a-rest-api-8cbc51479f80)
- [Serve dynamic content and host microservices with Cloud Functions](https://firebase.google.com/docs/hosting/functions)
- [Serverless Node.js Functions Using Google Cloud | Toptal](https://www.toptal.com/nodejs/serverless-nodejs-using-google-cloud)
- [Nodejs google cloud function REST API demo | Codexpedia](https://www.codexpedia.com/node-js/nodejs-google-cloud-function-rest-api-demo/)
- [Firebase Pricing](https://firebase.google.com/pricing)
- [Deploy a Node.js Application With the App Engine in 10 Minutes! | by Andrew Didinchuk | Towards Data Science](https://towardsdatascience.com/deploy-a-node-js-application-with-app-engine-in-10-minutes-69b03e4d54f0?gi=269cd3490680)
- [Creating a Node.js REST API using Firebase Cloud Functions, without Express? - Stack Overflow](https://stackoverflow.com/questions/64682930/creating-a-node-js-rest-api-using-firebase-cloud-functions-without-express)
- [Comparing Google's Serverless Offerings: Cloud Run, Cloud Functions, App Engine | Splunk](https://www.splunk.com/en_us/blog/devops/gcp-serverless-comparison.html)

### AWS

- [cloudcommunity/Cloud-Service-Providers-Free-Tier-Overview: Comparing the free tier offers of the major cloud providers like AWS, Azure, GCP, Oracle etc.](https://github.com/cloudcommunity/Cloud-Service-Providers-Free-Tier-Overview)
- [AWS Free Tier Cost - DEV Community](https://dev.to/wparad/aws-free-tier-cost-3oi8)
- [Is the AWS Free Tier really free? - Last Week in AWS](https://www.lastweekinaws.com/blog/is-the-aws-free-tier-really-free/)
- [Azure Free Tier: Azure Free Account? Is it really free? - DEV Community](https://dev.to/azure/azure-free-account-is-it-really-free-53cb)
- [Side Projects That We Can Create With Free APIs - DEV Community](https://dev.to/aumayeung/side-projects-that-we-can-create-with-free-apis-270p)
- [AWS Elastic Beanstalk – Deploy Web Applications](https://aws.amazon.com/elasticbeanstalk/)
- [AWS Proton Pricing | Fully Managed Application Deployment Service | Amazon Web Services](https://aws.amazon.com/proton/pricing/)
- [AWS App Runner: a Container-Native Platform-as-a-Service – The New Stack](https://thenewstack.io/aws-app-runner-a-container-native-platform-as-a-service/#:~:text=There%20is%20one%20noteworthy%20difference,t%20support%20that%20use%20case.)
- [What does 400,000 GB-seconds compute mean? : aws](https://www.reddit.com/r/aws/comments/esgb8p/what_does_400000_gbseconds_compute_mean/)
- [Deploy And Run Docker Images on AWS ECS | by Sohel Ravankole | Clairvoyant Blog](https://blog.clairvoyantsoft.com/deploy-and-run-docker-images-on-aws-ecs-85a17a073281?gi=b3bc3a63c854)
- [The Best Docker Hosting Platforms of 2021 - Digital.com](https://digital.com/best-web-hosting/docker/)

### Oracle cloud

- [Cloud Cost Estimator](https://www.oracle.com/cloud/cost-estimator.html)
- [Cloud Pricing and Costs | Oracle](https://www.oracle.com/cloud/pricing/)
- [Oracle Cloud Always Free Tier | Oracle](https://www.oracle.com/cloud/free/?source=:ow:o:p:nav:0621CloudPricingButton&intcmp=:ow:o:p:nav:0621CloudPricingButton#always-free)
- [Google Cloud Platform Pricing Calculator](https://cloudpricingcalculator.appspot.com/)
- [The Oracle Cloud Free Tier. The New “Always Free Service”s… | by Franck Pachot | Medium](https://franckpachot.medium.com/the-oracle-cloud-free-tier-37c27f3b1e19)
- [5 Reasons why Oracle Free Tier is better than your Raspberry Pi | by Roberto Di Bella | Medium](https://roberto-di-bella.medium.com/5-reasons-why-oracle-free-tier-is-better-than-your-raspberry-pie-277ac8cb37e3)
- [ALWAYS FREE Oracle Cloud Free Tier — The Latest Services for Developers - Oracle Developers - Medium](https://medium.com/oracledevs/always-free-oracle-cloud-free-tier-the-latest-services-for-developers-56d154620425)
- [Judgement Day — the Oracle cloud goes on trial | by Paul Guerin | Medium](https://paulguerin.medium.com/judgement-day-the-oracle-cloud-goes-on-trial-e2e71e485bb9)
- [How to get 2x Oracle Cloud servers free forever - DEV Community](https://dev.to/phocks/how-to-get-2x-oracle-cloud-servers-free-forever-4o22)
- [Deploy a node app on Oracle Public cloud for free | by Vivek Kumar (Vik) | oracle-saas-paas | Medium](https://medium.com/oracle-saas-paas/deploy-a-node-app-on-oracle-public-cloud-for-free-7444b01c0659)
- [Writing Node.js apps for Oracle Autonomous JSON Database | Oracle Scripting and Oracle: Christopher Jones Blog](https://blogs.oracle.com/opal/writing-nodejs-apps-for-oracle-autonomous-json-database)
- [Simple Node.js backend app using Oracle Cloud Infrastructure(OCI) cloud native services | A-Team Chronicles](https://www.ateam-oracle.com/simple-nodejs-backend-app-using-oracle-cloud-infrastructureoci-cloud-native-services)
- [Deploy a Node.js Application to Oracle Cloud](https://www.oracle.com/webfolder/technetwork/tutorials/obe/cloud/apaas/node/getting-started-node-accs/getting-started-node-accs.html)
- [Overview of Object Storage](https://docs.oracle.com/en-us/iaas/Content/Object/Concepts/objectstorageoverview.htm)
- [Build a REST API with Node.js and Oracle 18c. | by Petros Koulianos 💀☠👽 | Javarevisited | Medium](https://medium.com/javarevisited/how-to-build-a-rest-api-with-node-js-and-oracle-18c-xe-f57bbbdd9b09)
- [Free Tier: Install Node Express on an Oracle Linux Instance](https://docs.oracle.com/en-us/iaas/developer-tutorials/tutorials/node-on-ol/01oci-ol-node-summary.htm)
- [Deploy a node app on Oracle Public cloud for free | by Vivek Kumar (Vik) | oracle-saas-paas | Medium](https://medium.com/oracle-saas-paas/deploy-a-node-app-on-oracle-public-cloud-for-free-7444b01c0659)
- [How to Create Always FREE Services in Oracle Cloud | K21 Academy](https://k21academy.com/1z0-932/how-to-create-always-free-services-in-oracle-cloud/)
- [OBIEE in IL: Oracle Always Free cloud Tier and what can we do with it](https://obieeil.blogspot.com/2020/09/oracle-always-free-cloud-and-what-can.html)
- [Andrej Baranovskij Blog: Multiple Node.js Applications on Oracle Always Free Cloud](https://andrejusb.blogspot.com/2019/11/multiple-nodejs-applications-on-oracle.html)
- [Andrej Baranovskij Blog: Running Oracle JET in Oracle Cloud Free Tier](https://andrejusb.blogspot.com/2019/09/running-oracle-jet-in-oracle-cloud-free.html)
- [Dimitri Gielis Blog (Oracle Application Express - APEX): Best and Cheapest Oracle APEX hosting: Free Oracle Cloud](https://dgielis.blogspot.com/2019/09/best-and-cheapest-oracle-apex-hosting.html)
- [Andrej Baranovskij Blog: FreeTier](https://andrejusb.blogspot.com/search/label/FreeTier)
- [Running Oracle JET in Oracle Cloud Free Tier | by Andrej Baranovskij | Oracle Developers | Medium](https://medium.com/oracledevs/running-oracle-jet-in-oracle-cloud-free-tier-9b324f3893b8)
- [How to Deploy Nodejs and Express REST APIs to Shared Hosting Including Database](https://morioh.com/p/e408c7800889)
- [Multiple Node.js Applications on Oracle Always Free Cloud by Andrej Baranovskij | Oracle WebLogic Partner Community EMEA Blog](https://blogs.oracle.com/emeapartnerweblogic/multiple-nodejs-applications-on-oracle-always-free-cloud-by-andrej-baranovskij)
- [Running Oracle JET in Oracle Cloud Free Tier by Andrej Baranovskij | Oracle WebLogic Partner Community EMEA Blog](https://blogs.oracle.com/emeapartnerweblogic/running-oracle-jet-in-oracle-cloud-free-tier-by-andrej-baranovskij)

### Alibaba Cloud

- [Simple Application Server Pricing: Single Server-Based Service - Alibaba Cloud](https://www.alibabacloud.com/product/swas/pricing?spm=a3c0i.7938564.8215766810.3.7781441eV7QZJ3)
- [Alibaba Cloud Pricing | Flexible and Cost-effective](https://www.alibabacloud.com/pricing#J_8215766810)
- [My 3-Month Experience with Alibaba Cloud | by Alibaba Cloud | Medium](https://alibaba-cloud.medium.com/my-3-month-experience-with-alibaba-cloud-f4435d968865)

### Azure

- [Pricing Calculator | Microsoft Azure](https://azure.microsoft.com/en-us/pricing/calculator/)
- [App Service | Microsoft Azure](https://azure.microsoft.com/en-gb/services/app-service/)
- [Free tier of Azure App Service? : AZURE](https://www.reddit.com/r/AZURE/comments/de8508/free_tier_of_azure_app_service/)

### Misc. Useful links

- [14 Best "Cheap Cloud Hosting" ($0.01 to $5.00) - Top Services for 2021](https://www.hostingadvice.com/how-to/best-cheap-cloud-hosting/)
- [6 Best Completely FREE Cloud Hosting Services 2021](https://www.websiteplanet.com/blog/best-free-cloud-hosting-services/)
- [Pricing | GearHost](https://www.gearhost.com/pricing)
- [Free for developers](https://free-for.dev/#/)
- [Top Free Hosting For Developers: Pros and Cons | by Janessa Tran | Meta Box | Medium](https://medium.com/meta-box/top-free-hosting-for-developers-pros-and-cons-bafc1d905274)
- [Free for developers major-cloud-providers](https://free-for.dev/#/?id=major-cloud-providers)
- [Top Free Hosting For Developers: Pros and Cons | by Janessa Tran | Meta Box | Medium](https://medium.com/@janessatran_28094?source=follow_footer-----bafc1d905274--------------------------------)
- [Limits – Vercel Docs](https://vercel.com/docs/platform/limits)
- [Cloud Pricing Calculator - CrowdStorage](https://crowdstorage.com/pricing/)
- [Pricing - UKCloud](https://ukcloud.com/pricing/)
- [AWS/Azure/Google Cloud Cost Calculator: Calculate the Price of Migration](https://l.dataart.com/cloud-migration)
- [[2021 Best] 6 Cloud Computing Services to Get Free VM - Super Easy](https://www.supereasy.com/100-free-6-best-cloud-service-providers/)
- [Looking for free server/tier providers that let you selfhost : selfhosted](https://www.reddit.com/r/selfhosted/comments/nniky3/looking_for_free_servertier_providers_that_let/)
- [Search Results - DEV Community](https://dev.to/search?q=free%20tier)
- [Awesome free cloud services for your next project - DEV Community](https://dev.to/rizkyrajitha/awesome-free-cloud-services-for-your-next-project-43mn)
- [10 Top PaaS Providers of 2021 - DevTeam.Space](https://www.devteam.space/blog/10-top-paas-providers/)
- [What is Backend as a Service (BaaS)? | Low-code backend to build modern apps](https://blog.back4app.com/backend-as-a-service-baas/)
- [Low-code backend to build modern apps | Back4App](https://www.back4app.com/)
- [What is Firebase? All secrets unlocked | Low-code backend to build modern apps](https://blog.back4app.com/firebase/)
- [Recommended minimum server sizes • Node](https://help.cloud66.com/node/references/non-recommended-server-sizes.html)
- [Convox Platform as a Service](https://convox.com/)
- [How to Deploy a Express Node.js app on Kubernetes and an Intro to Containerisation - DEV Community](https://dev.to/bmwhopper/how-to-deploy-a-express-nodejs-app-on-kubernetes-and-an-intro-to-containerisation-2fin)
- [Compare All Plans | Back4App](https://www.back4app.com/compare-all-plans)
- [What is a GB-second?](https://flaviocopes.com/what-is-a-gb-second/)
- [qsub - what is 'Gbytes seconds'? - Stack Overflow](https://stackoverflow.com/questions/13674729/what-is-gbytes-seconds)
- [11 Best Docker Hosting Platforms for your Containers](https://geekflare.com/docker-hosting-platforms/)
- [Docker cloud hosting. Cheap, simple and fast to deploy and manage](https://dockerize.io/)
