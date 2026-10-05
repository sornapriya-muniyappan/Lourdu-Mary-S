🏛️ LegalEase - AI-Powered Legal Compliance Platform
LegalEase Logo
Automate your legal workflows with AI. Draft contracts, track compliance, and handle payments - all in one platform built for Indian startups and SMEs.

License FastAPI Next.js Blockchain MongoDB

🎯 Overview
LegalEase is a comprehensive AI-powered legal compliance and business automation platform designed specifically for Indian startups and SMEs. It combines cutting-edge AI technology with legal expertise to automate complex business processes, from document generation to tax filing and compliance management.

✨ Key Features
🤖 AI-Powered Legal Automation - Generate contracts, legal notices, and compliance documents
📊 Tax & GST Management - Automated ITR filing, GST returns, and compliance tracking
🔗 Blockchain Document Notarization - Immutable document verification on Base blockchain
👥 Specialized AI Agents - Dedicated agents for different legal and accounting tasks
📁 Advanced Document Management - OCR, smart categorization, and blockchain hashing
💬 Real-time Automation - WebSocket-based live updates and automation status
🏢 Complete Business Onboarding - Step-by-step business setup and compliance
📱 Modern Web Interface - Beautiful, responsive UI with professional legal theme
🏗️ Architecture
LegalEase is built with a modern microservices architecture:

Frontend (Next.js)  ←→  Backend (FastAPI)  ←→  Blockchain (Solidity)
     │                        │                      │
     │                   MongoDB Atlas          Base Network
     │                        │                      │
     └─────────────────   WebSocket   ─────────────────┘
                              │
                    GST Verification API
🚀 Quick Start
Prerequisites
Node.js 18+ and npm/yarn
Python 3.8+
MongoDB
MetaMask or compatible Web3 wallet
1. Clone the Repository
git clone https://github.com/your-username/legalease.git
cd legalease
2. Backend Setup
# Navigate to backend directory
cd backend

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Start the backend server
uvicorn main:app --reload
3. Frontend Setup
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your configuration

# Start the frontend server
npm run dev
4. Blockchain Setup (Optional)
# Navigate to blockchain directory
cd blockchain

# Install dependencies
npm install

# Set up environment variables
cp env.example .env
# Edit .env with your private key

# Deploy to Base Sepolia testnet
npm run deploy:base-sepolia
5. GST Verification API (Optional)
# Navigate to GST API directory
cd GST-Verification-API

# Install dependencies
pip install -r requirements.txt

# Start the GST verification service
python app.py
🔧 Configuration
Backend Environment Variables
# Database
MONGODB_URL=mongodb+srv://your-mongodb-url
MONGODB_DB_NAME=legalease

# AI Configuration
OPENAI_API_KEY=your-openai-api-key
GOOGLE_API_KEY=your-google-api-key
AI_PROVIDER=openai

# Security
SECRET_KEY=your-secret-key-here
CORS_ORIGINS=["http://localhost:3000"]

# File Upload
UPLOAD_DIR=uploads
MAX_FILE_SIZE=10485760  # 10MB
Frontend Environment Variables
# API Configuration
NEXT_PUBLIC_API_URL=http://localhost:8000
NEXT_PUBLIC_WS_URL=ws://localhost:8000

# Blockchain Configuration
NEXT_PUBLIC_REGISTRY_BASE_SEPOLIA=0xYourContractAddress
NEXT_PUBLIC_BASE_SEPOLIA_RPC=https://sepolia.base.org
📋 Features Overview
🤖 AI Agents
LegalEase includes specialized AI agents for different legal and accounting tasks:

Agent	Description	Capabilities
Tax Filing Copilot	Automated tax management	ITR filing, GST returns, tax calculation
Compliance Health Agent	Regulatory compliance monitoring	Deadline tracking, risk assessment, alerts
Notice Responder	Legal notice management	Notice analysis, response drafting, follow-up
Document Generator	Legal document creation	Contracts, agreements, templates
Trademark Assistant	IP management	Trademark search, filing, status tracking
General Assistant	Q&A and guidance	Legal queries, business advice, support
📊 Dashboard Features
Real-time Compliance Score - Track your business compliance status
Task Management - Upcoming deadlines and pending tasks
Document Analytics - Usage statistics and document insights
Automation Status - Live updates on running processes
Calendar Integration - Compliance deadlines and appointments
🔐 Document Management
Smart Upload - Drag & drop with automatic file type detection
OCR Processing - Text extraction from scanned documents
Blockchain Notarization - Immutable document verification
Advanced Search - Full-text search across documents
Folder Organization - Hierarchical document structure
Version Control - Track document changes and revisions
💼 Business Onboarding
Complete step-by-step business setup:

