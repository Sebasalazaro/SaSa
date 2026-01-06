<p align="center">
  <img src="https://github.com/user-attachments/assets/cc959d7a-6ab4-4fb9-b34d-67d20c8af48c" alt="SaSa Logo" width="300"/>
</p>

<h1 align="center">SaSa - Save & Share</h1>

<p align="center">
  <strong>A sustainable food marketplace connecting businesses with surplus food to conscious consumers</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-18.3.1-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React"/>
  <img src="https://img.shields.io/badge/Node.js-Express-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/AWS-DynamoDB-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Material--UI-6.1.6-007FFF?style=for-the-badge&logo=mui&logoColor=white" alt="Material-UI"/>
</p>

---

## 🌍 Overview

**SaSa** is a full-stack web application inspired by TooGoodToGo, designed to combat food waste while making healthy food accessible to everyone. The platform enables restaurants, bakeries, supermarkets, farms, and other food businesses to sell surplus inventory at discounted prices before it goes to waste.

### 🎯 Key Features

- **🏪 Business Dashboard**: Complete admin interface for managing products, surprise boxes, and business profiles
- **📦 Surprise Boxes**: Mystery food packages offering 2x+ value of the purchase price
- **🗺️ Interactive Map**: Real-time geolocation showing nearby businesses with available deals
- **💚 Donation System**: Connect businesses with charitable organizations for food donations and certifications
- **🔐 Authentication System**: Secure user and business account management with cookies-based sessions
- **📱 Responsive Design**: Mobile-first approach with Material-UI components
- **🖼️ Image Management**: AWS S3 integration for efficient media storage
- **🤖 AI Integration**: OpenAI-powered features for enhanced user experience

---

## 🚀 Technology Stack

### Frontend
- **React 18.3** with Vite for lightning-fast development
- **Material-UI (MUI)** for consistent, professional UI components
- **React Router** for seamless navigation
- **Google Maps API** for interactive location features
- **Axios** for HTTP requests
- **TailwindCSS** + **Styled Components** for styling flexibility
- **React Hot Toast** for elegant notifications

### Backend
- **Node.js** with **Express.js**
- **AWS DynamoDB** with DynamoDB Toolbox for NoSQL data management
- **AWS S3** for scalable image storage with presigned URLs
- **OpenAI API** integration for AI-powered features
- **Cookie-based authentication** for secure session management
- **CORS** enabled for frontend-backend communication

### Development Tools
- **ESLint** for code quality
- **Nodemon** for automatic server restarts
- **Vite** for optimized frontend bundling

---

## 📁 Project Structure

```
SaSa/
├── client/                 # React frontend application
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── sections/      # Page-level components
│   │   ├── assets/        # Images, icons, and CSS
│   │   └── App.jsx        # Main application component
│   ├── vite.config.js
│   └── package.json
│
├── server/                # Node.js backend API
│   ├── controllers/       # Business logic handlers
│   ├── models/            # DynamoDB data models
│   ├── routes/            # API route definitions
│   ├── ddbClient.js       # DynamoDB configuration
│   ├── s3Client.js        # AWS S3 configuration
│   ├── aiApi.js           # OpenAI integration
│   ├── index.js           # Express server entry point
│   └── package.json
│
└── README.md
```

---

## 🛠️ Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- AWS Account with DynamoDB and S3 configured
- Google Maps API key
- OpenAI API key (optional, for AI features)

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/sasa.git
cd sasa
```

### 2. Backend Setup
```bash
cd server
npm install

# Create .env file with the following variables:
# AWS_ACCESS_KEY_ID=your_aws_access_key
# AWS_SECRET_ACCESS_KEY=your_aws_secret_key
# AWS_REGION=your_region
# S3_BUCKET_NAME=your_bucket_name
# OPEN_AI_API_KEY=your_openai_key

npm run dev
```

### 3. Frontend Setup
```bash
cd client
npm install

# Create .env file with:
# VITE_GOOGLE_MAPS_API_KEY=your_google_maps_key
# VITE_API_URL=http://localhost:5000

npm run dev
```

### 4. Access the Application
- Frontend: `http://localhost:5173`
- Backend API: `http://localhost:5000`

---

## 💡 Core Functionality

### For Businesses
1. **Register & Profile Management**: Create business profiles with location, hours, and contact info
2. **Product Management**: Add individual food items with pricing, descriptions, and images
3. **Surprise Box Creation**: Bundle surplus items into mystery packages
4. **Donation Partnerships**: Connect with charitable organizations for tax benefits
5. **Real-time Inventory**: Update availability instantly

### For Consumers
1. **Browse Nearby Deals**: Find discounted food on interactive maps
2. **Search & Filter**: Locate specific cuisines, dietary preferences, or business types
3. **Secure Purchases**: Cookie-based authentication for safe transactions
4. **Personalized Recommendations**: AI-powered suggestions based on preferences
5. **Support Local Businesses**: Contribute to sustainability while saving money

---

## 🗄️ Database Architecture

The application uses AWS DynamoDB with a single-table design pattern for optimal performance:

- **Users Table**: Consumer and business account information
- **Businesses**: Restaurant/store profiles with geolocation data
- **Products**: Individual food items with pricing and inventory
- **Surprise Boxes**: Bundled food packages
- **Donations**: Records of charitable contributions

All images are stored in AWS S3 with presigned URLs for secure access.

---

## 🔐 Security Features

- Cookie-based session management with `js-cookie`
- CORS configuration for controlled API access
- Environment variable protection for sensitive credentials
- AWS IAM roles for service-to-service authentication
- Input validation and sanitization

---

## 🌟 Future Enhancements

- [ ] Payment gateway integration (Stripe/PayPal)
- [ ] Push notifications for new deals
- [ ] Advanced analytics dashboard for businesses
- [ ] Mobile app (React Native)
- [ ] Multi-language support
- [ ] Carbon footprint tracking
- [ ] Loyalty rewards program
- [ ] Social sharing features

---

## 🤝 Contributing

This is a portfolio project, but suggestions and feedback are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Sebastian Salazar**  
Full-Stack Developer passionate about building apps that helps communities and people.

- 💼 LinkedIn: (www.linkedin.com/in/sebastian-salazar-osorio/)
- 📧 Email: sebasalazaro@gmail.com

**Valentina Morales**  
Software Engineer passionate about designing and building end to end full-stack apps.

- 💼 LinkedIn: (https://www.linkedin.com/in/valentina-morales-villada/)
- 📧 Email: valentinamoralesvillada13@gmail.com

---

## 🙏 Acknowledgments

- Inspired by [TooGoodToGo](https://toogoodtogo.com/)
- Built as part of academic coursework at EAFIT University with 
- Special thanks to all contributors and supporters of the project

---

<p align="center">
  <strong>⭐ If you found this project interesting, please consider giving it a star!</strong>
</p>

<p align="center">
  Made with ❤️ and ♻️ for a sustainable future
</p>
