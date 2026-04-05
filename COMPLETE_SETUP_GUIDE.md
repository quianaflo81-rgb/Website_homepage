# 🚀 Complete Setup Guide for quianacan.dev

## 📋 What You're Setting Up:

1. **quianacan.dev** → Portfolio landing page (NEW!)
2. **ethics.quianacan.dev** → Criminal Justice Ethics Analyzer (already deployed)
3. **warondugs.quianacan.dev** → War on Drugs site (currently on Wix)

---

## STEP 1: Deploy Portfolio Landing Page (5 min)

### A. Deploy to Netlify:
1. Download `portfolio-index.html` from this chat
2. Go to: https://app.netlify.com/drop
3. Drag the file onto the page
4. Netlify gives you a URL like: `random-name-123.netlify.app`

### B. Rename the site (optional):
1. Click "Site settings"
2. Click "Change site name"
3. Enter: `quianacan-portfolio` (or anything you want)

**Keep this browser tab open - you'll need it for DNS!**

---

## STEP 2: Connect ethics.quianacan.dev (5 min)

### A. In your Ethics Analyzer Netlify site:
1. Go to: https://app.netlify.com
2. Find your site: **ethical-cj-research**
3. Click it to open
4. Click **"Domain settings"** at top
5. Scroll to **"Custom domains"** section
6. Click **"Add custom domain"**
7. Enter: **ethics.quianacan.dev**
8. Click **"Verify"** then **"Add domain"**

### B. Get DNS settings:
Netlify will show you something like:
```
Type: CNAME
Name: ethics
Value: ethical-cj-research.netlify.app
```

**Write these down or take a screenshot!**

---

## STEP 3: Connect warondugs.quianacan.dev to Wix (10 min)

### A. In Wix Dashboard:
1. Go to your Wix dashboard: https://manage.wix.com
2. Click on your War on Drugs site
3. Go to **Settings** → **Domains**
4. Click **"Connect a domain you already own"**
5. Enter: **warondugs.quianacan.dev**
6. Wix will give you DNS records to add

**Write down the Wix DNS settings!**

---

## STEP 4: Connect quianacan.dev (main portfolio) (5 min)

### A. In your Portfolio Netlify site:
1. The site you just created in Step 1
2. Click **"Domain settings"**
3. Click **"Add custom domain"**
4. Enter: **quianacan.dev** (no subdomain)
5. Click **"Verify"** then **"Add domain"**

### B. Get DNS settings:
Netlify will show you something like:
```
Type: A
Name: @
Value: 75.2.60.5

Type: CNAME
Name: www
Value: your-site.netlify.app
```

**Write these down!**

---

## STEP 5: Add ALL DNS Records to Name.com (10 min)

Now you'll add ALL the DNS records you collected above.

### A. Go to Name.com:
1. Log in to: https://www.name.com
2. Click **"My Domains"**
3. Click **"quianacan.dev"**
4. Click **"DNS Records"** or **"Manage DNS"**

### B. Add these records:

**For main portfolio (quianacan.dev):**
```
Type: A
Host: @
Answer: 75.2.60.5
TTL: 300
```

**For ethics subdomain:**
```
Type: CNAME
Host: ethics
Answer: ethical-cj-research.netlify.app
TTL: 300
```

**For War on Drugs subdomain:**
```
Type: CNAME
Host: warondugs
Answer: [the value Wix gave you]
TTL: 300
```

**For www redirect:**
```
Type: CNAME
Host: www
Answer: [your-portfolio-site].netlify.app
TTL: 300
```

### C. Save all records

---

## STEP 6: Wait for DNS Propagation (15 min - 24 hours)

DNS changes can take time:
- Usually works in 15-30 minutes
- Can take up to 24 hours
- Check status at: https://dnschecker.org

### Test your sites:
- https://quianacan.dev (portfolio)
- https://ethics.quianacan.dev (ethics analyzer)
- https://warondugs.quianacan.dev (war on drugs)

---

## ✅ When Everything Works:

You'll have:
- ✅ Professional portfolio at your own domain
- ✅ Both projects accessible via subdomains
- ✅ Everything connected and working
- ✅ Free hosting forever (Netlify)
- ✅ Free domain for 1 year (GitHub Student)

---

## 🆘 Troubleshooting:

**"DNS verification pending"**
→ Wait 30 minutes, then check again

**"Site not found"**
→ Double-check DNS records match exactly what Netlify/Wix provided

**"SSL certificate pending"**
→ Netlify auto-generates SSL, can take 30 min after DNS resolves

**Still stuck?**
→ Take screenshots and come back to this chat!

---

## 🎉 Success!

Once working, you have a complete professional web presence:
- Your name as domain
- Multiple projects
- Professional presentation
- Perfect for resume/applications

**Cost: $0/year with GitHub Student Pack!**
