# Itihaas - Indian Heritage Tourism Platform

<img width="1901" height="902" alt="image" src="https://github.com/user-attachments/assets/170aa44e-c2e0-44f9-8c0e-a3006ab88f66" />

## 🌟 Overview

<img width="1906" height="904" alt="image" src="https://github.com/user-attachments/assets/779bf5ba-9a80-4c41-bb87-a19b6187a5ed" />

Itihaas is a comprehensive Indian heritage tourism platform that connects travelers with India's rich cultural heritage, monuments, and historical sites. The platform offers guided tours, merchandise, interactive maps, and a unique reward system to enhance the tourism experience.

## 🏛️ Features

<img width="1907" height="910" alt="image" src="https://github.com/user-attachments/assets/f135d1fe-3675-40aa-ae11-972a24f9035c" />
<img width="1916" height="909" alt="image" src="https://github.com/user-attachments/assets/e70d3c62-b615-42b4-8e23-5bb6cbd07013" />
<img width="1913" height="906" alt="image" src="https://github.com/user-attachments/assets/d6c6c976-bece-4004-9613-6ce636f71e5c" />
<img width="1919" height="913" alt="image" src="https://github.com/user-attachments/assets/0df6c18e-2dfd-4d50-885f-436b11aebd12" />
<img width="1915" height="903" alt="image" src="https://github.com/user-attachments/assets/23150275-d356-4058-aff6-6f883b8b99e8" />

## Done by
<img width="1915" height="903" alt="image" src="project/website/static/team/cto.jpg" />

### Core Features
- **Interactive Heritage Map**: Explore UNESCO World Heritage sites and monuments across India
- **Guided Tours**: Connect with certified tour guides for personalized experiences
- **Booking System**: Reserve visits to monuments and heritage sites
- **Multilingual Support**: Available in English and Hindi
- **User Reviews & Ratings**: Share experiences and read reviews from other travelers
- **News Integration**: Stay updated with latest heritage and tourism news

### E-commerce Features
- **Heritage Merchandise**: Shop for traditional Indian clothing and souvenirs
- **Shopping Cart**: Add items and manage your shopping experience
- **Order Management**: Track orders and view order history
- **Payment Integration**: Secure payment processing

### User Management
- **User Registration & Authentication**: Secure login system with email verification
- **Profile Management**: Upload profile pictures and manage personal information
- **Guide Registration**: Special registration for tour guides
- **Admin Dashboard**: Comprehensive admin panel for platform management

### Interactive Features
- **AI Chatbot**: Get instant assistance and information about heritage sites
- **WhatsApp Integration**: Receive booking confirmations via WhatsApp
- **Automated Messaging**: Scheduled notifications and updates
- **Itihaas Coins**: Reward system for user engagement and activities

### Content Features
- **Festival Calendar**: Discover festivals and celebrations across India
- **Video Content**: Educational videos about heritage sites
- **Photo Galleries**: Visual exploration of monuments and sites
- **Audio Narration**: Guided audio tours for monuments

## 🛠️ Technology Stack

### Backend
- **Flask**: Python web framework
- **SQLAlchemy**: Database ORM
- **Flask-Login**: User authentication
- **Flask-WTF**: Form handling and CSRF protection
- **Flask-Babel**: Internationalization support

### Frontend
- **HTML5/CSS3**: Modern responsive design
- **JavaScript**: Interactive user experience
- **Bootstrap**: UI framework for responsive layouts

### External APIs
- **Google Maps API**: Interactive mapping and location services
- **GNews API**: Real-time news integration
- **WhatsApp Business API**: Messaging integration

### Database
- **SQLite**: Development database
- **SQLAlchemy**: Database management and migrations

## 📦 Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)
- Git

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd itihaas
   ```

2. **Navigate to the project directory**
   ```bash
   cd project
   ```

3. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```

