# yuzu.party

```
 __  __     __  __     ______     __  __     ______   ______     ______     ______   __  __
/\ \_\ \   /\ \/\ \   /\___  \   /\ \/\ \   /\  == \ /\  __ \   /\  == \   /\__  _\ /\ \_\ \
\ \____ \  \ \ \_\ \  \/_/  /__  \ \ \_\ \  \ \  _-/ \ \  __ \  \ \  __<   \/_/\ \/ \ \____ \
 \/\_____\  \ \_____\   /\_____\  \ \_____\  \ \_\    \ \_\ \_\  \ \_\ \_\    \ \_\  \/\_____\
  \/_____/   \/_____/   \/_____/   \/_____/   \/_/     \/_/\/_/   \/_/ /_/     \/_/   \/_____/

```

Party planning software open(-sourced) to all. Check it out at [yuzu.party](https://yuzu.party). Built with the legendary [Fkit stack](https://www.youtube.com/watch?v=rFP7rUYtOOg).

## Development

1. Set up Firebase project.
   1. Enable Authentication and toggle the Phone method.
   2. Enable Firestore and copy over the rules in `firestore.rules`.
   3. Enable Storage and copy over the rules in `storage.rules`.
2. Set up a phone number on Twilio.
3. Copy `.env.example` to `.env` and fill in the values.
   1. For `SECRET_FIREBASE_SERVICE_ACCOUNT_KEY` refer to https://dev.to/vvo/how-to-add-firebase-service-account-json-files-to-vercel-ph5
4. Run `npm i`
5. Run `npm run dev`

## How to deploy

This project is optimized for `Vercel`. If you want to use something else, swap out `@sveltejs/adapter-vercel` with the appropriate adapter found at https://kit.svelte.dev/docs/adapters.

1. Set up a Vercel project.
2. Do all the configurations outline in `Development`.
3. Input the environment variables in the Vercel project settings.
4. Deploy!
