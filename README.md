# vercel-redirect
Redirecting APEX domains on Vercel to your WWW subdomain for [Typedream](https://typedream.com/) landing pages.

**If you have your own Vercel Account and would like to deploy projects under your Vercel Account, as well as use Typedream to serve your landing page, you can do the following:**

Let's say you own the domain `example.com`, and want to run your project under `app.example.com` , and use Typedream for your landing page at `example.com`

### Part 1: Delegating `www.example.com` to Typedream
1. Add `app.example.com` to your deployment in your Vercel Account. This will make `example.com` to be owned by your Vercel account.
2. Delegate `www.example.com` to Typedream's Account: Ask [our support team](https://join.slack.com/t/asktypedream/shared_invite/zt-okdwowd0-1NR87SIoGX~OzVhhPoC9aw) to send over an email requesting the subdomain delegation. Once you receive the email, you should approve it.
3. When it's approved, go to Typedream > Site Settings > Custom Domain and enter `www.example.com`. This should now work.
4. You can **check that `www.example.com` is now showing your landing page**

### Part 2: Redirecting example.com to www.example.com
1. Clone this project
2. **Replace `www.example.com` under `vercel.json` on line 3 to your own domain.** 
3. Deploy it in your Vercel Account
4. Go to the deployment settings > Domains > add `example.com` to this deployment.
5. It will automatically redirect requests to `example.com/*` to `www.example.com/*`
6. Confirm that `example.com` now redirects to `www.example.com` and is showing your Typedream landing page

### Any questions?
[Chat us in Slack!](https://join.slack.com/t/asktypedream/shared_invite/zt-okdwowd0-1NR87SIoGX~OzVhhPoC9aw)
