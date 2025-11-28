# Grit x Forge Payplan Calculator & CRM System

A comprehensive recruitment and payplan management system built for modern recruiting teams. Features include commission calculations, prospect pipeline management, training tracking, and advanced follow-up automation.

## 🚀 Features

### 💰 **Payplan Calculator**
- Interactive commission calculation tools
- PDF export functionality
- Role-based access (Rep, Veteran, Manager, Admin)
- Mobile-optimized responsive design

### 📊 **CRM Dashboard**
- Complete prospect pipeline management
- Advanced filtering and search capabilities
- Bulk actions for prospect management
- CSV import/export functionality
- Real-time statistics and metrics

### 🔔 **Follow-up Reminder System**
- Automated reminder alerts for overdue and due-today follow-ups
- **Notes display** directly on reminder cards
- **Follow-up purpose tracking** (interview prep, salary negotiation, etc.)
- **Recurring follow-up automation** (daily, weekly, monthly, etc.)
- Smart notification system with color-coded priority

### 🎓 **Training Tracker**
- Step-by-step training progress monitoring
- Dual notes system (public & internal trainer notes)
- Trainer assignment and notification system
- Self-progress updates for reps
- Role-based training visibility

### ⚙️ **Admin Portal**
- User management and role assignment
- System configuration and settings
- Advanced reporting and analytics
- Bulk user operations

## 📱 Mobile-First Design

### **App-Ready Features**
- Optimized for iOS/Android deployment
- Touch-friendly interface with 44px+ button targets
- Responsive hamburger navigation
- Smooth animations and transitions
- Native app-like styling and behavior

### **Mobile Optimizations**
- 16px font sizes to prevent iOS zoom
- Compact reminder cards with icon-only buttons
- Streamlined forms and inputs
- Mobile-specific spacing and padding

## 🔐 Authentication & Security

### **Role-Based Access Control**
- **Rep**: Access to calculator and own training tracker
- **Veteran**: Full CRM access, training oversight
- **Manager**: All Veteran permissions + advanced CRM features
- **Admin**: Complete system access + user management

### **Secure Authentication**
- Supabase-powered authentication
- Session management with localStorage
- Automatic login validation
- Secure logout across all pages

## 🛠️ Technology Stack

- **Frontend**: Vanilla HTML, CSS, JavaScript
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **PDF Generation**: jsPDF
- **Icons**: Bootstrap Icons (SVG)
- **Styling**: Modern CSS with gradients, animations, and responsive design

## 🗄️ Database Schema

### **Core Tables**
- `users` - User accounts and role management
- `prospects` - Prospect/candidate information and pipeline
- `training_steps` - Training progression tracking
- `section_notes` - Training notes and feedback
- `global_notes` - Internal notes system

### **Key Fields Added**
- `recurring_follow_up` - Automated follow-up intervals
- `followup_purpose` - Context for follow-up reminders
- `next_follow_up_date` - Scheduled follow-up tracking

## 🚀 Getting Started

### **Prerequisites**
1. Supabase account and project setup
2. Database tables created with proper schema
3. Web server or hosting platform

### **Installation**
1. Clone this repository
2. Update Supabase credentials in each HTML file:
   ```javascript
   const supabaseUrl = 'YOUR_SUPABASE_URL';
   const supabaseKey = 'YOUR_SUPABASE_ANON_KEY';
   ```
3. Run the following SQL commands in Supabase:
   ```sql
   ALTER TABLE prospects ADD COLUMN recurring_follow_up TEXT;
   ALTER TABLE prospects ADD COLUMN followup_purpose TEXT;
   ```
4. Deploy to your hosting platform

### **Configuration**
- Update logo references to your brand assets
- Customize color schemes in CSS variables
- Configure role-based navigation visibility
- Set up email/SMS integrations (optional)

## 📋 Usage

### **CRM Workflow**
1. **Add prospects** via form or CSV import
2. **Set follow-up dates** with optional recurring schedules
3. **Track reminders** with contextual notes and purposes
4. **Click prospect names** to view detailed training progress
5. **Complete follow-ups** to automatically schedule next ones

### **Training Management**
1. **Assign trainers** to specific reps or training sections
2. **Track progress** through multi-step training modules
3. **Add notes** (public for reps, internal for trainers)
4. **Monitor completion** rates and training effectiveness

### **Mobile Usage**
- **Hamburger menu** access on all pages
- **Icon-only buttons** for compact mobile interface
- **Touch-optimized** forms and interactions
- **Logout** available in sidebar menu across all pages

## 🎨 UI/UX Features

### **Modern Design Elements**
- Gradient backgrounds and card-based layouts
- Smooth hover effects and animations
- Status badges with gradients and shadows
- Mobile-first responsive breakpoints

### **Enhanced Usability**
- Contextual tooltips and help text
- Color-coded priority systems
- Visual feedback for all interactions
- Consistent navigation across pages

## 🔄 Recent Updates

### **v2.0 - Mobile & Follow-up Enhancement**
- ✅ Mobile-first responsive design overhaul
- ✅ Advanced follow-up reminder system with notes
- ✅ Recurring follow-up automation
- ✅ Clickable prospect names → training tracker
- ✅ Hamburger navigation with sidebar logout
- ✅ Enhanced status badges and visual polish
- ✅ Icon updates across all pages

## 🚀 Future Roadmap

### **Integration Features**
- Email automation for follow-ups
- SMS notification system  
- Calendar integration (Google Calendar, Outlook)
- Slack/Teams notifications

### **Advanced Features**
- Advanced analytics dashboard
- Automated reporting
- Performance metrics tracking
- API integrations for external tools

## 📞 Support

For technical support or feature requests, please create an issue in this repository.

## 📄 License

This project is proprietary to Grit x Forge. All rights reserved.

---

**Built with ❤️ for modern recruiting teams**