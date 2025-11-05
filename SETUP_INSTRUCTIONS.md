# Setup Instructions for GitHub Pages

## Your Information
- **GitHub Username:** WestonGuidero
- **Repository Name:** burn-and-turn-legal
- **Support Email:** burnandturnpokertrainer@gmail.com

---

## STEP 1: Create GitHub Repository (Browser - 2 minutes)

1. Go to: https://github.com/new
2. Fill in:
   - **Repository name:** `burn-and-turn-legal`
   - **Description:** "Legal documents for Burn and Turn Poker Trainer"
   - **Visibility:** ✅ Public (required for free GitHub Pages)
   - **DO NOT** check any initialization boxes (no README, no .gitignore, no license)
3. Click **"Create repository"**

---

## STEP 2: Push Files to GitHub (Terminal - Copy & Paste)

Once the repository is created, run these commands:

```bash
cd "J:\DOCUMENTS\Programming\Poker App\burn-and-turn-legal"

git branch -M main

git remote add origin https://github.com/WestonGuidero/burn-and-turn-legal.git

git commit -m "Initial commit: Privacy Policy and Terms of Service"

git push -u origin main
```

**Note:** You may be prompted to log in to GitHub. Follow the authentication prompts.

---

## STEP 3: Enable GitHub Pages (Browser - 1 minute)

1. Go to your repository: https://github.com/WestonGuidero/burn-and-turn-legal
2. Click **Settings** tab (top navigation)
3. Click **Pages** in the left sidebar
4. Under "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** Select `main` and `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for deployment
7. Refresh the page - you'll see: "Your site is live at https://westonguidero.github.io/burn-and-turn-legal/"

---

## STEP 4: Get Your Public URLs

After GitHub Pages is enabled, your documents will be available at:

- **Privacy Policy:**
  `https://westonguidero.github.io/burn-and-turn-legal/PRIVACY_POLICY`

- **Terms of Service:**
  `https://westonguidero.github.io/burn-and-turn-legal/TERMS_OF_SERVICE`

**Test the URLs** in your browser to make sure they load correctly!

---

## STEP 5: Update Google OAuth Consent Screen (Browser - 3 minutes)

1. Go to: https://console.cloud.google.com
2. Select your project (the one with Supabase OAuth)
3. Navigate to: **APIs & Services** → **OAuth consent screen**
4. Click **EDIT APP**

### Update these fields:

**App name:**
```
Burn and Turn Poker Trainer
```

**App logo:**
- Click "Upload Logo"
- Select: `J:\DOCUMENTS\Programming\Poker App\GtoPreFlopApp\assets\B-120x120.jpg`

**User support email:**
```
burnandturnpokertrainer@gmail.com
```

**Developer contact information:**
```
burnandturnpokertrainer@gmail.com
```

**Application home page (optional):**
```
https://westonguidero.github.io/burn-and-turn-legal/
```

**Privacy Policy URL:**
```
https://westonguidero.github.io/burn-and-turn-legal/PRIVACY_POLICY
```

**Terms of Service URL:**
```
https://westonguidero.github.io/burn-and-turn-legal/TERMS_OF_SERVICE
```

5. Click **SAVE AND CONTINUE**
6. Review Scopes page - should already have email and profile
7. Click **SAVE AND CONTINUE**
8. Review Test users (if applicable)
9. Click **BACK TO DASHBOARD**

---

## STEP 6: Test OAuth Branding (Terminal)

Run your app on web to test the new branding:

```bash
cd "J:\DOCUMENTS\Programming\Poker App\GtoPreFlopApp"
npm run web
```

1. Click "Sign in with Google"
2. You should now see:
   - **App name:** "Burn and Turn Poker Trainer"
   - **App logo:** Your B logo
   - Links to Privacy Policy and Terms

---

## Next Steps After Testing

Once OAuth branding is confirmed:

### Development Build (for testing on real devices):
```bash
cd "J:\DOCUMENTS\Programming\Poker App\GtoPreFlopApp"
eas build --profile development --platform ios
# or
eas build --profile development --platform android
```

### Preview Build (for internal testing/TestFlight):
```bash
eas build --profile preview --platform ios
# or
eas build --profile preview --platform android
```

---

## Summary Checklist

- [ ] Create GitHub repository `burn-and-turn-legal`
- [ ] Push files with git commands
- [ ] Enable GitHub Pages
- [ ] Verify URLs load in browser
- [ ] Update Google OAuth consent screen with all info
- [ ] Test OAuth flow on web (`npm run web`)
- [ ] Build development/preview builds for device testing

---

**Questions or issues?** Refer back to SESSION_STATUS.md in your main app folder.
