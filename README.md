# 🌍 Wanderly — Tourist Management System

> **Explore. Plan. Book. Experience.**

Wanderly is a web-based **Tourist Management System** designed to provide travelers with a centralized platform for discovering tourist destinations, exploring hotels, checking transportation options, discovering regional cuisine, and managing travel bookings.

The system combines tourism discovery, accommodation, transportation, food ordering, booking management, and administration into one integrated platform.

---

## 🌐 Project Links

🔗 **GitHub Repository:**
https://github.com/mukesh9342472953/Tourist-Management-System

---

## 📌 Project Overview

Planning a trip often requires using multiple platforms for destinations, hotels, transportation, food, and booking management.

**Wanderly** addresses this problem by bringing these major tourism services together in a single platform.

The system provides two major experiences:

* 👤 **Tourist Portal** – Explore destinations, hotels, transportation, food, and manage bookings.
* 🛠️ **Admin Portal** – Monitor destinations, accommodations, bookings, and tourism-related information.

The project is designed with a responsive frontend and an optional Node.js/Express.js + MySQL backend architecture.

---

# 🎯 Problem Statement

Tourists often depend on different applications and websites for different parts of their journey.

For example:

* One platform for finding destinations
* Another platform for hotels
* Another for transportation
* Different sources for local food
* Separate systems for managing bookings

This creates a fragmented travel-planning experience.

### Main Problems

* ❌ Multiple disconnected tourism services
* ❌ Difficulty managing travel information
* ❌ Separate hotel and transportation searches
* ❌ No centralized booking history
* ❌ Difficulty discovering regional cuisine
* ❌ Lack of centralized tourism administration

---

# 💡 Proposed Solution

Wanderly provides a centralized tourism management platform where users can:

```text
Discover Destinations
        ↓
Explore Hotels
        ↓
Search Transportation
        ↓
Discover Regional Food
        ↓
Add Services / Food to Cart
        ↓
Book Services
        ↓
Manage Bookings
        ↓
View Travel Dashboard
```

Administrators can monitor and manage tourism-related information through the administration interface.

---

# ✨ Key Features

## 👤 Tourist Features

### 🌍 Destination Exploration

Users can explore different tourist destinations and discover places based on their interests.

Features include:

* Historical destinations
* Natural attractions
* Wildlife destinations
* Spiritual destinations
* Tourist attractions
* Destination descriptions
* Destination images
* Image galleries

---

## 🏨 Hotel Management

Users can explore available hotels and accommodation options.

### Features

* Search hotels
* Filter hotels
* View hotel details
* View hotel images
* View room information
* Check pricing
* Select booking dates
* Calculate booking cost
* Confirm reservations

---

## 🚆 Transportation Management

Wanderly provides transportation discovery and booking functionality.

### Supported Categories

* 🚌 Bus
* 🚆 Train
* ✈️ Flight

Users can view:

* Source
* Destination
* Departure time
* Arrival time
* Available seats
* Ticket price
* Transport type

### Transportation Flow

```text
Source
  ↓
Destination
  ↓
Transport Type
  ↓
Available Services
  ↓
Select Service
  ↓
Booking
```

---

# 🍱 Regional Food & Cuisine

Wanderly also focuses on discovering regional Indian cuisine.

Users can explore traditional dishes and food items associated with different regions.

### Features

* Browse regional cuisine
* View food images
* View food descriptions
* View prices
* Add food to cart
* Increase/decrease quantity
* Remove items
* Calculate subtotal
* Calculate tax
* Calculate delivery charges
* Calculate final amount

### Food Ordering Flow

```text
Select Region
      ↓
Explore Food
      ↓
Select Dish
      ↓
Add to Cart
      ↓
Manage Quantity
      ↓
Calculate Total
      ↓
Place Order
```

---

# 🛒 Shopping Cart

The shopping cart allows users to manage selected food items before checkout.

### Cart Features

* Add items
* Remove items
* Increase quantity
* Decrease quantity
* Display item count
* Calculate subtotal
* Calculate tax
* Calculate delivery charges
* Calculate final amount

```text
Item Price × Quantity
        ↓
     Subtotal
        ↓
       Tax
        ↓
Delivery Charge
        ↓
   Final Amount
```

---

# 🔐 User Authentication

Wanderly provides user registration and login functionality.

Users can:

* Register an account
* Login
* Maintain session information
* Access their dashboard
* View booking information

The static frontend uses browser-based persistence for demonstration and GitHub Pages compatibility.

For a production environment, authentication can be extended using secure backend authentication and password hashing.

---

# 👤 Tourist Dashboard

