# 🎓 EduNFC - Smart Education Platform

Revolutionary NFC-based education platform for seamless student-teacher interactions with AI-powered insights.

![EduNFC Banner](https://via.placeholder.com/1200x400/FF6B35/FFFFFF?text=EduNFC+-+Smart+Education+Platform)

## ✨ Features

- 🎯 **NFC-Based Profiles** - Instant access with a simple tap
- 👨‍🎓 **Role-Based Dashboards** - Separate interfaces for students and teachers
- 📊 **Real-Time Analytics** - Track attendance, grades, and progress
- 🔐 **Secure Authentication** - Massar code integration with strong password requirements
- 🎨 **Modern UI** - Beautiful, responsive design with dark theme
- 📱 **Mobile Optimized** - Works seamlessly on all devices

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- PostgreSQL database (Vercel Postgres recommended)

### Installation

1. **Clone the repository**
   \`\`\`bash
   git clone https://github.com/yourusername/edunfc-app.git
   cd edunfc-app
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   \`\`\`

3. **Set up environment variables**
   \`\`\`bash
   cp .env.example .env.local
   # Edit .env.local with your database URL and other settings
   \`\`\`

4. **Initialize database**
   - Run the SQL scripts in `/scripts` folder
   - First: `create-tables.sql`
   - Then: `seed-data.sql`

5. **Start development server**
   \`\`\`bash
   npm run dev
   \`\`\`

Visit `http://localhost:3000` to see the application.

## 🏗️ Tech Stack

- **Framework**: Next.js 14 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: Radix UI + shadcn/ui
- **Database**: PostgreSQL
- **Authentication**: Custom with bcrypt
- **Icons**: Lucide React
- **Deployment**: Vercel

## 📱 Application Structure

\`\`\`
app/
├── auth/
│   ├── login/          # Login page
│   └── register/       # Registration with role selection
├── dashboard/
│   ├── student/        # Student dashboard
│   └── teacher/        # Teacher dashboard
├── api/
│   ├── register/       # Registration API
│   └── profile/        # Profile data API
└── globals.css         # Global styles

components/
├── ui/                 # shadcn/ui components
└── nfc-scanner.tsx     # NFC scanning component

scripts/
├── create-tables.sql   # Database schema
└── seed-data.sql       # Sample data
\`\`\`

## 🔐 Authentication

### Massar Code Format
- **Pattern**: 1 letter + 9 numbers (e.g., `A123456789`)
- **Unique**: Each user must have a unique Massar code
- **Required**: Mandatory for all registrations

### Password Requirements
- ✅ Minimum 8 characters
- ✅ At least 1 uppercase letter
- ✅ At least 1 lowercase letter  
- ✅ At least 1 number
- ✅ At least 1 special character

## 🎨 Customization

### Colors
- **Primary**: Orange (#FF6B35)
- **Accent**: Green (#10B981) & Red (#EF4444)
- **Background**: Black with gradients

### Fonts
- **Primary**: Inter
- **Secondary**: Poppins
- **Fallback**: System fonts

## 🚀 Deployment

### Deploy to Vercel

1. **Connect to Vercel**
   \`\`\`bash
   npm i -g vercel
   vercel login
   vercel
   \`\`\`

2. **Set up database**
   - Create Vercel Postgres database
   - Run SQL scripts via Vercel dashboard
   - Update environment variables

3. **Configure environment**
   \`\`\`env
   DATABASE_URL=your_postgres_url
   NEXTAUTH_SECRET=your_secret_key
   NEXTAUTH_URL=your_production_url
   \`\`\`

## 📊 Database Schema

### Core Tables
- **users** - User accounts and authentication
- **profiles** - Extended user profiles with NFC data
- **courses** - Course information and management
- **enrollments** - Student-course relationships
- **attendance** - Attendance tracking and analytics

## 🛠️ Development

### Available Scripts
\`\`\`bash
npm run dev          # Start development server
npm run build        # Build for production
npm run start        # Start production server
npm run lint         # Run ESLint
npm run type-check   # TypeScript type checking
\`\`\`

### Adding Features

1. **New Dashboard Widget**
   - Create component in `components/`
   - Add to respective dashboard
   - Update API if needed

2. **New User Role**
   - Update database schema
   - Add role-specific routes
   - Create dashboard components

3. **Real NFC Integration**
   - Install Web NFC API libraries
   - Update NFC scanner component
   - Add device compatibility checks

## 🔒 Security

- 🔐 Password hashing with bcrypt
- 🛡️ Input validation and sanitization
- 🔑 Unique Massar code verification
- 🚫 SQL injection prevention
- 🔒 Environment variable protection

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

- 📧 Email: support@edunfc.com
- 💬 Issues: [GitHub Issues](https://github.com/yourusername/edunfc-app/issues)
- 📖 Documentation: [Wiki](https://github.com/yourusername/edunfc-app/wiki)

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) for the amazing framework
- [Tailwind CSS](https://tailwindcss.com/) for utility-first styling
- [Radix UI](https://www.radix-ui.com/) for accessible components
- [Lucide](https://lucide.dev/) for beautiful icons

---

Made with ❤️ for the future of education
\`\`\`

Let me also create a .gitignore file:
