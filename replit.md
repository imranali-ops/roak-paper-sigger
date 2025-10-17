# Modern Banking System - Java OOP Project

## Overview
A comprehensive Banking System web application built with Java backend using Object-Oriented Programming principles and modern web technologies for the frontend. This project demonstrates core OOP concepts including inheritance, polymorphism, encapsulation, and abstraction.

## Project Structure

### Backend (Java)
- **Models Package** (`src/main/java/models/`)
  - `Account.java` - Abstract base class for all account types
  - `SavingsAccount.java` - Savings account with interest calculation
  - `CurrentAccount.java` - Current account with overdraft facility
  - `FixedDepositAccount.java` - Fixed deposit with maturity system
  - `Customer.java` - Customer entity with multiple accounts
  - `Transaction.java` - Transaction records
  - `Loan.java` - Loan management with EMI calculation
  - `Card.java` - Credit/Debit card management

- **Services Package** (`src/main/java/services/`)
  - `BankingService.java` - Core banking operations service (Singleton pattern)

- **Main Application** (`src/main/java/Main.java`)
  - Spark Framework web server
  - RESTful API endpoints
  - JSON data serialization with Gson

### Frontend
- **HTML** (`src/main/resources/public/index.html`) - Structure
- **CSS** (`src/main/resources/public/style.css`) - Modern gradient UI design
- **JavaScript** (`src/main/resources/public/script.js`) - Interactive functionality

## Features

### Core Banking Features
1. **Account Management**
   - Multiple account types (Savings, Current, Fixed Deposit)
   - Account creation and management
   - Real-time balance updates

2. **Transactions**
   - Money deposit and withdrawal
   - Inter-account transfers
   - Transaction history tracking

3. **Loan Services**
   - Multiple loan types (Home, Car, Personal, Education)
   - EMI calculation
   - Interest rate management
   - Loan payment tracking

4. **Card Management**
   - Credit and Debit card issuance
   - Card details management
   - Credit limit tracking

5. **Bill Payments**
   - Electricity, Water, Gas bills
   - Internet and Mobile recharge
   - Payment from account

### Advanced Features
- User Authentication (Login/Register)
- Dashboard with account overview
- Quick action buttons
- Transaction filtering by account
- Real-time data updates
- Responsive design
- Beautiful gradient UI

### Demo Account
- **Username:** demo
- **Password:** demo123
- Pre-loaded with sample data for testing

## OOP Concepts Demonstrated

### 1. Inheritance
- `Account` (Abstract Base Class)
  - `SavingsAccount` extends Account
  - `CurrentAccount` extends Account
  - `FixedDepositAccount` extends Account

### 2. Polymorphism
- Method overriding: `deposit()` and `withdraw()` methods
- Different behavior for different account types

### 3. Encapsulation
- Private fields with public getters
- Data hiding and access control
- Package-level organization

### 4. Abstraction
- Abstract `Account` class
- Interface-like service patterns

### 5. Design Patterns
- Singleton Pattern (BankingService)
- Service Layer Pattern
- MVC-like architecture

## Technology Stack

### Backend
- **Java 11** - Programming language
- **Maven** - Build and dependency management
- **Spark Framework 2.9.4** - Web framework
- **Gson 2.10.1** - JSON serialization
- **SLF4J** - Logging

### Frontend
- **HTML5** - Structure
- **CSS3** - Styling with gradients and animations
- **JavaScript (ES6+)** - Client-side logic
- **Font Awesome 6.4.0** - Icons

## API Endpoints

### Authentication
- `POST /api/login` - User login
- `POST /api/register` - User registration

### Banking Operations
- `POST /api/deposit` - Deposit money
- `POST /api/withdraw` - Withdraw money
- `POST /api/transfer` - Transfer between accounts
- `GET /api/transactions/:accountNumber` - Get transaction history

### Advanced Services
- `POST /api/apply-loan` - Apply for loan
- `POST /api/pay-bill` - Pay utility bills
- `POST /api/issue-card` - Request new card

## Running the Application

The application runs on port 5000 and is accessible at:
```
http://localhost:5000
```

### Build Command
```bash
mvn clean compile exec:java -Dexec.mainClass="Main"
```

## Project Highlights

✅ Complete OOP implementation with inheritance hierarchy  
✅ RESTful API architecture  
✅ Modern, responsive UI design  
✅ Multiple account type support  
✅ Advanced banking features (loans, cards, bills)  
✅ Transaction tracking and history  
✅ Real-time data updates  
✅ Demo data for easy testing  

## Development Notes

### Date: October 14, 2025
- Initial project setup with Java 11
- Implemented complete banking system with OOP principles
- Created modern web interface with beautiful UI/UX
- Added advanced features for comprehensive banking experience
- Fixed transfer validation (prevents same-account transfers)
- Added proper error messages with better UX
- Implemented backend rehydration for state consistency
- **Enhanced UI Design:**
  - Modern gradient backgrounds with animated patterns
  - Smooth animations and transitions (fade-in, slide-in, hover effects)
  - Glass morphism and depth effects with shadows
  - Beautiful card designs with 3D hover animations
  - Improved typography and spacing
  - Better color palette with gradient accents
  - Responsive design for all devices
  - Custom scrollbar styling
  - Professional button and input designs
- Perfect for Object-Oriented Programming course project demonstration

## Future Enhancements (Optional)
- Database integration (PostgreSQL/MySQL)
- Email notifications
- PDF statement generation
- Multi-currency support
- 2FA authentication
- Mobile app support