4. **Activate the virtual environment**
   ```bash
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

5. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

6. **Set up environment variables**
   Create a `.env` file in the project directory with the following variables:
   ```env
   FLASK_APP=main.py
   FLASK_ENV=development
   SECRET_KEY=your-secret-key-here
   EMAIL_USER=your-email@gmail.com
   EMAIL_PASSWORD=your-app-password
   GOOGLE_MAPS_API_KEY=your-google-maps-api-key
   GNEWS_API_KEY=your-gnews-api-key
   ```

7. **Initialize the database**
   ```bash
   python main.py
   ```

8. **Run the application**
   ```bash
   flask run
   ```

The application will be available at `http://localhost:5000`

## 🗂️ Project Structure

```
itihaas/
├── project/
│   ├── main.py                 # Application entry point
│   ├── config.py              # Configuration settings
│   ├── requirements.txt       # Python dependencies
│   ├── models.py             # Database models
│   └── website/
│       ├── __init__.py       # Flask app factory
│       ├── views.py          # Main route handlers
│       ├── auth.py           # Authentication routes
│       ├── merchandise.py    # E-commerce functionality
│       ├── chatbot.py        # AI chatbot integration
│       ├── whatsapp.py       # WhatsApp messaging
│       ├── automated_messaging.py  # Automated notifications
│       ├── models.py         # Database models
│       ├── merchandise_models.py   # E-commerce models
│       ├── static/           # Static files (CSS, JS, images)
│       └── templates/        # HTML templates
└── README.md
```

## 🚀 Key Features Explained

### Interactive Map
- Explore heritage sites across India
- Filter by categories (temples, forts, palaces, etc.)
- Get detailed information about each site
- View location coordinates and directions

### Booking System
- Reserve visits to monuments
- Select preferred dates and times
- Choose number of visitors
- Receive confirmation via email and WhatsApp

### Guide Management
- Certified guides can register on the platform
- Users can browse and book guides
- Guide profiles with experience and specializations
- Rating and review system for guides

### Merchandise Shop
- Traditional Indian clothing and accessories
- Secure shopping cart functionality
- Order tracking and history
- Multiple payment options

### Itihaas Coins
- Earn coins for various activities
- Redeem coins for discounts and rewards
- Track coin balance and transaction history

## 🔧 Configuration

### Environment Variables
- `SECRET_KEY`: Flask secret key for session management
- `EMAIL_USER`: Gmail address for sending emails
- `EMAIL_PASSWORD`: Gmail app password
- `GOOGLE_MAPS_API_KEY`: Google Maps API key
- `GNEWS_API_KEY`: GNews API key for news integration

### Database Configuration
The application uses SQLite by default for development. For production, you can configure other databases like PostgreSQL or MySQL.

## 📱 API Endpoints

### Authentication
- `POST /sign-up`: User registration
- `POST /login`: User login
- `POST /logout`: User logout
- `POST /verify-email`: Email verification

### Tours & Bookings
- `GET /index`: Heritage sites listing
- `POST /book`: Create new booking
- `GET /booking-history`: View booking history
- `POST /guide-signup`: Guide registration

### Merchandise
- `GET /shop`: Product catalog
- `GET /product/<id>`: Product details
- `POST /add-to-cart`: Add to shopping cart
- `POST /checkout`: Process order

### Reviews & Ratings
- `GET /review`: View all reviews
- `POST /api/reviews`: Submit new review

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Team

- **CEO**: Project leadership and strategy
- **CTO**: Technical architecture and development
- **CRO**: Revenue optimization and business development
- **Curator**: Content management and heritage expertise

## 📞 Support

For support and queries:
- Email: itihaasdairy@gmail.com
- Website: [Itihaas Platform](http://localhost:5000)

## 🔮 Future Enhancements

- Mobile app development
- Virtual reality tours
- Advanced AI recommendations
- Social media integration
- Multi-language support expansion
- Advanced analytics dashboard

---

**Itihaas** - Preserving India's Heritage, One Journey at a Time 🇮🇳
