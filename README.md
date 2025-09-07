# Vegan Social Platform - `Pulipdang`

🇺🇸 English | [🇰🇷 한국어](README.ko.md)

A comprehensive vegan community platform that connects vegan enthusiasts through social feeds, cafe reservations, group activities, and community discussions.

## 📝 Project Overview

**Purpose**: Create a dedicated social platform for vegans to share experiences, discover vegan-friendly cafes, organize meetups, and engage in community discussions

**Target Users**: Vegan community members seeking connection, information, and shared experiences

**Core Features**:
- **User Login** → Secure account creation and login for personalized user experience
- **Vegan Feed** → SNS-style sharing of vegan experiences and lifestyle content
- **Cafe Reservation** → Discover and book vegan dessert cafes in Seoul
- **Group Activities** → Organize and participate in vegan-centered meetups
- **Community Board** → Open discussion forum for vegan topics

## 🔧 Technology Stack

### 🛠️ Backend
- **Language**: Java
- **Framework**: Spring Boot
- **ORM**: MyBatis for database integration and mapper configuration
- **Architecture**: MVC pattern with layered service architecture

### 🎨 Frontend
- **Core Technologies**: HTML5, CSS3, JavaScript
- **UI/UX**: Responsive web design with modern styling
- **Template Engine**: Thymeleaf for server-side rendering

### 🗄️ Database
- **Primary Database**: MySQL for data storage and management
- **Data Modeling**: Relational database design with normalized structure

### ⚙️ Development Tools
- **Version Control**: GitHub for collaboration and code repository
- **IDE**: IntelliJ IDEA for backend development environment
- **Build Tool**: Gradle for dependency management and build automation

## 📁 Project Structure

```
vegan-social-platform/
├── src/main/java/com/playdata/miniproject/
│   ├── board/                    # Board functionality
│   │   ├── controller/          # Board controllers
│   │   ├── dao/                 # Data access objects
│   │   ├── dto/                 # Data transfer objects
│   │   ├── mapper/              # MyBatis mappers
│   │   └── service/             # Business logic services
│   ├── cafe/                    # Cafe reservation system
│   │   ├── controller/          # Cafe controllers
│   │   ├── dao/                 # Cafe data access
│   │   ├── dto/                 # Cafe DTOs
│   │   ├── mapper/              # Cafe mappers
│   │   └── service/             # Cafe services
│   ├── community/               # Group community features
│   │   ├── controller/          # Community controllers
│   │   ├── dao/                 # Community data access
│   │   ├── dto/                 # Community DTOs
│   │   ├── mapper/              # Community mappers
│   │   └── service/             # Community services
│   ├── feed/                    # Social feed functionality
│   │   ├── controller/          # Feed controllers
│   │   ├── dao/                 # Feed data access
│   │   ├── dto/                 # Feed DTOs
│   │   ├── mapper/              # Feed mappers
│   │   └── service/             # Feed services
│   ├── user/                    # User management
│   │   ├── controller/          # User controllers
│   │   ├── dao/                 # User data access
│   │   ├── dto/                 # User DTOs
│   │   ├── mapper/              # User mappers
│   │   └── service/             # User services
│   ├── config/                  # Configuration classes
│   └── util/                    # Utility classes
├── src/main/resources/
│   ├── mappers/                 # MyBatis XML mappers
│   ├── static/                  # Static web resources
│   │   ├── css/                 # Stylesheets
│   │   ├── js/                  # JavaScript files
│   │   └── images/              # Image assets
│   └── templates/               # Thymeleaf templates
└── build.gradle                # Build configuration
```

## 🌟 Core Features

### 1. User Authentication & Profile Management
![User Pages](images/User_page_1.png)

- Secure user registration and login system
- Personalized user profiles with vegan preferences
- Account management and privacy settings

### 2. Vegan Social Feed
![Feed Pages](images/Feed_page_1.jpg)

- Share vegan lifestyle experiences and recipes
- Photo and text-based posts with social interactions
- Community engagement through likes and comments
- Personal feed management and content curation

### 3. Vegan Cafe Discovery & Reservation
![Cafe & Reservation](images/C&R_page_1.png)

- Comprehensive directory of vegan dessert cafes in Seoul
- Real-time reservation system with availability checking
- Cafe information including menus, locations, and reviews
- Integrated booking management for users

### 4. Community Groups & Meetups
![Group Pages](images/Group_page_1.png)

- Create and join vegan-focused interest groups
- Organize local meetups and events
- Group discussion boards and activity planning
- Member management and participation tracking

### 5. Discussion Board
![Board Pages](images/Board_page_1.png)

- Open forum for vegan-related discussions
- Topic categorization and search functionality
- User-generated content with moderation features
- Knowledge sharing and community support

## 🚀 Getting Started

### Prerequisites
- Java 11 or higher
- MySQL 8.0+
- Gradle 7.0+
- IntelliJ IDEA (recommended)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd vegan-social-platform
```

2. Configure database settings:
```bash
# Update application.properties with your MySQL configuration
cp src/main/resources/application.properties.example src/main/resources/application.properties
```

3. Build and run the application:
```bash
./gradlew bootRun
```

4. Access the application:
```
http://localhost:8080
```

## 👥 Team Members

[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/YunSHCode) **Yun Seong Hun** - Full-stack Development (Board/Community)  
[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/nao0963) **Kim Sun Young** - Database Design & Backend Development(User)  
[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/05Daul) **Kim Da Ul** - Frontend Development & Integration (Cafe)  
[<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/netioz) **Kim Min Ji** - Frontend Development & UI/UX (Feed)

## 📊 Database Design

### Entity-Relationship Diagram
<img src="src/main/resources/static/images/ERD.png" alt="ERD Diagram" width="80%">

The database design supports:
- User authentication and profile management
- Content creation and social interactions
- Reservation system with temporal data
- Group membership and activity tracking

## 📋 Documentation

### Project Specifications
- [Feature Specifications](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=1791406220#gid=1791406220)
- [Requirements Specifications](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=1670477596#gid=1670477596)

### Testing Results
- [Frontend Test Results](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=1518302369#gid=1518302369)
- [Backend Test Results](https://docs.google.com/spreadsheets/d/1VlRIEm97TF-sAsTUuvemY0y4OFjPHJ-vdtcl8LMIWGc/edit?gid=475843754#gid=475843754)

## ✨ Technical Highlights

### Architecture Design
- **MVC Pattern**: Clean separation of concerns with controller, service, and data access layers
- **RESTful APIs**: Standardized HTTP endpoints for frontend-backend communication
- **Responsive Design**: Mobile-first approach ensuring cross-device compatibility

### Security Features
- User authentication and session management
- Input validation and SQL injection prevention
- Secure file upload handling for user-generated content

### Performance Optimization
- Database query optimization with MyBatis
- Static resource caching and compression
- Efficient image handling and storage

## 🔮 Future Enhancements

- **Mobile Application**: Native iOS and Android apps
- **Real-time Notifications**: Push notifications for community activities
- **Advanced Search**: AI-powered content discovery and recommendations
- **Integration APIs**: Third-party vegan restaurant and product databases
- **Internationalization**: Multi-language support for global vegan community

---

*This team project was created to practice the basics of web development using Java Spring Boot.*
