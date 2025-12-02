# 🚀 Quick Start Guide

## Website PT. Lagada Jaya Sejahtera - Versi Modern

---

## ⚡ Cara Menggunakan Website

### 1. **Langsung Buka di Browser**
```
Cukup buka file: index.html
```
Website akan langsung berfungsi dengan semua fitur modern!

---

## 📱 Fitur Utama yang Bisa Dicoba

### ✅ **1. Loading Screen**
- Refresh halaman untuk melihat animasi loading

### ✅ **2. WhatsApp Float Button** (Pojok kanan bawah hijau)
- Klik untuk langsung chat via WhatsApp
- Selalu terlihat di semua halaman

### ✅ **3. Navigation Tabs**
- Beranda
- Tentang Kami
- Layanan
- Tim
- Kontak

### ✅ **4. Statistics Counter** (Di halaman "Tentang Kami")
- Scroll ke section untuk melihat angka naik otomatis
- 100+ Mitra, 50+ Events, 1000+ Transaksi, 95% Satisfaction

### ✅ **5. Services Accordion** (Di halaman "Layanan")
- Klik untuk expand/collapse detail
- 4 Paket Kopi + PPOB + Event Organizer

### ✅ **6. Testimonials** (Di halaman "Tim")
- Auto-rotate setiap 5 detik
- Klik arrow untuk manual navigation
- Klik dot untuk jump ke testimonial tertentu

### ✅ **7. FAQ Section** (Di halaman "Tim", setelah testimonial)
- Klik pertanyaan untuk lihat jawaban
- 6 pertanyaan umum
- Auto-close FAQ lain saat dibuka

### ✅ **8. Contact Form** (Di halaman "Kontak")
- Isi form lengkap
- Klik "Kirim via WhatsApp" → Otomatis buka WhatsApp
- Atau klik "Kirim via Email" → Buka email client

### ✅ **9. Scroll to Top Button** (Pojok kanan bawah, di atas WhatsApp)
- Muncul setelah scroll ke bawah
- Klik untuk kembali ke atas smooth

### ✅ **10. Mobile Menu**
- Resize browser ke ukuran mobile
- Klik hamburger menu (☰) di kanan atas
- Menu muncul dengan semua link

---

## 🎨 Customization Cepat

### Ganti Warna Utama
**File:** `index.html` & `modern-style.css`

```html
<!-- Ganti semua: -->
bg-blue-500 → bg-purple-500 (contoh)
text-blue-600 → text-purple-600
#3b82f6 → #yourcolor
```

### Ganti Nomor WhatsApp
**File:** `script.js` (line 233 & 364)

```javascript
// Ganti:
6282199968492
// Dengan nomor Anda (format: 62xxx tanpa +)
```

### Ganti Email
**File:** `index.html` (search: "Corporate@lakujoo.com")

```html
<!-- Ganti di 2 tempat: -->
<a href="mailto:Corporate@lakujoo.com">
```

### Tambah Testimonial
**File:** `index.html` (cari "testimonial-item")

```html
<!-- Copy block ini: -->
<div class="testimonial-item" data-testid="testimonial-4">
    <div class="flex justify-center mb-6">
        <img src="https://ui-avatars.com/api/?name=Nama+Baru&size=80&background=3b82f6&color=fff" alt="Nama Baru" class="rounded-full">
    </div>
    <p class="text-gray-600 text-lg mb-6 italic">
        "Quote testimonial di sini..."
    </p>
    <h4 class="font-bold text-gray-800">Nama Lengkap</h4>
    <p class="text-blue-500">Jabatan - Kota</p>
    <div class="flex justify-center mt-3 text-yellow-400">
        ★★★★★
    </div>
</div>

<!-- Tambah dot baru: -->
<span class="testimonial-dot" data-testid="testimonial-dot-4"></span>
```

### Tambah FAQ
**File:** `index.html` (cari "faq-item")

```html
<!-- Copy block ini: -->
<div class="faq-item" data-aos="fade-up" data-testid="faq-item-7">
    <div class="faq-question">
        <span>Pertanyaan baru?</span>
        <svg class="faq-icon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <polyline points="6 9 12 15 18 9"></polyline>
        </svg>
    </div>
    <div class="faq-answer hidden">
        Jawaban untuk pertanyaan baru.
    </div>
</div>
```

### Ubah Angka Statistik
**File:** `index.html` (cari "stat-card")

```html
<!-- Ganti data-target: -->
<span class="counter" data-target="100">0</span>
<!-- Angka 100 adalah target akhir -->
```

---

## 📂 File yang Perlu Diupload ke Hosting

### ✅ **Files Wajib:**
```
1. index.html          ← Main file
2. modern-style.css    ← Modern CSS
3. script.js           ← All JavaScript
4. style.css          ← Original CSS (optional, tapi included)
5. Images/            ← Folder dengan semua gambar
6. FlyerKoding.pdf    ← Brochure
7. KatalogFranchise.pdf ← Catalog
```

