# 📧 Contact Form Setup Guide

## Step 1: Create a Formspree Account

1. Go to [https://formspree.io](https://formspree.io)
2. Click **Get Started** or **Sign Up**
3. Sign up with your email: `mahendra.ippala@gmail.com`
4. Verify your email address

## Step 2: Create a New Form

1. After logging in, click **+ New Form**
2. Name it: `Portfolio Contact Form`
3. Set the destination email to: `mahendra.ippala@gmail.com`
4. Click **Create Form**

## Step 3: Get Your Form ID

1. After creating the form, you'll see a URL like:
   ```
   https://formspree.io/f/xnqobzwq
   ```
2. Copy the form ID (the part after `/f/`)

## Step 4: Update Your Portfolio

1. Open `index.html`
2. Find this line (around line 489):
   ```html
   <form class="contact-form animate-on-scroll" id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
3. Replace `YOUR_FORM_ID` with your actual form ID:
   ```html
   <form class="contact-form animate-on-scroll" id="contactForm" action="https://formspree.io/f/xnqobzwq" method="POST">
   ```

## Step 5: Test the Form

1. Open your portfolio in a browser
2. Fill out the contact form
3. Click **Send Message**
4. You should receive an email at `mahendra.ippala@gmail.com`

## Step 6: Push to GitHub

```bash
cd /Users/mahendrareddyippala/Documents/n8n-workflows/portfolio
git add .
git commit -m "Setup contact form with Formspree"
git push origin main
```

## ✨ Features

- ✅ Direct email delivery to your inbox
- ✅ Success/error messages for users
- ✅ Loading state while sending
- ✅ Spam protection (built into Formspree)
- ✅ Free tier: 50 submissions/month
- ✅ No backend required

## 📊 Formspree Dashboard

You can view all submissions in your Formspree dashboard:
- See all messages
- Export to CSV
- Set up email notifications
- Enable spam filtering

## 🔒 Privacy

Formspree is GDPR compliant and doesn't share your data with third parties.

---

**Need help?** Contact Formspree support at [support@formspree.io](mailto:support@formspree.io)
