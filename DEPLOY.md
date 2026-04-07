# Deploy to GitHub Pages

## Quick Setup Steps

### 1. Create GitHub Repository

Go to https://github.com/new and create a new public repository named `portfolio`.

### 2. Push Code to GitHub

Run these commands in your terminal (from the portfolio directory):

```bash
# Add the remote repository
git remote add origin https://github.com/revanth802/portfolio.git

# Push to main branch
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section (or click "Pages" in the left sidebar)
4. Under "Source", select **Deploy from a branch**
5. Select **main** branch and **/(root)** folder
6. Click **Save**

### 4. Access Your Live Site

Your portfolio will be live at:
**https://revanth802.github.io/portfolio**

(It may take 2-5 minutes to deploy)

---

## Setting Up Contact Form

The contact form uses Formspree (free tier available):

1. Go to https://formspree.io and sign up
2. Create a new form
3. Copy your form endpoint URL (e.g., `https://formspree.io/f/YOUR_FORM_ID`)
4. In `index.html`, find the form action and replace `YOUR_FORM_ID` with your actual form ID

---

## Customization

To customize your portfolio:

1. **Update Personal Info**: Edit text in `index.html`
2. **Change Colors**: Modify CSS variables in `:root` in `styles.css`
3. **Add Projects**: Edit the Projects section in `index.html`
4. **Add Profile Photo**: Replace the placeholder in the About section with an `<img>` tag

---

## Troubleshooting

**Site not showing?**
- Make sure the repository is public
- Check that GitHub Pages is enabled in Settings
- Wait 2-5 minutes for deployment

**Changes not reflecting?**
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check that files were pushed to the correct branch

**Form not working?**
- Make sure Formspree account is set up
- Verify the form action URL is correct
- Check spam folder for test submissions