The tourist dashboard provides a centralized view of the user's activities.

### Dashboard Features

* View active bookings
* View hotel reservations
* View transportation bookings
* View food orders
* View booking history
* View user information
* Cancel applicable bookings

### Dashboard Flow

```text
                    TOURIST DASHBOARD
                           │
          ┌────────────────┼────────────────┐
          ↓                ↓                ↓
       Hotels          Transport          Food
          │                │                │
          └────────────────┼────────────────┘
                           ↓
                    Booking History
```

---

# 🛠️ Admin Portal

The administration module allows authorized administrators to monitor tourism-related information.

## 📊 Admin Dashboard

The admin dashboard can provide information such as:

* Total bookings
* Registered users
* Available destinations
* Accommodation information
* Booking information
* Tourism-related statistics

---

## 📍 Destination Management

Administrators can inspect destination information and tourism records.

Possible operations include:

* View destinations
* Review destination information
* Manage destination data
* Monitor attractions

---

## 🏨 Accommodation Management

Administrators can monitor:

* Hotel listings
* Hotel capacity
* Room information
* Pricing
* Accommodation availability

---

## 📋 Booking Management

The booking management module provides centralized monitoring of tourist bookings.

```text
Tourist
   ↓
Service Selection
   ↓
Booking
   ↓
Booking Status
   ↓
Admin Monitoring
```

---

# 🏗️ System Architecture

```text
                    🌍 WANDERLY
              TOURIST MANAGEMENT SYSTEM
                         │
          ┌──────────────┴──────────────┐
          │                             │
       👤 Tourist                    🛠️ Admin
          │                             │
   ┌──────┼──────┐              ┌───────┼───────┐
   ↓      ↓      ↓              ↓       ↓       ↓
Places  Hotels Transport      KPI    Hotels  Bookings
   │      │      │              │       │       │
   └──────┼──────┘              └───────┼───────┘
          ↓                             ↓
        Food                    System Management
          │
          ↓
        Cart
          │
          ↓
       Booking
          │
          ↓
   Tourist Dashboard
          │
          ↓
   Backend REST API
          │
          ↓
       MySQL
```

---

# 🔄 Application Workflow

```text
Start
  ↓
Open Wanderly
  ↓
Register / Login
  ↓
Explore Destinations
  ↓
Select Destination
  ↓
Explore Hotels / Transport / Food
  ↓
Select Required Service
  ↓
Enter Booking Information
  ↓
Calculate Cost
  ↓
Confirm Booking / Order
  ↓
View Dashboard
  ↓
Manage Booking History
```

---

# 🛠️ Technology Stack

## Frontend

| Technology      | Purpose                       |
| --------------- | ----------------------------- |
| HTML5           | Website structure             |
| CSS3            | Styling and responsive design |
| JavaScript ES6+ | Application logic             |
| CSS Grid        | Layout management             |
| Flexbox         | Responsive components         |
| Web Components  | Reusable components           |
| LocalStorage    | Client-side persistence       |

## Backend

| Technology | Purpose                    |
| ---------- | -------------------------- |
| Node.js    | Server runtime             |
| Express.js | REST API framework         |
| MySQL      | Relational database        |
| mysql2     | MySQL connectivity         |
| dotenv     | Environment configuration  |
| CORS       | Cross-origin communication |
| Axios      | HTTP requests              |

---

# 📂 Project Structure

```text
Tourist-Management-System/
│
├── frontend/
│   │
│   ├── index.html
│   ├── wanderly.html
│   │
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   ├── app.js
│   │   ├── indiaPlaces.js
│   │   └── indiaHotels.js
│   │
│   ├── images/
│   │   ├── destinations/
│   │   ├── hotels/
│   │   └── foods/
│   │
│   ├── foods_generated.json
│   ├── hotels_generated_v4.json
│   └── places_generated.json
│
├── backend/
│   │
│   ├── server.js
│   ├── database.sql
│   ├── update_schema.js
│   ├── package.json
│   ├── .env.example
│   │
│   ├── config/
│   │
│   └── routes/
│
├── build_foods.js
├── build_hotels.js
├── build_hotels_v2.js
├── build_hotels_v3.js
├── build_hotels_v4.js
│
├── download_images_retry.js
├── fix_index.js
│
├── replace_dest_slides.js
├── replace_foods.js
├── replace_foods_v2.js
├── replace_hotels_v2.js
├── replace_hotels_v3.js
├── replace_hotels_v4.js
│
├── audit-and-verify-images.cjs
├── audit-food-images.cjs
├── audit-hotel-images.cjs
├── audit-hotels-images.cjs
└── verify-hotel-images.cjs
```

