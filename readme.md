# ShieldSphere - Enterprise Account Security Platform
  
  **Enterprise-grade account security monitoring and threat detection platform**

## 🎯 Problem Statement

In today's digital landscape, users face unprecedented security threats:
- **Account takeovers** through compromised credentials and brute-force attacks
- **Unauthorized access** from suspicious locations and unfamiliar devices
- **Lack of visibility** into login activities and security threats
- **Limited threat response** mechanisms for real-time attack mitigation
- **No compliance tracking** for GDPR and security standards
- **Difficulty in identifying** compromised passwords before damage occurs

Traditional security solutions are either too complex, lack real-time monitoring, or fail to provide actionable insights to users. Organizations and individuals need a **simple, intelligent, and proactive** security monitoring system.

---

## 💡 Solution

**ShieldSphere** is a production-ready cybersecurity platform that provides:

✅ **Real-time Login Monitoring** - Track every login attempt with location, device, and threat assessment  
✅ **Intelligent Threat Detection** - Automatic detection of brute force, impossible travel, and suspicious patterns  
✅ **Two-Factor Authentication** - TOTP-based 2FA with QR code setup  
✅ **Device Management** - Fingerprint and track all devices accessing your account  
✅ **Geolocation Tracking** - Interactive map showing login locations worldwide  
✅ **Password Breach Detection** - Check if your passwords have been compromised  
✅ **URL Phishing Scanner** - Analyze URLs for phishing and malware threats  
✅ **IP Reputation Checker** - Evaluate IP addresses for malicious activity  
✅ **Security Recommendations** - AI-driven suggestions based on your security profile  
✅ **Compliance Reports** - GDPR compliance reports with user data exports  
✅ **Auto-Response System** - Automatic account protection during detected threats  
✅ **Dashboard Analytics** - Comprehensive security analytics with visual charts  

---

## 🌟 Key Features

### 🔐 Authentication & Security
- Email/password registration and login
- Two-factor authentication (TOTP) with QR code
- Auto-response system for threat detection
- Secure session management with token-based auth

### 📊 Dashboard & Analytics
- Real-time security overview with key metrics
- Login success/failure breakdown charts
- Device and location statistics
- Recent activity timeline

### 🗺️ Location & Device Tracking
- Interactive Leaflet.js map visualization
- Device fingerprinting (browser, OS, user agent)
- Geographic distribution analysis
- Device type and browser breakdown

### ⚠️ Threat Detection & Prevention
- Real-time brute force detection
- Impossible travel detection
- Suspicious location alerts
- Device-based anomaly detection
- Automatic IP blocking for threats

### 🔍 Security Tools
- **Password Breach Checker** - Identify compromised credentials
- **URL Phishing Scanner** - Detect malicious URLs
- **IP Reputation Checker** - Analyze IP threat levels
- **Security Recommendations** - Priority-based security advice

### 📋 Compliance & Reporting
- GDPR compliance reports
- User data export functionality
- Access logs and audit trails
- Security incident documentation

### 🎨 User Experience
- Light/Dark mode with smooth transitions
- Responsive design for all devices
- Beautiful glassmorphism UI with animations
- Intuitive navigation and settings

---

## 🎁 Unique Features

1. **Production-Ready Design** - Enterprise-grade UI with premium cybersecurity aesthetic
2. **Real Backend Integration** - 100% integrated with Railway-deployed FastAPI backend
3. **Zero Hardcoding** - All data dynamically fetched from backend APIs
4. **Multi-Theme Support** - Light and dark modes with localStorage persistence
5. **Interactive Visualizations** - Maps, charts, and real-time data displays
6. **Comprehensive API Integration** - Leverages all backend endpoints
7. **Auto-Response Threat Mitigation** - Automatic protection on threat detection
8. **Enterprise Compliance** - Built-in GDPR and security standard reporting

---

## 📁 Project Structure

```
shieldsphere/
├── app/                          # Next.js App Router pages
│   ├── page.tsx                  # Home/Login page
│   ├── dashboard/
│   │   └── page.tsx              # Main dashboard
│   ├── login-dashboard/
│   │   └── page.tsx              # Detailed login analytics
│   ├── login-history/
│   │   └── page.tsx              # Login attempt history
│   ├── login-devices/
│   │   └── page.tsx              # Device management
│   ├── login-locations/
│   │   └── page.tsx              # Location tracking
│   ├── login-map-view/
│   │   └── page.tsx              # Interactive map visualization
│   ├── security-recommendations/
│   │   └── page.tsx              # Security advice
│   ├── compliance-reports/
│   │   └── page.tsx              # GDPR reports
│   ├── settings/
│   │   └── page.tsx              # Account settings & 2FA
│   ├── layout.tsx                # Root layout with theme provider
│   └── globals.css               # Global styles
│
├── components/
│   ├── auth/
│   │   ├── auth-form.tsx         # Login/Register form
│   │   └── two-fa-setup.tsx      # 2FA QR code setup
│   ├── dashboard/
│   │   ├── security-overview.tsx # Dashboard metrics
│   │   ├── security-alerts.tsx   # Alert cards
│   │   └── recent-activity.tsx   # Activity timeline
│   ├── layout/
│   │   └── dashboard-layout.tsx  # Sidebar navigation
│   └── ui/                       # shadcn/ui components
│       ├── button.tsx
│       ├── card.tsx
│       ├── input.tsx
│       ├── alert.tsx
│       └── ... (other UI components)
│
├── lib/
│   ├── theme-context.tsx         # Theme provider & context
│   └── api-client.ts             # API client utilities
│
├── config/
│   └── index.ts                  # Backend URL configuration
│
├── public/
│   ├── hero-dark-bg.jpg          # Dark mode hero background
│   ├── hero-light-bg.jpg         # Light mode hero background
│   └── dashboard-bg-dark.jpg     # Dashboard background
│
├── package.json                  # Dependencies
├── tsconfig.json                 # TypeScript config
├── tailwind.config.js            # Tailwind CSS config
├── next.config.mjs               # Next.js config
└── README.md                     # This file
```

