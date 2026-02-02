# Nanyuki Cottage Hospital - Multi-Page Website

A professional, fully animated, multi-page website for Nanyuki Cottage Hospital featuring comprehensive healthcare information, online appointment booking, and responsive design.

## 🎯 Project Overview

This is an **initial showcase** website with complete navigation structure and two sample detailed pages (one service, one department). All services and departments are listed in navigation dropdowns, ready for future expansion.

## 📁 File Structure

```
nanyuki-cottage-hospital/
│
├── index.html                           # Homepage
├── about.html                            # About Us page
├── services.html                         # Services listing
├── service-emergency.html                # Sample Service Detail Page (Emergency Care)
├── departments.html                      # Departments listing
├── department-internal-medicine.html     # Sample Department Detail Page
├── contact.html                          # Contact page with form & map
├── appointment.html                      # Appointment booking page
├── styles.css                            # All CSS styles and animations
├── script.js                             # All JavaScript functionality
└── README.md                             # This file
```

## 🌟 Features

### Pages Included
1. **Homepage (index.html)**
   - Animated hero section with typing effect
   - Features showcase
   - About preview
   - Services preview
   - Statistics with counters
   - Testimonials carousel
   - CTA sections

2. **About Us (about.html)**
   - Hospital story and history
   - Mission, Vision, Values
   - Why Choose Us section
   - Image galleries

3. **Services (services.html)**
   - Complete services listing
   - Card-based layout
   - Links to detail pages (1 implemented, others "Coming Soon")

4. **Service Detail - Emergency Care (service-emergency.html)**
   - Full service description
   - Features list
   - Why choose section
   - CTA for appointments

5. **Departments (departments.html)**
   - All departments listed
   - Interactive cards
   - Links to detail pages (1 implemented, others ready for expansion)

6. **Department Detail - Internal Medicine (department-internal-medicine.html)**
   - Comprehensive department info
   - Conditions treated
   - Approach and methodology
   - Appointment booking CTA

7. **Contact (contact.html)**
   - Contact information cards
   - Contact form
   - Google Maps integration
   - Multiple contact methods

8. **Appointment Booking (appointment.html)**
   - Comprehensive booking form
   - Date/time selection
   - Department selection
   - Payment method options
   - Form validation

### Navigation Structure

**Dropdown Menus Include:**

**Services:**
- Emergency & Trauma Care (✓ Page Created)
- Maternity & Children's Care
- Surgery & Endoscopy
- Laboratory & Diagnostics
- ICU & Critical Care
- Physiotherapy & Rehabilitation
- Radiology & Imaging
- Renal Dialysis
- Home Health Services

**Departments:**
- Internal Medicine (✓ Page Created)
- Orthopaedic & Spine
- Dental Services
- Optical & Eye Care
- Mental Health & Counseling
- Pharmacy
- Diabetes & Hypertension Clinic
- Nutrition & Dietetics
- Geriatric & Palliative Care
- Allergy Testing & Immunotherapy

## 🎨 Design Features

### Animations
- Fade in/out effects
- Slide animations
- Zoom effects
- Typing effects on hero title
- Parallax scrolling
- Ken Burns effect on images
- Card hover effects with 3D tilt
- Counter animations
- Carousel transitions
- Progress bar on scroll
- Pulse animations on CTA buttons

### Color Scheme
- **Primary Burgundy**: #8B1538
- **Gold Accent**: #D4AF37
- **Off-White**: #F8F6F2
- **Supporting colors** for various UI elements

### Typography
- **Headings**: Playfair Display (serif)
- **Body**: Inter (sans-serif)

## 🚀 Getting Started

### Option 1: Direct Browser Usage
1. Download all files to a folder
2. Open `index.html` in any modern web browser
3. Navigate through the site using the menu

### Option 2: Local Web Server (Recommended)

