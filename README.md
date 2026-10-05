# Lourdu-Mary-S
LegalEase - AI  Powered legal document generator 

This is not a simple doc generator - it's a full startup-level platform.

*✨ Key Features:*
- AI-Powered Legal Automation - Generate contracts, notices, compliance docs
- Tax & GST Management - Automated ITR filing, GST returns
- Blockchain Document Notarization - On Base blockchain
- Specialized AI Agents for legal/accounting tasks
- Document Management with OCR + smart categorization
- Real-time Automation via WebSocket

*🏗️ Architecture:*
Frontend (Next.js) <-> Backend (FastAPI) <-> Blockchain (Solidity)
     | | |
     | MongoDB Atlas Base Network
     └───────────────── WebSocket ─────────────────┘
                              |
                    GST Verification API
*🎨 Design System:*
- Color: Legal brown `#8B4513` + warm cream `#F8F3EE`
- Typography: Baskervville (headings) + Montserrat (body)
- Components: Shadcn/ui with custom legal styling a271

*📁 Special Pages:*
- `/editor` - AI document editor
- `/automation` - Browser automation
- `/compliance` - Compliance tracking calendar
- `/settings`, `/help`, `/pricing` a271

*🚀 How to Run:*

Backend:
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
Frontend:
cd frontend
npm install
npm run dev
Blockchain (Optional):
cd blockchain
npm install
npm run deploy:base-sepolia
*Performance:*
- API < 200ms, Document Upload < 5s, AI Processing < 10s a271
