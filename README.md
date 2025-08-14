# Mutual Fund Platform 📊
![Java](https://img.shields.io/badge/Java-8+-blue)
![Spring Boot](https://img.shields.io/badge/SpringBoot-2.5.0-green)
![GitHub repo size](https://img.shields.io/github/repo-size/YourUsername/RepoName)


## Overview 💼

This project allows users to explore mutual funds, make investments, track their portfolio, and perform buy/sell transactions. With secure authentication and a user-friendly interface, investors can seamlessly manage their financial journey.

## Features ✨

#### 🛡 User Authentication
Secure login and registration for investors.

#### 📊 Portfolio Tracking
View investments, transaction history, and current holdings.

#### 💰 Buy/Sell Transactions
Execute transactions with real-time NAV updates.

#### 💵 Wallet Management
Prevent investors from overspending their balance.

#### 📈 Dynamic NAV Computation
Automatic calculation of NAV based on stock prices and weights.


## Installation 🛠

### Prerequisites
- 💻 Java JDK 8+
- 🖥 Spring Tool Suite (STS)
- 🗄 Oracle Database

### Steps to Set Up
- Clone the Repository:  
  `git clone https://github.com/YourUsername/Mutual-Fund-Platform.git`
- Import Project in STS → File → Import → Existing Maven Projects → Select project → Finish
- Configure Database:
  - Update `application.properties`:
    ```properties
    spring.datasource.url=jdbc:oracle:thin:@localhost:1521:orcl
    spring.datasource.username=YOUR_DB_USERNAME
    spring.datasource.password=YOUR_DB_PASSWORD
    ```
- Run Project in STS → Right-click project → Run As → Spring Boot App
- Frontend Setup → Open `Mutual_Fund_Project_Frontend` folder in your preferred editor or live server


## API Endpoints ⚡

### 🛡 User Authentication
- `POST /login` → Investor login
- `POST /register` → Investor registration
- `GET /investors` → List all investors

### 💰 Investments
- `GET /investments` → List all investments
- `POST /investments/add` → Add a new investment
- `GET /investments/id/{investorId}` → Get investments by investor

### 📊 Mutual Funds
- `GET /mutualfunds` → List all mutual funds
- `POST /mutualfund/add` → Add a new mutual fund
- `GET /mutualfunds/id/{mfid}` → Get details of a specific mutual fund

### 📈 Stocks & Fund Composition
- `GET /stocks` → List all stocks
- `POST /stocks/add` → Add a new stock
- `GET /stocksinfund` → View stocks in each mutual fund
- `POST /stocksinfund/add` → Add stock weights to a fund



## Tech Stack 🛠
- **Backend:** Java, Spring Boot, MVC Framework
- **Database:** Oracle SQL, DBeaver, SQL Plus
- **Frontend:** HTML, CSS, JavaScript (or React if used)


## Troubleshooting ⚠️
- **Database Connection Issues:** Ensure Oracle DB is running and credentials in `application.properties` are correct.
- **Maven Dependencies:** Right-click project → Maven → Update Project → select “Force Update of Snapshots/Releases.”
- **Port Conflicts:** Update `server.port` in `application.properties` if the default port is already in use.


## Authors 👤

- [@jasmine-1612](https://github.com/jasmine-1612)
