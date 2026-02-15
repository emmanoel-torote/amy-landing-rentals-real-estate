# Amy Rex Real Estate Landing Page

High-converting, SEO-optimized landing page for luxury real estate inquiries from vacation rental guests in Todos Santos, Pescadero, and Cerritos, Baja California Sur.

## Features

✅ **SEO Optimized**
- Complete Schema.org markup (RealEstateAgent, LocalBusiness, Service)
- Semantic HTML5 structure
- Optimized meta tags and Open Graph
- Mobile-first responsive design
- Fast loading (<2s LCP target)

✅ **Conversion Focused**
- QR code optimized (tracks source parameter)
- UTM parameter tracking
- Web3Forms integration (no backend needed)
- WhatsApp direct link
- Success message handling

✅ **Design**
- Barefoot luxury aesthetic
- Cormorant Garamond + Inter typography
- Terracotta (#A47B67) and Sand (#F6EDE4) brand colors
- Lots of white space
- Mobile-first responsive

## Deployment Instructions

### 1. Push to GitHub

```bash
git init
git add .
git commit -m "Initial commit: Amy Rex real estate landing page"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/amy-rex-real-estate.git
git push -u origin main
```

### 2. Deploy to Vercel

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Import your GitHub repository
4. Vercel will auto-detect it as a static site
5. Click "Deploy"

### 3. Configure Custom Domain (CNAME)

**In Vercel:**
1. Go to Project Settings → Domains
2. Add domain: `real-estate.amyrextodossantos.com` (or your preferred subdomain)
3. Vercel will provide CNAME values

**In your DNS provider (for amyrextodossantos.com):**
1. Add a CNAME record:
   - **Name**: `real-estate` (or your chosen subdomain)
   - **Value**: `cname.vercel-dns.com` (Vercel will provide exact value)
   - **TTL**: 3600 (or Auto)

2. Wait 5-60 minutes for DNS propagation

### 4. Update Landing Page

Once deployed, update these values in `index.html`:

1. **Phone number** (line 40, 69, 73, and WhatsApp link):
   - Replace `+52-XXX-XXX-XXXX` with actual number
   - Update WhatsApp link: `52XXXXXXXXXX`

2. **Canonical URL** (line 22):
   ```html
   <link rel="canonical" href="https://real-estate.amyrextodossantos.com">
   ```

3. **Open Graph URL** (line 18):
   ```html
   <meta property="og:url" content="https://real-estate.amyrextodossantos.com">
   ```

4. **Schema.org URLs** (lines 36-38):
   ```json
   "url": "https://real-estate.amyrextodossantos.com"
   ```

## QR Code Setup

Generate QR codes with source tracking:

- **Villa Aguamarina**: `https://real-estate.amyrextodossantos.com?source=aguamarina`
- **Costa Eterea**: `https://real-estate.amyrextodossantos.com?source=eterea`
- **Other properties**: `?source=PROPERTY_NAME`

The source parameter is automatically captured in the form submission.

## Form Integration

Uses **Web3Forms** (already configured):
- Access Key: `4b7a1a19-7581-48bf-a040-4b870a805045`
- No backend required
- Email notifications automatic
- Captures source tracking

## SEO Checklist Post-Deployment

- [ ] Submit to Google Search Console
- [ ] Verify canonical URL is live
- [ ] Test mobile responsiveness
- [ ] Check page speed (target <2s LCP)
- [ ] Verify Schema markup with Google Rich Results Test
- [ ] Test form submission
- [ ] Test WhatsApp link
- [ ] Verify QR code tracking parameters

## Analytics Integration (Optional)

Add Google Analytics by inserting before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-NHWG4QN3BW"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-NHWG4QN3BW');
</script>
```

## Browser Support

- Chrome/Edge (last 2 versions)
- Safari (last 2 versions)
- Firefox (last 2 versions)
- Mobile Safari (iOS 13+)
- Chrome Mobile (Android 8+)

## License

Proprietary - Amy Rex Property Management & Real Estate
