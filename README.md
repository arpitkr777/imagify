# Imagify - AI-Powered Text-to-Image Generator

![Imagify Logo](https://via.placeholder.com/150x50?text=Imagify)

A full-stack AI SaaS application that transforms text descriptions into stunning images using advanced generative AI technology. Built with the MERN stack and featuring a credit-based monetization system.

## 🚀 Features

- **AI Image Generation**: Convert text prompts into high-quality images in seconds
- **User Authentication**: Secure JWT-based authentication system
- **Credit System**: Purchase credits to generate images
- **Payment Integration**: Support for Razorpay and Stripe payment gateways
- **Responsive Design**: Modern, mobile-friendly UI built with Tailwind CSS
- **Real-time Notifications**: Toast notifications for user feedback
- **Smooth Animations**: Framer Motion powered animations for enhanced UX

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern JavaScript library for building user interfaces
- **Vite** - Fast build tool and development server
- **Tailwind CSS** - Utility-first CSS framework
- **Framer Motion** - Animation library for React
- **React Router** - Declarative routing for React
- **Axios** - HTTP client for API requests
- **React Toastify** - Toast notifications

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Tokens for authentication
- **bcrypt** - Password hashing
- **Razorpay & Stripe** - Payment processing

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- Node.js (v16 or higher)
- MongoDB (local or cloud instance)
- npm or yarn package manager

## 🔧 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/imagify.git
cd imagify
```

### 2. Backend Setup

```bash
cd server
npm install
```

Create a `.env` file in the server directory with the following variables:

```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
AI_API_KEY=your_ai_service_api_key
```

Start the backend server:

```bash
npm run server
```

### 3. Frontend Setup

```bash
cd ../client
npm install
```

Create a `.env` file in the client directory:

```env
VITE_BACKEND_URL=http://localhost:4000
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

Start the frontend development server:

```bash
npm run dev
```

### 4. Access the Application

Open your browser and navigate to `http://localhost:5173` (Vite's default port)

## 📖 Usage

1. **Sign Up/Login**: Create an account or log in to access the platform
2. **Purchase Credits**: Buy credits using Razorpay or Stripe to generate images
3. **Generate Images**: Enter a text description and click "Generate Images"
4. **View Results**: See your generated images in the results page
5. **Download/Share**: Download or share your AI-generated images

## 🗂️ Project Structure

```
imagify/
├── client/                 # React frontend
│   ├── public/            # Static assets
│   ├── src/
│   │   ├── assets/        # Images and icons
│   │   ├── components/    # Reusable React components
│   │   ├── context/       # React context for state management
│   │   ├── pages/         # Page components
│   │   └── ...
│   ├── package.json
│   └── vite.config.js
├── server/                # Node.js backend
│   ├── configs/           # Database configuration
│   ├── controllers/       # Route controllers
│   ├── middlewares/       # Custom middlewares
│   ├── models/           # MongoDB models
│   ├── routes/           # API routes
│   ├── server.js         # Main server file
│   └── package.json
└── README.md
```

## 🔗 API Endpoints

### User Routes
- `POST /api/user/register` - User registration
- `POST /api/user/login` - User login
- `POST /api/user/verify-razor` - Verify Razorpay payment
- `GET /api/user/credits` - Get user credits

### Image Routes
- `POST /api/image/generate-image` - Generate image from text prompt

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- AI image generation powered by [AI Service Provider]
- Payment processing by Razorpay and Stripe
- Icons and assets from various free resources

## 📞 Support

For support, email support@imagify.com or join our Discord community.

---

**Made with ❤️ using MERN Stack**