# Student Marketplace

Student Marketplace is a marketplace app for buying and selling used textbooks between students. It was built as a university project, with the aim of solving a problem most of us have run into directly: paying full price for textbooks that get used for one semester and then sit on a shelf.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Screenshots](#screenshots)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
  - [Running the App](#running-the-app)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Team](#team)
- [Contributing](#contributing)
- [License](#license)

## About the Project

Student Marketplace gives students a way to buy, sell, and trade used textbooks (and other study materials) directly with each other, instead of relying on bookstores or generic resale sites with no relevance to their courses.

The app is built around two core parts: a marketplace for listings, and a notifications system that keeps students informed about new listings, price changes, and messages without needing to check the app constantly.

The project doubles as a learning exercise for our team — working with a real codebase, collaborating through Git, and taking a product from planning through to a working build.

## Features

**Marketplace**

Students can list textbooks and other study materials with a title, course code, condition, price, and photos. Listings can be browsed or searched by course, subject, or keyword, and filtered by price, condition, or campus. Buyers can save listings they're interested in and contact sellers directly to arrange a sale.

**Notifications**

Students get notified when a new listing matches something they're searching for, when a saved item drops in price, or when they receive a message from a buyer or seller. The system is also used for general announcements and app updates.

**Accounts**

Sign-up is restricted to verified university email addresses. Each user has a profile with their listing history and reviews from past transactions.

## Tech Stack

The stack below reflects our current setup — update as the project evolves.

| Layer | Technology |
|---|---|
| Frontend | React / React Native |
| Backend | Spring Boot |
| Database | mySQL|
| Auth | Supabase |
| Notifications | Firebase Cloud Messaging / WebSockets / OneSignal |
| Hosting | Vercel |
| Version Control | Git and GitHub |

## Screenshots

Screenshots and a short demo will be added here once the UI is further along.

## Getting Started

These steps will get a local copy of the project running for development.

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later)
- npm, yarn, or pnpm
- Git
- A local or cloud database instance (PostgreSQL or MongoDB)

### Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

Install dependencies:

```bash
npm install
```

### Environment Variables

Create a `.env` file in the root directory:

```env
DATABASE_URL=your_database_connection_string
JWT_SECRET=your_jwt_secret
NOTIFICATIONS_API_KEY=your_notifications_service_key
PORT=3000
```

The `.env` file should never be committed — it's already listed in `.gitignore`.

### Running the App

```bash
npm run dev
```

The app runs at `http://localhost:3000` by default.

To run tests:

```bash
npm test
```

## Project Structure

```
student marketplace/
├── src/
│   ├── components/     # Reusable UI components
│   ├── pages/          # App pages and screens
│   ├── routes/         # API routes
│   ├── controllers/    # Request handlers and business logic
│   ├── models/         # Database models and schemas
│   ├── services/       # Notifications, auth, and other services
│   ├── utils/          # Helper functions
│   └── App.js
├── public/             # Static assets
├── tests/              # Unit and integration tests
├── .env.example
├── package.json
└── README.md
```

This will be updated as the folder structure is finalised.

## Usage

1. Sign up with a university email
2. Browse listings by subject or course code, or search by title
3. Post a textbook for sale with photos, price, and condition
4. Save searches or favourite listings to get notified of matches and price drops
5. Message a seller directly to arrange the exchange

## Roadmap

- [ ] User authentication with university email verification
- [ ] Marketplace listing creation, browsing, and search
- [ ] Real-time notifications system
- [ ] In-app messaging between buyers and sellers
- [ ] Ratings and reviews for users
- [ ] Mobile app version
- [ ] Payment integration (stretch goal)

Full list of proposed features and known issues in [Issues](../../issues).

## Team

| Name | Role | GitHub |
|---|---|---|
| Luke Zyster | Frontend / Team Lead | [@username](https://github.com/LukeZyster) |
| Isaac Ziyengwa | Backend | [@username](https://github.com/keepin-it-eazy) |
| Nuyra Swanson | Database / DevOps | [@username](https://github.com/NuyraSwanson) |
| Jada Rinquest | Frontend / UI/UX Design | [@username](https://github.com/Jada-Rinquest) |
| Rocco Visagie | UI/UX Design | [@username](https://github.com/RGV-Code) |
| Ayren Villet | UI/UX Design | [@username](https://github.com/Ayren-Villet) |
| Joshua Bonzet | Backend / UI/UX Design | [@username](https://github.com/Kultur26) |



## Contributing

1. Create a new branch: `git checkout -b feature/your-feature-name`
2. Commit your changes: `git commit -m "Add: your feature description"`
3. Push the branch: `git push origin feature/your-feature-name`
4. Open a pull request

Please follow the existing code style and keep commit messages clear.

## License

This project was built for a university course. If it's made public or open source later, a license (e.g. MIT) will be added here.
