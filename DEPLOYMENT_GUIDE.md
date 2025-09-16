# Website Deployment Guide

## Quick Delivery Process (Sell → Deploy → Collect)

### Step 1: Make the Sale
- Show demo at: `https://your-demo-site.netlify.app`
- Price: $1200-1500 for professional website + lead capture
- Close with: "I can have this live for you in 24 hours"

### Step 2: Customize & Deploy (30 minutes max)

#### A. Quick Customization
1. **Change company info:**
   - Search/replace "Exterior Specialties" with their company name
   - Update phone number `(850) 556-4663`
   - Update service areas (Tallahassee → their city)
   - Update business details in About section

2. **Update contact form action:**
   ```html
   <!-- Replace the form action with Netlify Forms -->
   <form action="#" method="POST" netlify name="contact">
   ```

#### B. Netlify Deployment
1. **Create new repo** from your template
2. **Push to GitHub** with their company name
3. **Deploy to Netlify:**
   - Connect GitHub repo
   - Deploy settings: Build command: (none), Publish directory: (root)
   - Site name: `client-company-name`

#### C. Domain Setup Options

**Option 1: You Buy Domain ($15)**
- Buy domain on Namecheap/GoDaddy
- Point to Netlify
- Add $50 to invoice for "domain setup"

**Option 2: They Buy Domain**
- Give them DNS settings to update:
  - Type: CNAME
  - Name: www
  - Value: their-site.netlify.app
- You handle Netlify SSL setup

**Option 3: Use Netlify Subdomain (Free)**
- `their-company.netlify.app`
- Still professional looking
- Zero domain costs

### Step 3: Form Integration (5 minutes)

#### Netlify Forms (Easiest)
```html
<!-- Just add 'netlify' attribute to form -->
<form netlify name="contact" method="POST">
```
- Forms submit to Netlify dashboard
- You can forward to their email
- No server needed

#### Alternative: Formspree ($8/month)
```html
<form action="https://formspree.io/f/CLIENT_ID" method="POST">
```

### Step 4: Client Handover

**What they get:**
- Live website at their domain
- Contact form that emails them
- Mobile responsive design
- Professional online presence

**What you deliver:**
1. Live website URL
2. Login credentials (if needed)
3. Simple instruction sheet
4. "Website is live!" celebration

## Templates for Client Communication

### Email Template: Website is Live!
```
Subject: 🎉 Your Website is Now Live!

Hi [Client Name],

Great news! Your new website is now live at:
👉 www.[their-domain].com

✅ Professional design showcasing your services
✅ Mobile-friendly for all devices
✅ Contact form sending leads directly to your email
✅ Optimized for local search

You should start seeing the contact form submissions in your email within minutes.

Next steps:
- Share the link with customers
- Add it to your business cards
- Update your Google Business Profile

Questions? Just reply to this email!

Best regards,
[Your Name]
```

### Pricing Structure
- **Website + Basic Form:** $1200
- **Domain Setup:** +$50
- **Premium Design:** +$300
- **Monthly Updates:** $75/month (optional)

### Time Investment Per Client
- Customization: 20 minutes
- Deployment: 10 minutes
- Domain setup: 5 minutes
- **Total: 35 minutes per $1200+ sale**

## Pro Tips for Scaling

1. **Create template repo** - clone for each client
2. **Use environment variables** for easy text replacement
3. **Batch deployments** - do 3-4 clients at once
4. **Upsell maintenance** - monthly updates for recurring revenue
5. **Referral incentives** - discount for client referrals

This system lets you sell confidently knowing you can deliver quickly!