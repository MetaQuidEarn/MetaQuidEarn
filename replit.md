# Overview

MetaQuid is a modern task-based ad monetization platform with an attractive dark theme and smooth user interface. The platform allows users to earn money by watching advertisements and completing daily tasks. Built as a single-page application with Monetag SDK integration, automatic Telegram Mini App login, and multiple cryptocurrency/local payment withdrawal options with referral requirements.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Single-page Application (SPA)**: Built using vanilla HTML, CSS, and JavaScript without frameworks
- **Task-based Interface Design**: Two-panel layout with available tasks section and stats sidebar
- **Animated Background System**: Gradient background with smooth CSS animations
- **Component-based Styling**: Modern card-based design with smooth transitions and hover effects

## Design System
- **Typography**: Space Grotesk for headers and JetBrains Mono for monospace elements - creating a modern, professional aesthetic
- **Visual Theme**: Attractive dark theme with smooth animations and premium card-based layout
- **Color Scheme**: Professional color palette with blue/teal accents (#3B82F6, #10B981), gradient backgrounds, and clean card designs
- **UI Framework**: Advanced CSS with smooth transitions, cubic-bezier animations, subtle shadows and hover effects
- **Icons**: Custom emoji icons for payment methods and task categories
- **Responsive Layout**: Mobile-first responsive design with optimized layouts for all screen sizes

## Task-based Earning System
- **Task Types**: Advertisement viewing ($0.33), Daily check-in ($0.50)
- **Minimum Task Requirement**: 300 tasks must be completed before withdrawal eligibility
- **Daily Task Limits**: 50 tasks per day with progress tracking and visual progress bars
- **USD-based Rewards**: All earnings displayed in USD with real-time balance updates

## Earning Features
- **Monetag SDK Integration**: Real ad serving through Monetag (Zone: 9670918) with professional task interface
- **Task Rate Display**: Shows $0.33 per task in header statistics
- **Advertisement Revenue**: $0.33 per watched advertisement with smooth completion flow
- **Mobile-First Design**: Fully responsive interface optimized for mobile devices

## Payment Integration
- **Multiple Withdrawal Methods**: bKash, Nagad, Rocket, Binance Pay, Bitcoin, USDT
- **Minimum Withdrawal**: $30.00 threshold 
- **Referral Requirement**: Users must refer 10 people after reaching $30 to unlock withdrawal
- **Telegram Mini App Integration**: Full WebApp API integration with automatic login
- **Bot Notifications**: All user actions sent to Telegram bot via WebApp sendData API
- **Admin Contact**: Direct Telegram contact @sakibalhasannaim for support

## Telegram Mini App Features
- **Automatic Login**: Users automatically logged in when accessing via Telegram
- **User Data Integration**: App receives user's name, username, and Telegram ID
- **Native Telegram UI**: App adapts to Telegram's theme and interface
- **Real-time Bot Communication**: All activities sent to bot including logins, task completions, and withdrawal requests
- **Secure Authentication**: Uses Telegram's WebApp API for user verification

## Monetag Advertisement Integration
- **SDK Implementation**: Properly placed Monetag SDK below head tag as specified
- **Zone Configuration**: Zone 9670918 configured with show_9670918 function
- **Multiple Ad Formats**: Banner ads, popup ads, and main ad container
- **Ad Revenue Tracking**: $0.33 per ad view with real-time balance updates
- **Error Handling**: Fallback content when SDK not available

# External Dependencies

## CDN Services
- **Font Awesome**: cdnjs.cloudflare.com for icon library (v6.4.0)
- **Google Fonts**: fonts.googleapis.com for Poppins font family
- **Chart.js**: cdn.jsdelivr.net for data visualization library

## Browser APIs
- **Viewport API**: Meta viewport configuration for responsive design
- **CSS Backdrop Filter**: Modern browser features for glassmorphism effects

## Future Integration Points
- **Payment Gateways**: Architecture ready for Bangladeshi payment providers (bKash, Nagad, etc.)
- **Ad Networks**: Prepared for integration with local and international ad networks
- **Analytics Services**: Foundation laid for performance tracking and reporting services