Using Python:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`

Using Node.js:
```bash
npm install -g live-server
live-server
```

### Option 3: Deploy to Web Host
1. Upload all files to your web hosting
2. Ensure all files are in the same directory
3. Access via your domain

## 📱 Responsive Design

Fully responsive with breakpoints at:
- **Desktop**: 1024px and above
- **Tablet**: 768px - 1023px
- **Mobile**: Below 767px

## 🔧 Customization Guide

### Adding More Service/Department Pages

To add a new service or department page:

1. **Copy an existing detail page** (e.g., `service-emergency.html`)
2. **Rename it** appropriately (e.g., `service-maternity.html`)
3. **Update the content**:
   - Page title
   - Hero image
   - Service/department name
   - Description
   - Features list
   - Images
4. **Update navigation** in all HTML files:
   - Change dropdown link from `services.html` to your new page

### Updating Colors

Edit CSS variables in `styles.css`:
```css
:root {
    --color-burgundy: #8B1538;
    --color-gold: #D4AF37;
    --color-off-white: #F8F6F2;
}
```

### Replacing Images

Replace placeholder images throughout HTML files:
- Hero sections: 1920x1080px recommended
- Service cards: 600x400px recommended
- Department icons: Use Font Awesome or custom icons

### Contact Information

Update in all HTML files:
- Phone: `+254 (062) 203 666`
- Email: `info@nanyukicottagehospital.co.ke`
- Address: Nanyuki Town, Laikipia County, Kenya
- Google Maps embed (in `contact.html`)

## 📋 Dependencies (CDN-loaded)

- **AOS** (Animate On Scroll) - v2.3.1
- **Swiper** - v11
- **Font Awesome** - v6.5.1
- **Google Fonts** - Inter & Playfair Display

No npm installation required!

## 🔒 Form Integration

Forms currently show success notifications. To integrate with backend:

### Email Integration (Simple)
Use a service like Formspree, EmailJS, or Web3Forms:

```javascript
// Example with EmailJS
emailjs.send('service_id', 'template_id', formData)
    .then(() => {
        showNotification('Message sent successfully!', 'success');
    });
```

### Backend Integration (Advanced)
```javascript
fetch('/api/appointments', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
})
.then(response => response.json())
.then(data => showNotification('Success!', 'success'))
.catch(error => showNotification('Error', 'error'));
```

## ✨ Interactive Elements

- Sticky navigation with scroll effect
- Mobile hamburger menu
- Smooth scrolling between sections
- Scroll-to-top button
- WhatsApp float button
- Animated counters
- Testimonials carousel
- Form validation
- Loading animations
- Progress bar
- Notification system

## 🎯 Next Steps for Full Implementation

1. **Create remaining service detail pages** (8 more)
2. **Create remaining department detail pages** (9 more)
3. **Add actual hospital images**
4. **Integrate forms with email/backend**
5. **Add Google Analytics**
6. **Implement SEO optimizations**
7. **Add blog/news section** (if needed)
8. **Set up proper 404 page**

## 📞 Support

For questions or customization needs:
- Email: info@nanyukicottagehospital.co.ke
- Phone: +254 (062) 203 666

## 🔄 Version History

### Version 1.0.0 (Current - Initial Showcase)
- ✅ 8 complete pages
- ✅ 2 sample detail pages (1 service, 1 department)
- ✅ Full navigation structure
- ✅ Responsive design
- ✅ Complete animation suite
- ✅ All dropdown menus populated
- ✅ Ready for expansion

## 📝 License

© 2026 Nanyuki Cottage Hospital. All rights reserved.

---

**Note**: This is an initial showcase version. The dropdown menus list all services and departments, but detailed pages are provided for Emergency Care (service) and Internal Medicine (department) as templates. Other pages can be created by duplicating and customizing these templates.

**Development Time**: Optimized for rapid deployment while maintaining professional quality.

**Browser Compatibility**: Chrome, Firefox, Safari, Edge (last 2 versions), Mobile browsers.
