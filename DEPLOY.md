# Deploy to Firebase

## One-time setup

```bash
npm install -g firebase-tools
firebase login
firebase projects:create hyperlite-org   # or use existing project ID
```

Update `.firebaserc` with your actual Firebase project ID, then:

```bash
firebase deploy
```

## Custom domain (hyperlite.org)

1. Firebase Console → Hosting → Add custom domain
2. Enter `hyperlite.org`
3. Add the DNS records Firebase gives you to your domain registrar
4. SSL provisioned automatically

## Deploy after changes

```bash
firebase deploy
```

That's it. Static site — no build step needed.