---

# 🗄️ Database Architecture

The backend uses **MySQL** as the relational database.

The system is designed around tourism-related entities such as:

```text
Users
  │
  ├───────────────┐
  │               │
  ↓               ↓
Profiles        Bookings
                   │
       ┌───────────┼───────────┐
       ↓           ↓           ↓
     Hotels     Transport     Food
       │
       ↓
 Destinations
```

### Main Entities

* Users
* Places / Destinations
* Hotels
* Transportation
* Bookings
* Food Orders

---

# 🔌 Backend API Structure

The backend follows a REST-style API architecture.

```text
/api
 │
 ├── /users
 │
 ├── /places
 │
 ├── /hotels
 │
 ├── /transport
 │
 ├── /booking
 │
 └── /food-order
```

### Example Booking Flow

```text
Frontend
   │
   │ POST /api/booking
   ↓
Express Server
   ↓
API Route
   ↓
Database Operation
   ↓
MySQL
   ↓
Booking Response
   ↓
Frontend Dashboard
```

---

# 🔄 Data Flow

## Hotel Booking

```text
Select Hotel
     ↓
Select Dates
     ↓
Calculate Nights
     ↓
Calculate Total
     ↓
Confirm Booking
     ↓
Backend API
     ↓
MySQL Database
     ↓
Booking Confirmation
```

## Food Ordering

```text
Browse Food
     ↓
Select Dish
     ↓
Add to Cart
     ↓
Modify Quantity
     ↓
Calculate Bill
     ↓
Place Order
```

## Transport Booking

```text
Source
  ↓
Destination
  ↓
Transport Type
  ↓
Search
  ↓
Select Service
  ↓
Check Availability
  ↓
Booking
```

---

# 🚀 Installation

## 1. Clone the Repository

```bash
git clone https://github.com/mukesh9342472953/Tourist-Management-System.git
```

Navigate into the project:

```bash
cd Tourist-Management-System
```

---

# 🌐 2. Run Frontend

The frontend does not require a build tool.

### Using VS Code Live Server

Open:

```text
frontend/index.html
```

Then:

```text
Right Click → Open with Live Server
```

---

### Using Python

From the project root:

```bash
python -m http.server 3000
```

Open:

```text
http://localhost:3000
```

or:

```text
http://localhost:3000/frontend/
```

---

# ⚙️ 3. Setup Backend

Navigate to the backend:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file using `.env.example`.

Example:

```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=tourist_db
DB_PORT=3306
PORT=5000
```

---

# 🗄️ 4. Setup MySQL Database

Open MySQL and create the database:

```sql
CREATE DATABASE tourist_db;
```

Select the database:

```sql
USE tourist_db;
```

Import the database schema:

```bash
mysql -u root -p tourist_db < database.sql
```

You can also open:

```text
backend/database.sql
```

using MySQL Workbench and execute the SQL script.

---

# ▶️ 5. Start Backend

Inside the `backend` folder:

```bash
node server.js
```

The backend will run on:

```text
http://localhost:5000
```

---

# 🌐 GitHub Pages Deployment

The frontend can be deployed as a static website using GitHub Pages.

### Deployment Flow

```text
GitHub Repository
       ↓
GitHub Pages
       ↓
Static Frontend
       ↓
Public Website
```

### Steps

1. Open your GitHub repository.
2. Go to **Settings**.
3. Open **Pages**.
4. Select the required deployment source.
5. Deploy the frontend.
6. Open the generated GitHub Pages URL.

> GitHub Pages hosts the frontend only. The Node.js backend and MySQL database require separate server/cloud hosting.

---

# 🧪 Testing

The application should be tested across the following areas.

### Functional Testing

* User registration
* User login
* Destination browsing
* Hotel search
* Hotel booking
* Transport search
* Transport booking
* Food browsing
* Cart operations
* Food ordering
* Dashboard
* Admin functions

### UI Testing

* Desktop responsiveness
* Tablet responsiveness
* Mobile responsiveness
* Navigation
* Forms
* Modals
* Images
* Buttons
* Cards

### Browser Testing

Test the application using:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox

Open browser developer tools:

```text
F12 → Console
```

and verify that the application runs without unexpected JavaScript errors.

---

# 🔐 Security Considerations

For production deployment, the following security improvements should be implemented:

* Password hashing
* Secure authentication
* JWT/session management
* Server-side validation
* SQL injection protection
* Rate limiting
* HTTPS
* Secure HTTP headers
* Role-based access control
* Environment-based secrets
* Database backups

> Never upload real passwords, API keys, or database credentials to GitHub.