---

## 🚀 Features Implementation

### Backend Integration
- **API Base URL**: `https://web-production-39f0f.up.railway.app`
- **All endpoints** fully integrated and functional
- **Real-time data** from Railway PostgreSQL database
- **Automatic authentication** with secure session management

### Frontend Technologies
- **Framework**: Next.js 16 with App Router
- **UI Library**: shadcn/ui with Radix UI
- **Styling**: Tailwind CSS v4 with custom themes
- **Charts**: Recharts for data visualization
- **Maps**: Leaflet.js for geolocation
- **State Management**: React hooks + localStorage
- **Forms**: React Hook Form with Zod validation

---

## 📋 Setup Instructions

### Prerequisites
- Node.js 18+ and npm/pnpm
- Backend running on Railway or localhost
- Environment variables configured

### 1. Clone & Install Dependencies

```bash
# Clone the repository
git clone <repository-url>
cd shieldsphere

# Install dependencies
npm install
# or
pnpm install
```

### 2. Configure Environment Variables

Create a `.env.local` file in the project root:

```env
# Backend API Configuration
NEXT_PUBLIC_API_URL=https://web-production-39f0f.up.railway.app

# For local development:
# NEXT_PUBLIC_API_URL=http://localhost:8000
```

### 3. Run Development Server

```bash
npm run dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 4. Build for Production

```bash
npm run build
npm start
# or
pnpm build
pnpm start
```

---

## 🌐 Deployment

### Deploy to Vercel (Recommended)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Add environment variable in Vercel dashboard:
# NEXT_PUBLIC_API_URL=https://web-production-39f0f.up.railway.app
```

### Environment Variables for Production
In your Vercel project settings, add:
- `NEXT_PUBLIC_API_URL` = Your backend URL

---

## 🔑 Key Endpoints Used

| Feature | Endpoint | Method |
|---------|----------|--------|
| Register | `/auth/register` | POST |
| Login | `/auth/login` | POST |
| 2FA Setup | `/2fa/setup/{email}` | GET |
| 2FA Verify | `/2fa/verify/{email}` | POST |
| Disable 2FA | `/disable-2fa/{email}` | POST |
| Login History | `/login-history/{email}` | GET |
| Login Dashboard | `/login-dashboard/{email}` | GET |
| Login Map | `/login-map/{email}` | GET |
| Devices | `/login-devices/{email}` | GET |
| Security Recommendations | `/security-recommendations/{email}` | GET |
| Password Breach Check | `/check-breached-password` | POST |
| URL Scan | `/scan-url` | POST |
| IP Reputation | `/get-ip-reputation` | POST |
| Compliance Report | `/compliance-report/{email}` | GET |
| Auto-Respond | `/auto-respond/{email}` | POST |

---

## 🎨 Customization

### Theme Colors
Edit `app/globals.css` to customize:
- Primary colors (cyan/blue)
- Accent colors
- Dark/light mode palette

### Background Images
Replace images in `public/`:
- `hero-dark-bg.jpg` - Dark mode login background
- `hero-light-bg.jpg` - Light mode login background
- `dashboard-bg-dark.jpg` - Dashboard background

### API Configuration
Update `config/index.ts` to change:
- Backend URL
- API timeout
- Default headers

---

## 🔒 Security Features

✅ **Encrypted Passwords** - bcrypt hashing in backend  
✅ **Secure Sessions** - HTTP-only cookies  
✅ **TOTP 2FA** - Industry-standard authentication  
✅ **Rate Limiting** - Brute force protection  
✅ **CORS Protection** - Secure cross-origin requests  
✅ **Data Validation** - Zod schema validation  
✅ **XSS Protection** - React sanitization  
✅ **HTTPS Only** - Enforced in production  

---

## 📊 Technology Stack

**Frontend:**
- Next.js 16.0+
- React 19.2+
- TypeScript 5+
- Tailwind CSS 4.1+
- shadcn/ui components

**Styling & UI:**
- Recharts (data visualization)
- Leaflet.js (maps)
- Lucide React (icons)
- Next Themes (dark mode)

**Backend Integration:**
- FastAPI (Python)
- PostgreSQL (Railway)
- JWT Authentication
- Email/Password + TOTP 2FA

---

## 🐛 Troubleshooting

### Build Errors
```bash
# Clear cache and rebuild
rm -rf .next
npm run build
```

### API Connection Issues
- Verify `NEXT_PUBLIC_API_URL` is correct
- Check backend is running
- Check browser console for detailed error logs
- Ensure CORS is enabled on backend

### Theme Not Persisting
- Clear browser localStorage
- Check that `localStorage` is enabled
- Verify theme toggle button functionality

---

## 📞 Support & Documentation

- **Backend Docs**: `https://web-production-39f0f.up.railway.app/docs` (Swagger)
- **Next.js Docs**: https://nextjs.org/docs
- **shadcn/ui**: https://ui.shadcn.com
- **Tailwind CSS**: https://tailwindcss.com

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 🙌 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

Frontend Deployment Link : frontend-sheild-sphere-ycdz.vercel.app