### 📖 **Files Dokumentasi (Optional untuk upload):**
```
- README.md
- UPGRADE_NOTES.md
- FEATURES.md
- BEFORE_AFTER.md
- QUICK_START.md (this file)
```

### 💾 **Backup Files (Jangan upload):**
```
- index.html.backup
- style.css.backup
```

---

## 🌐 Deploy ke Hosting

### Option 1: Upload via FTP/cPanel
```
1. Login ke hosting
2. Go to public_html/ atau www/
3. Upload semua files wajib
4. Done! Buka domain Anda
```

### Option 2: GitHub Pages
```
1. Create repository
2. Upload files
3. Enable GitHub Pages di Settings
4. Access via: username.github.io/repo-name
```

### Option 3: Netlify/Vercel (Gratis)
```
1. Drag & drop folder ke Netlify
2. Auto-deploy
3. Get free domain
```

---

## 🐛 Troubleshooting

### ❌ WhatsApp Button Tidak Muncul
**Solusi:**
- Cek file `modern-style.css` sudah diload
- Cek file `script.js` sudah diload
- Cek console browser untuk error

### ❌ Animasi Tidak Jalan
**Solusi:**
- Pastikan AOS library loaded (CDN)
- Cek JavaScript console
- Refresh halaman

### ❌ Form Tidak Kirim
**Solusi:**
- Form akan redirect ke WhatsApp, bukan email server
- Pastikan nomor WhatsApp benar di script.js
- Cek browser mengizinkan popup

### ❌ Counter Tidak Naik
**Solusi:**
- Scroll ke section statistics
- Pastikan Intersection Observer support
- Cek console untuk errors

### ❌ Mobile Menu Tidak Muncul
**Solusi:**
- Klik tombol hamburger (☰)
- Pastikan JavaScript loaded
- Check console errors

---

## 📊 Testing Checklist

Sebelum publish, test semua ini:

### Desktop
- [ ] Loading screen muncul
- [ ] All tabs navigation work
- [ ] Services accordion expand/collapse
- [ ] Statistics counter animate on scroll
- [ ] Testimonials auto-rotate
- [ ] FAQ expand/collapse
- [ ] Contact form validation
- [ ] WhatsApp float button click
- [ ] Scroll to top button
- [ ] All images load
- [ ] Hover effects work

### Mobile
- [ ] Responsive layout
- [ ] Mobile menu toggle
- [ ] Touch interactions work
- [ ] Buttons easy to tap
- [ ] Forms usable
- [ ] WhatsApp button visible
- [ ] Scroll smooth

### Cross-Browser
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] Edge
- [ ] Mobile browsers

---

## 🎓 Tips & Best Practices

### 1. **Keep It Updated**
- Update statistics numbers regularly
- Add new testimonials
- Update FAQ based on actual questions
- Refresh past events section

### 2. **Monitor Analytics**
- Add Google Analytics
- Track button clicks
- Monitor form submissions
- Check mobile usage

### 3. **Optimize Images**
- Compress images before upload
- Use WebP format for better performance
- Lazy load images if needed

### 4. **SEO**
- Update meta tags in `<head>`
- Add alt text to all images
- Use semantic HTML
- Submit sitemap to Google

### 5. **Performance**
- Test with Google PageSpeed Insights
- Optimize if needed
- Consider lazy loading for images
- Minimize external requests

---

## 💡 Pro Tips

### Tracking WhatsApp Clicks
```javascript
// Add to script.js for analytics
function openWhatsApp() {
    // Your analytics code here
    gtag('event', 'whatsapp_click', {
        'event_category': 'engagement',
        'event_label': 'WhatsApp Float Button'
    });
    
    window.open('https://wa.me/...', '_blank');
}
```

### Custom Loading Messages
```javascript
// In script.js, add text to loader:
<div id="loader">
    <div class="loader-spinner"></div>
    <p class="text-white mt-4">Memuat...</p>
</div>
```

### Add More Animations
```css
/* In modern-style.css */
.custom-animation {
    animation: yourAnimation 1s ease;
}

@keyframes yourAnimation {
    from { opacity: 0; }
    to { opacity: 1; }
}
```

---

## 📞 Support

Jika ada pertanyaan atau butuh bantuan:
- Email: Corporate@lakujoo.com
- WhatsApp: +62 821 9996 8492

---

## ✅ Launch Checklist

Final check sebelum launch:

- [ ] All content reviewed
- [ ] All links tested
- [ ] WhatsApp number correct
- [ ] Email addresses correct
- [ ] Images optimized
- [ ] Mobile tested
- [ ] Forms tested
- [ ] Analytics added
- [ ] SEO meta tags updated
- [ ] Favicon added (optional)
- [ ] Domain pointed correctly
- [ ] SSL certificate active
- [ ] 404 page setup (optional)

---

## 🎉 Ready to Launch!

Website Anda siap untuk:
✅ Attract customers
✅ Build trust
✅ Generate leads
✅ Showcase services
✅ Engage visitors
✅ Drive conversions

**Selamat! Website modern Anda sudah siap digunakan! 🚀**

---

*Dibuat dengan ❤️ menggunakan HTML, CSS, dan JavaScript modern*
