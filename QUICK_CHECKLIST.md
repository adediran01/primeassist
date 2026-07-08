# 🎯 PrimeAssist by AA — Quick Deployment Checklist

**Your website is fully customized and ready to deploy! Follow these steps in order.**

---

## ⏱️ ESTIMATED TIME: 45 minutes start-to-finish

---

## ✅ BEFORE YOU START (Have These Ready)

- [ ] GitHub account (free at github.com)
- [ ] Vercel account (free at vercel.com) — sign up with GitHub
- [ ] Resend account (free at resend.com) — for email service
- [ ] Your domain: primeassist.com (purchased)
- [ ] Access to your domain registrar (Namecheap, GoDaddy, etc.)

---

## 🔧 STEP 1: LOCAL SETUP (5 min)

```bash
# Install dependencies
cd primeassist-by-aa
npm install

# Create environment file
cp .env.example .env.local

# Test locally
npm run dev
# Visit http://localhost:3000
```

✅ **Check:** Homepage displays with navy/teal/gold colors

---

## 📤 STEP 2: PUSH TO GITHUB (5 min)

```bash
git init
git add .
git commit -m "Initial commit: PrimeAssist by AA"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/primeassist-by-aa.git
git push -u origin main
```

✅ **Check:** Code is on GitHub

---

## 🚀 STEP 3: DEPLOY TO VERCEL (5 min)

1. Go to vercel.com
2. Click "Add New" → "Project"
3. Select "primeassist-by-aa" repository
4. Click "Deploy"
5. Wait for deployment to complete

✅ **Check:** Site shows at `primeassist-by-aa.vercel.app`

---

## 🔑 STEP 4: ADD ENVIRONMENT VARIABLES (2 min)

On Vercel Dashboard:
1. Settings → Environment Variables
2. Add these for **Production**:

| Key | Value |
|-----|-------|
| `NEXT_PUBLIC_SITE_URL` | `https://primeassist.com` |
| `RESEND_API_KEY` | Get from resend.com → API Keys |
| `CONTACT_TO_EMAIL` | `adeyeraa2@gmail.com` |
| `CONTACT_FROM_EMAIL` | `PrimeAssist <noreply@primeassist.com>` |

3. Redeploy (Deployments → ⋮ → Redeploy)

✅ **Check:** Deployment succeeds

---

## 🌐 STEP 5: CONNECT DOMAIN (5 min)

### Get Resend API Key First:
1. Go to resend.com
2. Sign up / Log in
3. Dashboard → API Keys
4. Copy your API key (starts with `re_`)
5. Add to Vercel env vars above

### Connect Domain:
1. On Vercel: Settings → Domains
2. Enter: `primeassist.com`
3. Choose:
   - **Use Vercel Nameservers** (easiest) OR
   - **Add CNAME** (if keeping current registrar)
4. Follow Vercel's DNS instructions at your registrar
5. Wait 24-48 hours for DNS propagation

✅ **Check:** Vercel shows ✅ "Valid Configuration"

---

## 📧 STEP 6: SET UP EMAIL (5 min)

1. At resend.com dashboard
2. Go to "Domains"
3. Add: `primeassist.com`
4. Copy DNS records shown
5. Add these records at your domain registrar
6. Wait for verification (5-30 min)

✅ **Check:** Resend shows ✅ "Verified"

---

## 🔍 STEP 7: SET UP GOOGLE (5 min - Optional but recommended)

### Google Search Console:
1. Go to search.google.com/search-console
2. Add property: `primeassist.com`
3. Verify via DNS or HTML
4. Submit sitemap: `primeassist.com/sitemap.xml`

### Google Analytics:
1. Go to analytics.google.com
2. Create property: "PrimeAssist by AA"
3. Get Measurement ID: `G-XXXXXXXXXX`
4. Add to Vercel: `NEXT_PUBLIC_GA_ID = G-XXXXXXXXXX`
5. Redeploy

✅ **Check:** Domains verified, tracking active

---

## 🧪 STEP 8: FINAL TESTING (5 min)

**Visit:** `https://primeassist.com`

- [ ] Homepage loads with your colors
- [ ] Navigation works
- [ ] Services show 7 offerings
- [ ] Pricing in ₦ (Nigerian Naira)
- [ ] Portfolio shows 6 projects
- [ ] Contact form loads
- [ ] Dark mode toggle works
- [ ] Mobile responsive (test on phone)

**Test Contact Form:**
- [ ] Fill out and submit
- [ ] Check email inbox in 10 seconds
- [ ] Email comes from noreply@primeassist.com

✅ **Check:** All tests pass

---

## 📱 MOBILE TEST (2 min)

1. Visit on phone
2. Check:
   - [ ] Menu collapses to hamburger
   - [ ] Text is readable
   - [ ] Images load
   - [ ] Form works
   - [ ] Buttons clickable

✅ **Check:** Mobile responsive

---

## 🎉 LIVE! (You're Done!)

Your website is now:
- ✅ Live at primeassist.com
- ✅ Using your brand colors
- ✅ Showing your services & pricing
- ✅ Accepting inquiries via contact form
- ✅ Indexed by Google
- ✅ Ready for clients!

---

## 📣 SHARE WITH CLIENTS

```
🎉 PrimeAssist by AA is now live!

Visit: https://primeassist.com

We help brands grow through powerful design and smart marketing.
Professional. Creative. Results-Driven.

Let's create magic together! 💼✨

📱 WhatsApp: 08101607950
📧 Email: adeyeraa2@gmail.com
```

---

## ❌ TROUBLESHOOTING

### Emails not sending?
- [ ] Check RESEND_API_KEY in Vercel
- [ ] Verify domain in Resend dashboard
- [ ] Check spam folder

### Domain not working?
- [ ] DNS takes 24-48 hours
- [ ] Flush DNS: `ipconfig /flushdns` (Windows)
- [ ] Verify registrar nameserver settings

### Images not loading?
- [ ] Check image URLs in code
- [ ] Upload to Cloudinary or public folder

---

## 📞 NEXT STEPS

After launch:
1. Monitor contact form submissions
2. Add real client testimonials
3. Update portfolio as you complete projects
4. Write blog posts for SEO
5. Check Google Analytics for visitor behavior

---

## ✨ YOU'RE ALL SET!

Your professional website is live, branded perfectly, and ready to bring in clients.

**Enjoy! 🚀**
