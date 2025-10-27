# eQMS - Quality Management System

A complete Quality Management System (QMS) web application built with Next.js, React, TypeScript, and Tailwind CSS.

## Features

### ✅ Complete QMS Functionality
- **Unique Event ID Generation**: Automatic generation of unique IDs (QMS-0001, QMS-0002, etc.)
- **Full Workflow Engine**: Draft → Submitted → Review → Approved → Closed
- **Complete Audit Trail**: Track all actions with timestamps and user details
- **Dynamic Dashboard**: Real-time statistics with charts and overdue event highlights
- **Extension Request Workflow**: Request and approve deadline extensions
- **Team Collaboration**: Cross-functional team assignment and management
- **Event Categorization**: Support for Deviation, Complaint, CAPA, NCR, Investigation

### 🎯 Technical Features
- **Next.js App Router**: Modern React framework with server-side rendering
- **TypeScript**: Type-safe development
- **Tailwind CSS**: Utility-first CSS framework
- **Recharts**: Interactive data visualization
- **Mock Backend**: In-memory JSON storage for development
- **Toast Notifications**: Real-time alerts for user actions
- **Responsive Design**: Works on desktop and mobile devices

## User Requirements Satisfaction

| Requirement | Status | Implementation |
|-------------|--------|----------------|
| QMS-01: Unique ID generation | ✅ | Auto-generated IDs (QMS-0001, QMS-0002, etc.) |
| QMS-02: Full workflow support | ✅ | Complete workflow engine with audit trail |
| QMS-03: Dynamic dashboard | ✅ | Real-time stats with charts |
| QMS-04: Due dates & overdue alerts | ✅ | Date tracking with overdue highlighting |
| QMS-05: Extension requests | ✅ | Full extension request workflow |
| QMS-06: Automatic notifications | ✅ | Toast notifications for events and due dates |
| QMS-07: Team collaboration | ✅ | User assignment and team management |
| QMS-08: Event categorization | ✅ | 5 event categories supported |

## Getting Started

### Prerequisites
- Node.js 18 or later
- npm (comes with Node.js)

### Installation

1. **Navigate to the project directory:**
   ```bash
   cd "c:\QC005\VS Code Works\eQMS Application\eQMS Quality management"
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Install additional required dependencies (if not already installed):**
   ```bash
   npm install autoprefixer tailwindcss-animate
   ```

4. **Start the development server:**
   ```bash
   npm run dev
   ```

5. **Open your browser:**
   Navigate to [http://localhost:3000](http://localhost:3000)

### Demo Accounts

The application comes with pre-configured demo accounts:

| Username | Password | Role | Department |
|----------|----------|------|------------|
| admin | password | Admin | Quality Assurance |
| john.doe | password | Manager | Manufacturing |
| jane.smith | password | User | Quality Control |
| mike.wilson | password | User | Regulatory Affairs |

## Application Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── dashboard/         # Dashboard page
│   ├── events/           # Event management
│   ├── audit/            # Audit trail
│   ├── extensions/       # Extension requests
│   ├── team/             # Team management
│   ├── login/            # Authentication
│   ├── layout.tsx        # Root layout
│   └── page.tsx          # Home page
├── components/           # Reusable components
│   ├── ui/              # UI components (Button, Input, Card)
│   ├── DashboardLayout.tsx
│   └── ProtectedRoute.tsx
├── contexts/            # React contexts
│   ├── AuthContext.tsx  # Authentication state
│   └── QMSContext.tsx   # QMS data management
├── lib/                 # Utilities and data
│   ├── qms-data.ts      # Mock data service
│   └── utils.ts         # Utility functions
└── types/               # TypeScript type definitions
    └── qms.ts          # QMS data types
```

## Key Features Walkthrough

### 1. Authentication
- Login with demo credentials
- Protected routes with automatic redirection
- User role-based permissions

### 2. Dashboard
- Real-time event statistics
- Interactive charts (Bar chart for status, Pie chart for categories)
- Recent events overview
- Overdue event alerts

### 3. Event Management
- Create new quality events with auto-generated IDs
- Full event lifecycle management
- Advanced filtering and search
- Workflow status updates
- Event details and editing

### 4. Audit Trail
- Complete activity history
- Filterable by event, action, and date
- Timeline view with user attribution
- Action icons and status changes

### 5. Extension Requests
- Request deadline extensions with justification
- Approval workflow for managers/admins
- Status tracking and comments
- Integration with main event workflow

### 6. Team Management
- User profiles and statistics
- Department overview
- Workload distribution analysis
- Activity summaries

## Workflow Engine

The QMS supports a complete workflow with the following states:

1. **Draft**: Initial creation state
2. **Submitted**: Ready for review
3. **Review**: Under evaluation
4. **Approved**: Approved for closure
5. **Closed**: Completed and archived

Each state change is automatically logged in the audit trail.

## Data Model

The application uses a comprehensive data model including:

- **QMSEvent**: Core event structure
- **User**: User management and authentication
- **AuditTrail**: Activity logging
- **ExtensionRequest**: Deadline extension management
- **DashboardStats**: Aggregated statistics

## Development Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Run linting
npm run lint
```

## Technologies Used

- **Frontend Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Charts**: Recharts
- **Icons**: Lucide React
- **Notifications**: React Hot Toast
- **State Management**: React Context API

## Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge

## Future Enhancements

Potential improvements for production use:

1. **Backend Integration**: Replace mock data with real API
2. **Database**: PostgreSQL/MySQL integration
3. **File Uploads**: Document attachments
4. **Email Notifications**: Real email integration
5. **Advanced Reporting**: PDF generation
6. **Mobile App**: React Native version
7. **SSO Integration**: Enterprise authentication

## Support

For questions or issues:
1. Check the browser console for errors
2. Verify all dependencies are installed
3. Ensure Node.js version compatibility
4. Check network connectivity for development server

## License

This is a demo application for quality management system evaluation.

---

**Last Updated**: September 2025
**Version**: 1.0.0