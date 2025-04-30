# 🌟 Elkaavie Platform

Fullstack application for room management with 3 integrated components:
- **Backend**: Laravel (PHP)
- **Frontend**: React + TypeScript
- **Admin Panel**: Flutter (Mobile)

## 🛠 Tech Stack

**Backend**:
- Laravel 10
- MySQL
- REST API
- Laravel Sanctum (Authentication)
- Database migration system

**Frontend**:
- React 18
- TypeScript
- Tailwind CSS
- Axios
- Responsive design

**Admin**:
- Flutter 3
- Dart 3
- Material Design
- HTTP Client for API communication
- Interactive UI components

## 🚀 Key Features

- Multi-role authentication (User & Admin)
- Interactive dashboard with navigation between sections
- Room availability management with confirmation dialogs
- Booking status visualization with progress indicators
- Booking filtering and management
- User management with booking history
- Enhanced development environment with hot reload support
- Swiss design principles with clean typography and whitespace

## 💾 Database Structure

- Optimized database schema with normalized tables
- Room information directly integrated into rooms table
- Efficient relationships between users, rooms, and bookings
- Complete booking lifecycle management
- Visual database documentation (DBML)

## 📂 Folder Structure

```
elkaavie/
├── backend/          # Laravel (API & Core Logic)
│   ├── app/          # Models, Controllers
│   ├── config/       # Application configuration
│   ├── database/     # Migrations and seeders
│   └── routes/       # API endpoints
├── frontend/         # React (Web Interface)
│   ├── src/
│   │   ├── pages/    # Frontend pages
│   │   └── components/ # Reusable components
└── admin/            # Flutter (Mobile Admin)
    ├── lib/
    │   ├── screens/  # Admin UI screens
    │   ├── services/ # API communication
    │   └── utils/    # Helper functions
    └── test/         # Test files
```

## 💻 Development Environment

### Using the Interactive Run Script

The project includes an enhanced `run.sh` script for managing the development environment:

```bash
# Start all services
./run.sh
```

**Available commands:**
- `r` - Restart Flutter
- `f` - View Flutter logs
- `l` - View Laravel logs
- `q` - View Queue worker logs
- `s` - Status of all services
- `h` - Show help menu
- `x` - Stop all services and exit

### Manual Setup

**Backend (Laravel):**
```bash
cd backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve
```

**Frontend (React):**
```bash
cd frontend
npm install
npm run dev
```

**Admin (Flutter):**
```bash
cd admin
flutter pub get
flutter run
```

## 🔑 Environment Variables

Create `.env` file in backend folder:
```
DB_DATABASE=elkaavie
DB_USERNAME=root
DB_PASSWORD=
APP_KEY=
SANCTUM_STATEFUL_DOMAINS=localhost:3000
```

## 🎨 UI Features

### Admin Panel
- **Dashboard**: Interactive statistics cards with navigation to respective tabs
- **Rooms Management**: Visual indicators for room status (available, unavailable, booked)
- **Bookings**: Collapsible sections for better information organization
- **Users**: Differentiation between admin and regular users with booking history

### Design Principles
- Swiss design with clean typography and ample whitespace
- Clear visual hierarchy and intuitive navigation
- Consistent color coding for status indicators
- Responsive layouts for various screen sizes

## 👨‍💻 Author
- GitHub: [@hashiifabdillah](https://github.com/hashiifab)
- LinkedIn: [Hashiif Abdillah](https://www.linkedin.com/in/hashiif-abdillah-665373297/)