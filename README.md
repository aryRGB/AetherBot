# AetherBot 🤖

A powerful AI chatbot application built with the MERN stack, featuring conversational AI powered by Google Gemini and image generation capabilities through ImageKit.

## ✨ Features

- **Intelligent Conversations**: Engage in natural, context-aware conversations with advanced AI
- **Image Generation**: Create stunning images from text descriptions
- **User Authentication**: Secure authentication system with JWT tokens
- **Credit System**: Fair usage system with credit-based access
- **Image Management**: Store and manage generated images with ImageKit
- **Payment Integration**: Seamless payment processing with Stripe
- **Responsive Design**: Modern, mobile-friendly interface

## 🚀 Live Demo

**[Try AetherBot Now](#)** _(Replace with your deployment link)_

### How to Use the Live Demo

1. **Create an Account**: Click on the sign-up button and register with your email
2. **Welcome Credits**: You'll receive **10 free credits** upon registration
3. **Choose Your Mode**:
   - Look for the mode selector on the **left side of the textbox**
   - Select **"Text"** for conversational AI chat
   - Select **"Image"** to generate images from descriptions
4. **Start Creating**:
   - For text chat: Type your message and press send
   - For images: Describe what you want to create and let AI do the magic
5. **Monitor Credits**: Each interaction consumes credits - keep track in your dashboard

## 🛠️ Tech Stack

### Frontend

- **React.js**: Dynamic user interface
- **Axios**: HTTP client for API requests

### Backend

- **Node.js**: JavaScript runtime
- **Express.js**: Web application framework
- **MongoDB**: NoSQL database
- **Mongoose**: MongoDB object modeling

### AI & Services

- **Google Gemini API**: Advanced AI for conversational chat (accessed via OpenAI SDK)
- **ImageKit**: Image generation and storage
- **Stripe**: Payment processing
- **Svix**: Webhook management

### Security & Authentication

- **JWT (jsonwebtoken)**: Token-based authentication
- **bcryptjs**: Password hashing
- **CORS**: Cross-origin resource sharing
- **dotenv**: Environment variable management

## 📦 Dependencies

```json
{
  "axios": "^1.12.2",
  "bcryptjs": "^3.0.2",
  "cors": "^2.8.5",
  "dotenv": "^17.2.1",
  "express": "^5.1.0",
  "imagekit": "^6.0.0",
  "jsonwebtoken": "^9.0.2",
  "mongodb": "^6.20.0",
  "mongoose": "^8.19.2",
  "openai": "^5.12.2",
  "stripe": "^18.4.0",
  "svix": "^1.73.0"
}
```

## 🔧 Installation

### Prerequisites

- Node.js (v16 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Clone the Repository

```bash
git clone https://github.com/yourusername/aetherbot.git
cd Aetherbot
```

### Backend Setup

```bash
cd server
npm install
```

Create a `.env` file in the server directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
```

Start the backend server:

```bash
npm start
```

### Frontend Setup

```bash
cd ../client
npm install
npm run dev
```

## 🗂️ Project Structure

```
Aetherbot/
├── client/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   │   ├── ChatBox.jsx
│   │   │   ├── Message.jsx
│   │   │   └── Sidebar.jsx
│   │   ├── context/
│   │   │   └── AppContext.jsx
│   │   ├── pages/
│   │   │   ├── Community.jsx
│   │   │   ├── Credits.jsx
│   │   │   ├── Loading.jsx
│   │   │   └── Login.jsx
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── eslint.config.js
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── vercel.json
│   └── vite.config.js
├── server/
│   ├── configs/
│   │   ├── db.js
│   │   ├── imageKit.js
│   │   └── openai.js
│   ├── controllers/
│   │   ├── chatController.js
│   │   ├── creditController.js
│   │   ├── messageController.js
│   │   ├── userController.js
│   │   └── webhooks.js
│   ├── middlewares/
│   │   └── auth.js
│   ├── models/
│   │   ├── Chat.js
│   │   ├── Transaction.js
│   │   └── User.js
│   ├── routes/
│   │   ├── chatRoutes.js
│   │   ├── creditRoutes.js
│   │   ├── messageRoutes.js
│   │   └── userRoutes.js
│   ├── package.json
│   ├── package-lock.json
│   ├── server.js
│   └── vercel.json
└── README.md
```

## 🔐 Environment Variables

### Backend

| Variable                 | Description                                  |
| ------------------------ | -------------------------------------------- |
| `PORT`                   | Server port number                           |
| `MONGO_URI`              | MongoDB connection string                    |
| `JWT_SECRET`             | Secret key for JWT tokens                    |
| `GEMINI_API_KEY`         | Google Gemini API key                        |
| `IMAGEKIT_PUBLIC_KEY`    | ImageKit public key                          |
| `IMAGEKIT_PRIVATE_KEY`   | ImageKit private key                         |
| `IMAGEKIT_URL_ENDPOINT`  | ImageKit URL endpoint                        |
| `STRIPE_PUBLISHABLE_KEY` | Stripe publishable key                       |
| `STRIPE_SECRET_KEY`      | Stripe secret key                            |
| `STRIPE_WEBHOOK_SECRET`  | Stripe webhook secret for event verification |

## 💳 Credit System

- New users receive **10 free credits** upon registration
- Text conversations consume **1 credit** per message
- Image generation consumes **2 credits** per image
- Purchase additional credits through Stripe integration

## 🚀 Deployment

### Backend Deployment (Recommended: Railway/Render)

1. Push your code to GitHub
2. Connect your repository to Railway/Render
3. Add environment variables
4. Deploy

### Frontend Deployment (Recommended: Vercel/Netlify)

1. Build the production version: `npm run build`
2. Deploy the `dist` folder
3. Configure API endpoint

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

⭐ If you found this project helpful, please give it a star!
