 BC Solar Solutions - Multi-Tenant Lead Generation Platform

> **Professional solar quote generator for hosting multiple BC solar companies**

BC Solar Solutions is a production-ready multi-tenant platform that hosts solar installation companies across British Columbia. The platform generates professional solar quotes using satellite imagery analysis, AI-powered roof assessments, and accurate BC rebate calculations to capture and convert leads for solar dealers.

## 🚀 Live Demo

Experience the complete workflow from address input to professional PDF quotes with real satellite imagery and AI analysis.

## ✨ Key Features

### 🏢 Multi-Tenant Architecture
- **Host Multiple Solar Companies** - Each company gets custom branding and isolated quote data
- **Lead Generation Platform** - Professional quotes capture qualified leads for solar dealers
- **Custom Branding** - Company colors, logos, and contact information per tenant

### 🛰️ Advanced Technology
- **Real Satellite Imagery** - Esri World Imagery service provides actual roof views
- **AI-Powered Analysis** - Google Gemini API analyzes roof conditions and solar potential
- **Google Maps Integration** - Accurate address geocoding and location services
- **Professional PDF Quotes** - Print-optimized quotes with complete financial breakdowns

### 💰 BC-Specific Calculations
- **Accurate BC Hydro Rebates** - Up to $10,000 in provincial rebates calculated
- **Regional Pricing** - BC-specific solar panel and installation costs
- **Financial Analysis** - ROI calculations, payback periods, and 20-year savings projections

## 🛠️ Technology Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for fast development and building
- **Tailwind CSS** with shadcn/ui components
- **TanStack Query** for state management
- **Wouter** for client-side routing

### Backend
- **Express.js** with TypeScript
- **Drizzle ORM** with PostgreSQL support
- **In-memory storage** for development
- **RESTful API** design

### External Integrations
- **Google Gemini API** - AI roof analysis and proposal generation
- **Google Maps APIs** - Places API for address input
- **Esri World Imagery** - Real satellite imagery service
- **Google Solar API** - Building insights (optional)

## 🏗️ System Architecture

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   React Client  │    │  Express Server  │    │  External APIs  │
│                 │    │                  │    │                 │
│ • Address Input │───▶│ • Solar Analysis │───▶│ • Google Maps   │
│ • Roof Display  │    │ • AI Processing  │    │ • Gemini AI     │
│ • Quote Results │◀───│ • PDF Generation │    │ • Esri Imagery  │
│ • Multi-tenant  │    │ • Multi-tenant   │    │                 │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Google API keys (Gemini AI, Maps)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/bc-solar-solutions.git
cd bc-solar-solutions
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
# Create .env file with:
GEMINI_API_KEY=your_gemini_api_key
GOOGLE_MAPS_API_KEY=your_google_maps_key
```

4. **Start the development server**
```bash
npm run dev
```

5. **Open your browser**
Navigate to `http://localhost:5000`

## 📋 Complete Workflow

1. **Address Input** - Enter any BC residential address
2. **Satellite Analysis** - Real roof imagery automatically loaded
3. **AI Assessment** - Gemini API analyzes roof conditions and solar potential
4. **System Configuration** - Select solar panels and battery storage options
5. **Quote Generation** - Complete financial breakdown with BC rebates
6. **Professional PDF** - Print-ready quote with company branding

## 🏢 Business Model

### Lead Generation Platform
- **Host Multiple Companies** - Platform supports unlimited solar dealers
- **Custom Tenant Spaces** - Each company gets branded quote experience  
- **Qualified Lead Capture** - Professional quotes convert visitors to leads
- **Impressive Technology** - Satellite imagery and AI analysis build trust

### Revenue Streams
- **Platform Hosting Fees** - Monthly/annual fees for solar companies
- **Per-Quote Pricing** - Commission on generated quotes
- **Premium Features** - Advanced analytics and lead management

## 🔧 Configuration

### Adding New Solar Companies

```javascript
// Example tenant configuration
const newTenant = {
  businessName: "Solar Company Name",
  tagline: "Professional Solar Installation",
  phone: "(604) 555-0123",
  email: "info@solarcompany.com",
  address: "Vancouver, BC",
  primaryColor: "#005a87",
  secondaryColor: "#fdb913",
  isActive: true
};
```

### Customizing Pricing
Modify regional pricing in `server/services/solar.ts`:
- Solar panel costs per kW
- Battery storage pricing
- Installation labor rates
- BC Hydro rebate amounts

## 📊 API Documentation

### Core Endpoints

```bash
# Analyze address and generate solar potential
POST /api/solar/analyze
{
  "address": "123 Main St, Vancouver, BC",
  "latitude": 49.2500,
  "longitude": -123.1000
}

# Generate AI roof analysis
POST /api/solar/ai-analysis
{
  "roofImageUrl": "satellite_image_url",
  "solarConfigs": [{"panelsCount": 24, "yearlyEnergyDcKwh": 10466}]
}

# Create complete solar quote
POST /api/solar/quote
{
  "customerAddress": "123 Main St, Vancouver, BC",
  "solarSizeKw": 12,
  "panelCount": 24,
  "batterySize": 10,
  "yearlyEnergyKwh": 10466
}

# Generate PDF quote
POST /api/solar/generate-pdf
{
  "quoteId": 1
}
```

## 🔒 Security Features

- **Environment Variables** - All API keys stored securely
- **Input Validation** - Zod schema validation on all endpoints
- **Error Handling** - Graceful fallbacks for API failures
- **Rate Limiting** - Built-in protection against abuse

## 🚀 Deployment

### Replit Deployment (Recommended)
1. Import project to Replit
2. Set environment variables in Secrets
3. Click "Deploy"

### Manual Deployment
```bash
# Build for production
npm run build

# Start production server
npm start
```

## 📈 Roadmap

### Phase 1 (Current) ✅
- Multi-tenant quote generation
- Real satellite imagery
- AI-powered analysis
- Professional PDF quotes

### Phase 2 (Planned)
- **Lead Management Dashboard** - CRM for solar companies
- **Advanced Analytics** - Quote conversion tracking
- **Mobile App** - React Native companion app
- **Payment Integration** - Stripe for deposit collection

### Phase 3 (Future)
- **White-label Solution** - Fully customizable for each company
- **API Marketplace** - Third-party integrations
- **Advanced AI** - Predictive modeling and optimization

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini** - AI-powered roof analysis
- **Esri** - High-quality satellite imagery
- **BC Hydro** - Accurate rebate information
- **React Community** - Excellent development tools

## 📞 Support

For questions about hosting your solar company on our platform:
- Email: info@bcsolarsolutions.com
- Phone: (604) 555-0123
- Website: [BC Solar Solutions](https://bcsolarsolutions.com)

---

**Built with ❤️ for BC Solar Companies**

> Transform your solar business with professional lead generation technology
