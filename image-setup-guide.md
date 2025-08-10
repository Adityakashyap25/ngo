# Image Setup Guide for राष्ट्रीय ब्रह्मर्षि सेवा अभियान Website

## 📸 How to Add Images from Facebook Profile

### Step 1: Download Images from Facebook
1. Go to the Facebook page: https://www.facebook.com/people/राष्ट्रीय-ब्रह्मर्षि-सेवा-अभियान/100094250894826/
2. Right-click on images you want to use
3. Select "Save image as..." and save to your computer
4. Create a folder called `images` in your website directory

### Step 2: Organize Your Images
Create these folders in your `images` directory:
```
images/
├── hero/          # Main hero image
├── gallery/       # Activity photos
├── services/      # Service-related images
└── team/          # Team/volunteer photos
```

### Step 3: Update the Website with Real Images

#### A. Hero Section Image
Replace the placeholder in `index.html`:
```html
<!-- Current placeholder -->
<div class="hero-placeholder">
    <i class="fas fa-hands-helping"></i>
</div>

<!-- Replace with real image -->
<div class="hero-image">
    <img src="images/hero/main-hero.jpg" alt="राष्ट्रीय ब्रह्मर्षि सेवा अभियान" class="hero-img">
</div>
```

#### B. Gallery Section Images
Replace the placeholders in the gallery section:
```html
<!-- Current placeholder -->
<div class="gallery-placeholder">
    <i class="fas fa-users"></i>
    <p>सामूहिक सेवा</p>
</div>

<!-- Replace with real image -->
<div class="gallery-item">
    <img src="images/gallery/activity1.jpg" alt="सामूहिक सेवा" class="gallery-img">
    <div class="gallery-overlay">
        <h3>सामूहिक सेवा</h3>
    </div>
</div>
```

#### C. Service Section Images
Add images to service cards:
```html
<div class="service-card">
    <div class="service-icon">
        <img src="images/services/education.jpg" alt="शिक्षा सेवा" class="service-img">
    </div>
    <h3>शिक्षा सेवा</h3>
    <p>गरीब और वंचित बच्चों को निःशुल्क शिक्षा प्रदान करना।</p>
</div>
```

### Step 4: CSS Updates for Images

Add these styles to `styles.css`:

```css
/* Hero Image */
.hero-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 50%;
}

/* Gallery Images */
.gallery-img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.gallery-item:hover .gallery-img {
    transform: scale(1.05);
}

.gallery-overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: linear-gradient(transparent, rgba(0,0,0,0.7));
    color: white;
    padding: 20px;
    transform: translateY(100%);
    transition: transform 0.3s ease;
}

.gallery-item:hover .gallery-overlay {
    transform: translateY(0);
}

/* Service Images */
.service-img {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    object-fit: cover;
}
```

### Step 5: Recommended Images to Download

From the Facebook profile, look for these types of images:

1. **Hero Image**: Main organization photo or logo
2. **Gallery Images**:
   - Community service activities
   - Educational programs
   - Health camps
   - Environmental activities
   - Religious programs
   - Volunteer work

3. **Service Images**:
   - Education service photos
   - Health service photos
   - Social service photos
   - Environmental service photos

### Step 6: Image Optimization

Before adding images to the website:
1. **Resize images** to appropriate sizes:
   - Hero image: 600x600px
   - Gallery images: 400x300px
   - Service images: 200x200px

2. **Compress images** for faster loading:
   - Use online tools like TinyPNG
   - Keep file sizes under 200KB each

3. **Use appropriate formats**:
   - JPG for photographs
   - PNG for images with transparency
   - WebP for better compression (if supported)

### Step 7: Update Image Alt Text

Always add descriptive alt text in Hindi:
```html
<img src="images/gallery/health-camp.jpg" alt="स्वास्थ्य शिविर में डॉक्टर द्वारा जांच" class="gallery-img">
```

### Step 8: Test the Website

After adding images:
1. Open `index.html` in your browser
2. Check that all images load properly
3. Test responsive design on different screen sizes
4. Verify that images look good on mobile devices

## 🎯 Quick Implementation

If you want to quickly add images:

1. **Download 6-8 images** from the Facebook page
2. **Rename them** descriptively (e.g., `health-camp.jpg`, `education-program.jpg`)
3. **Create an `images` folder** in your website directory
4. **Place images** in the folder
5. **Update the HTML** using the examples above
6. **Add the CSS** for proper styling

## 📱 Mobile Considerations

When adding images, ensure they:
- Load quickly on mobile devices
- Look good on small screens
- Have appropriate alt text for accessibility
- Are optimized for web use

## 🔗 Facebook Integration

You can also add a direct link to the Facebook page:
```html
<div class="social-links">
    <a href="https://www.facebook.com/people/राष्ट्रीय-ब्रह्मर्षि-सेवा-अभियान/100094250894826/" target="_blank">
        <i class="fab fa-facebook"></i>
    </a>
</div>
```

This will help visitors connect directly to your Facebook page for more photos and updates. 