Basic Information - Company details and incorporation
Legal Structure - Entity type and shareholding
Compliance Setup - Tax registrations and licenses
Document Upload - Required business documents
Verification - AI-powered document verification
Activation - Business profile activation
🛠️ API Documentation
Authentication Endpoints
POST /api/v1/auth/register - User registration
POST /api/v1/auth/login - User login
GET /api/v1/auth/user/{email} - Get user profile
Business Management
POST /api/v1/businesses - Create business
GET /api/v1/businesses/{id} - Get business details
POST /api/v1/onboarding/start - Start onboarding process
Document Management
POST /api/v1/upload/document - Upload document
GET /api/v1/upload/document/{id} - Download document
GET /api/v1/upload/documents - List documents
Automation
WebSocket /api/v1/automation/ws - Real-time automation updates
POST /api/v1/tax-filing/initiate - Start tax filing process
Company Management
POST /api/v1/companies - Create company
GET /api/v1/companies - List companies
GET /api/v1/companies/{id} - Get company details
For complete API documentation, visit: http://localhost:8000/docs (Swagger UI)

🔗 Blockchain Integration
LegalEase integrates with the Base blockchain for document notarization:

Smart Contract Features
Document Notarization - Store SHA-256 hashes on-chain
Existence Verification - Check if documents are notarized
Immutable Storage - Permanent on-chain records
Event Emission - Real-time frontend integration
Contract Details
Network: Base Sepolia Testnet (Chain ID: 84532)
Contract: LegalEaseDocRegistry.sol
Features: Gas-optimized, duplicate prevention, event-based verification
📱 Frontend Pages
Core Pages
Landing Page (/) - Hero section with features overview
Dashboard (/dashboard) - Main application interface
Documents (/documents) - Document management interface
Agents (/agents) - AI agents management
Chat (/chat) - Conversational AI interface
Editor (/editor) - AI-powered document editor
Specialized Pages
Automation (/automation) - Browser automation interface
Compliance (/compliance) - Compliance tracking calendar
Settings (/settings) - Application configuration
Help (/help) - Documentation and support
Pricing (/pricing) - Subscription plans
🎨 Design System
LegalEase uses a professional legal theme with:

Color Palette: Legal brown (#8B4513) and warm cream (#F8F3EE)
Typography: Baskervville (headings) and Montserrat (body)
Components: Shadcn/ui with custom legal styling
Responsive Design: Mobile-first approach
Accessibility: WCAG 2.1 AA compliant
🧪 Testing
Run Tests
# Backend tests
cd backend
pytest

# Frontend tests
cd frontend
npm test

# Blockchain tests
cd blockchain
npm test
Test Coverage
Backend: API endpoints, business logic, database operations
Frontend: Component rendering, user interactions, API integration
Blockchain: Smart contract functionality, gas optimization
🚀 Deployment
Production Deployment
Backend Deployment (Railway/Heroku)
Frontend Deployment (Vercel/Netlify)
Database (MongoDB Atlas)
Blockchain (Base Mainnet)
Environment Setup
# Deploy backend
cd backend
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port $PORT

# Deploy frontend
cd frontend
npm run build
npm start

# Deploy blockchain
cd blockchain
npm run deploy:base
📊 Performance
Benchmarks
API Response Time: < 200ms average
Document Upload: < 5s for 10MB files
Blockchain Transaction: < 30s confirmation
AI Processing: < 10s for document generation
Optimization
Database Indexing: Optimized queries for fast retrieval
Caching: Redis for frequently accessed data
CDN: Static assets served via CDN
Code Splitting: Lazy loading for optimal performance
🔒 Security
Security Features
Data Encryption: End-to-end encryption for sensitive data
Authentication: JWT-based authentication system
Authorization: Role-based access control
Input Validation: Comprehensive input sanitization
Rate Limiting: API rate limiting and DDoS protection
Blockchain Security: Immutable document verification
🤝 Contributing
We welcome contributions! Please read our Contributing Guide for details on:

Code of conduct
Development process
Pull request guidelines
Issue reporting
Development Setup
# Fork the repository
git clone https://github.com/your-username/legalease.git
cd legalease

# Create feature branch
git checkout -b feature/your-feature-name

# Make your changes
# Test your changes
# Submit pull request
📝 License
This project is licensed under the MIT License. See the LICENSE file for details.

🆘 Support
Getting Help
Documentation: Check our comprehensive guides
Issues: Report bugs on GitHub Issues
Discussions: Join our GitHub Discussions
Email: Contact us at support@legalease.com
FAQ
Q: Is LegalEase free to use? A: LegalEase offers both free and premium plans. The free plan includes basic features, while premium plans unlock advanced AI capabilities and higher usage limits.

Q: Is my data secure? A: Yes, we use enterprise-grade encryption and follow strict data privacy regulations including GDPR and CCPA. Your documents are encrypted and never shared with third parties.

Q: Can I integrate LegalEase with other tools? A: Yes, LegalEase provides APIs for integration with popular tools like Google Workspace, Microsoft 365, and Slack.

🎉 Acknowledgments
OpenAI for AI capabilities
Base for blockchain infrastructure
MongoDB for database services
Vercel for frontend hosting
All contributors who made this project possible
Built with ❤️ for Indian startups and SMEs by Team AlphaQ
Website • Documentation • API • Status