---

# 📈 Advantages

### For Tourists

* 🌍 Centralized travel platform
* 🏨 Hotel discovery
* 🚆 Transportation search
* 🍱 Regional food discovery
* 🛒 Integrated cart
* 📋 Booking management
* 👤 Tourist dashboard

### For Administrators

* 📊 Centralized monitoring
* 🏨 Accommodation management
* 📍 Destination management
* 📋 Booking management
* 📈 Tourism information management

### For Developers

* Modular architecture
* Separate frontend/backend
* MySQL database integration
* Reusable datasets
* REST API structure
* Easy deployment
* Expandable architecture

---

# ⚠️ Current Limitations

The current project is primarily designed as an academic/project implementation and can be further extended for production use.

Current limitations may include:

* Some tourism data is locally stored.
* Static frontend persistence uses browser storage.
* Live hotel inventory is not connected to external hotel providers.
* Live transportation APIs are not integrated.
* Production payment gateway is not integrated.
* Real-time weather service is not currently integrated.

---

# 🔮 Future Enhancements

## 🤖 AI-Powered Travel Planner

A future version can generate personalized itineraries based on:

* Budget
* Number of days
* Interests
* Destination preferences
* Travel style

```text
User Preferences
       ↓
AI Recommendation
       ↓
Destinations
       ↓
Hotels
       ↓
Transportation
       ↓
Food
       ↓
Personalized Itinerary
```

---

## 🗺️ Interactive Maps

Future versions can integrate:

* Leaflet
* Mapbox
* Google Maps

Possible features:

* Tourist location mapping
* Hotel locations
* Nearby attractions
* Route planning
* Distance calculation

---

## 🌦️ Weather Integration

Weather APIs can be integrated to provide destination forecasts based on travel dates.

```text
Destination + Travel Date
          ↓
      Weather API
          ↓
       Forecast
```

---

## 💳 Payment Gateway

Future versions can integrate payment gateways such as:

* Razorpay
* Stripe

for secure online booking payments.

---

## ⭐ Reviews & Ratings

Users can be allowed to:

* Rate hotels
* Review destinations
* Review food
* Share travel experiences
* Upload travel photographs

---

## 🔔 Notifications

Future notification features may include:

* Booking confirmation
* Booking reminders
* Cancellation alerts
* Travel reminders
* Promotional notifications

---

## 📱 Mobile Application

The platform can eventually be extended into a mobile application.

```text
              Wanderly
                 │
       ┌─────────┴─────────┐
       ↓                   ↓
   Web Application    Mobile Application
       │                   │
       └─────────┬─────────┘
                 ↓
          Shared Backend API
                 ↓
             MySQL DB
```

---

# 📊 Project Modules

| Module           | Description                         |
| ---------------- | ----------------------------------- |
| Authentication   | User registration and login         |
| Destinations     | Explore tourist destinations        |
| Hotels           | Accommodation discovery and booking |
| Transportation   | Bus, train and flight services      |
| Food             | Regional cuisine discovery          |
| Cart             | Manage selected food items          |
| Booking          | Manage reservations                 |
| Dashboard        | View tourist activities             |
| Admin            | Manage tourism information          |
| Database         | Store application data              |
| Asset Management | Manage tourism images and datasets  |

---

# 🎓 Learning Outcomes

Through this project, the development team gains practical experience in:

* HTML5
* CSS3
* JavaScript
* Responsive web design
* Client-side state management
* LocalStorage
* Node.js
* Express.js
* REST API development
* MySQL
* Database design
* CRUD operations
* Authentication
* Git & GitHub
* GitHub Pages deployment
* Full-stack application architecture

---

# 🚀 Development Roadmap

```text
Phase 1
Tourism Website
       ↓
Phase 2
Interactive Booking System
       ↓
Phase 3
Node.js + Express Backend
       ↓
Phase 4
MySQL Database Integration
       ↓
Phase 5
Payment Integration
       ↓
Phase 6
Maps + Weather APIs
       ↓
Phase 7
AI Travel Planner
       ↓
Phase 8
Mobile Application
```

---

# 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for more information.

---

# 👨‍💻 Author

### Mukesh B.N.

**Computer Science and Engineering Student**

🔗 GitHub:
https://github.com/mukesh9342472953

🔗 Project Repository:
https://github.com/mukesh9342472953/Tourist-Management-System

---

# 🌍 Wanderly

> **Explore More. Plan Better. Travel Smarter.**

**Wanderly — A centralized Tourist Management System connecting destinations, hotels, transportation, regional cuisine, bookings, and tourism management in one platform.**
