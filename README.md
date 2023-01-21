This repo is entirely the work of [blog post](https://jeroenpelgrims.com/access-the-firebase-auth-user-in-sveltekit-server-side/) on accessing the Firebase user in the SvelteKit backend.
I just added Hunter's form actions @ https://www.youtube.com/watch?v=EQy-AYhZIlE&t=0s for realtime CRUD with firestore minus the update bit. I also added sign in with email and password NB* I didn't bother adding signup so  you  need to add your own user in firebase auth. I also added some regx to the private key as cloudflare throws an error otherwise(I finally gave up with cloudflare after fixing the private key error as Cloudflare promptly dumped another precisely 161 errors on me!!) .This version will build but I could not get a deploy out of Cloudflare . I tested server side locally with ngrok and it works suprisingly really well considering my phone is my internet and I am in the sticks. If you do try and deploy on cloudflare you will need to add your env variables again in the cloudflare dashboard.  


To get this example running it should be enough to do the following steps:

- Clone this repo
- run `npm install`
- Create a `.env` file with the correct values.
  (Check `.env.sample` for the variables you need to set)
