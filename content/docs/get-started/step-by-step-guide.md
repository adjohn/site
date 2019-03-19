---
date: 2017-06-05
title: Dashbird Serverless Monitoring Step By Step Guide
linktitle: Step by step guide
description: Step by step guide that gives software engineers and CTOs the most comprehensive overview of Dashbird's monitoring and debugging features. 
kbSeries: ["BGet Started"]
kbSeries_weight: 300
---

Dashbird's goal is to give you an easy way to monitor your AWS Lambda Functions. We manage this through the concept of using **Organizations**, where one organization is one connected **AWS Account**. [Check this out](/docs/user-guide/organizations/)  for a more detailed explanation!

But for now, let's jump into explaining the **Organization settings**.

## Importer settings
<div class="row">
  <div class="col-md-7 col-sm-12 col-xs-12 text-md-left pt-3">
    <p class="lato">Go ahead and navigate to the <a href="https://app.dashbird.io/clients">Importer settings</a> page. It's in the top right section of the app under the organization name.</p>
    <p class="lato">By default, <b>all Lambdas</b> are imported <code>(*)</code>. </p>
    <p class="lato">Add one or more <b>filters</b> to select the right subset of Lambda Functions. Filters are <a href="https://en.wikipedia.org/wiki/Glob_(programming)">glob patterns</a>, meaning you can specify which Lambda Functions you want to import by matching a string and a wildcard(*). For instance, filter <code>*-prod-*</code> matches all function names like <code>service-prod-functionName</code>.</p>
  </div>
  <div class="col-md-5 col-sm-12 col-xs-12 imgs-fluid">
    <img src='/images/docs/client-importer.png'>
  </div>
</div>

![Importer](/images/docs/importer-settings.png)

<br>

## Alerting
The **Alerting** tab let's you enable company-wide alerts if your Lambda Functions are experiencing any errors. You can toggle digestions if errors keep happening, and enable sending e-mails or notifications to a Slack integration. To read more about [Alerting](/docs/user-guide/alerting/) jump over to that section in our docs.

![Alerting](/images/docs/client-alerting.png)

<br>

## Subscriptions
The **Subscriptions** tab defines which subscription you are currently using, with the options of upgrading to other plans.

## Invite users
If you wish, you can go ahead and invite users to your organization. This way all your team members can have access to the same **Organization** in your Dashbird account.

![Invite Users](/images/docs/client-invite-user.png)

On the **Invite users** tab you can see which users are connected to the organization. It's as easy as just pressing the **Add+** button and filling out a form, to add another user.

![Invite User Modal](/images/docs/inviteuser.png)

<br>

The **Organization settings** make a lot more sense now. Moving on let's check out the general layout of the Dashbird app!

## Left Side Navigation
 <div class="row">
  <div class="col-md-5 col-sm-12 col-xs-12 imgs-fluid">
    <img src='/images/docs/left-side-nav.png'>
  </div>
  <div class="col-md-7 col-sm-12 col-xs-12 text-md-left pt-3">
    <p class="lato">The side navigation is your primary means of navigating between Dashbird's main features. You can:</p>
    <ul>
      <li>**List** all Lambda Functions</li>
      <li>Debug Functions with **Live Tailing**</li>
      <li>Check your **Alerts**</li>
      <li>**List** all Projects</li>
      <li>Do an **account-wide search**</li>
    </ul>
  </div>
</div>

<br>

## Main Dashboard
The [main dashboard](https://app.dashbird.io/) is what you'll see once you sign in to your Dashbird account. It's where your most important metrics are, and where you have a bird's eye perspective on your whole system! Of course, you can navigate back to the main dashboard by clicking the Dashbird logo in the top left corner of your screen.

![Main Dashboard](/images/docs/overview.png)

You can quickly filter metrics based on when they occurred. Last 24h, yesterday, this week or this month are the quick settings which are available.

The main dashboard is also where you can have a glimpse at your **errors** and **alerts**. All of them are readily available to see in more detail through hot links in the UI.

---

This wraps up the **Get Started** section, go ahead and move on to the [**User Guide**](/docs/user-guide/monitoring/) for more hands-on tutorials on how to get the best out of Dashbird!
