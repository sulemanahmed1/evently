You can visit the application and use the functionalities on this URL: https://evently-neon.vercel.app/ 
This application is created using Nextjs and MongoDB. Additional external libraries are use and are following 
Clerk for authentication (You have to create a webhook for Clerk as well)  
Stripe for payments      (You have to create a webhook for Stripe as well) 
SHADCN for UI components 
Uploadthing for uploading images 

In order to download and use this application you would have to install all the npm packages 

```bash 
npm install 
or
yarn install 
```

Thereafter you need to create a .env.local in the root folder and it should contain following keys or uri's. 
For the URL you could customize it to your linking. 

```bash 
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<Insert your Clerk key here> 

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

MONGODB_URI=<Your mongodb URI here and my db is named nextjs>  

UPLOADTHING_SECRET=<Your ULOADTHING_SECTRET here>  
UPLOADTHING_APP_ID=<Your ULOADTHING_APP_ID here>

NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=<Your Stripe fk key here>

STRIPE_WEBHOOK_SECRET=<Your Stripe webhook secret here>

// NEXT_PUBLIC_SERVER_URL=http://localhost:3000 ( for dev )
// NEXT_PUBLIC_SERVER_URL=http://<your app url> ( for prod, keep in mind if you are using https then add the 's' after http  )

```
