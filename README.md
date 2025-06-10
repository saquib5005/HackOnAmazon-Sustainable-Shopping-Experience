# HackOnAmazon-Amazon Sustainable Shopping Experience

<div align="center">
  
  ![Screenshot 2025-06-10 090944](https://github.com/user-attachments/assets/00688e6c-3344-414e-8f89-891546aa23de)
  <br>
  <h3>AI-powered eco-friendly shopping experience</h3>
  <p>Developed for the HackOnAmazon Challenge</p>
  
  <p>
    <a href="#✨ Features">Features</a> •
    <a href="#installation">Installation</a> •
    <a href="#usage">Usage</a> •
    <a href="#architecture">Architecture</a> •
    <a href="#tech-stack">Tech Stack</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#license">License</a>
  </p>
</div>

## 🌱 Overview

Amazon Sustainable Shopping Experience is an AI-powered solution that recommends eco-friendly products and provides a dedicated green store with optimum product grading. The platform creates customer dashboards showing their contribution to carbon footprint reduction and includes features for sustainable packaging choices and group buying to reduce environmental impact.

This project was developed as part of the HackOnAmazon challenge to address the theme of "Sustainable Shopping Experience."

## ✨ Features

### 🔍 Eco-Friendly Recommendations
- Smart product recommendations with green scores
- Side-by-side comparison with conventional products
- Environmental impact preview for each product
- "This saves X kg of CO₂" indicators
- Real-time nudges suggesting eco-friendly swaps based on browsing behavior
- Interactive product detail pages with eco-alternative suggestions

### 💰 Carbon vs. Cash Comparison
- See how much CO₂ you save compared to the cost
- Example: "This bamboo toothbrush costs ₹100 more but saves ₹500 in environmental cleanup costs"
- Detailed breakdown of environmental savings
- Collective impact visualization (e.g., "If 1,000 shoppers do this...")

### 🚚 Delivery Impact Information
- Compare environmental impact of different delivery speeds (1-day vs. standard)
- CO₂ emissions visualization for each delivery option
- Nudges toward lower-impact delivery choices
- Consolidated delivery options to reduce packaging waste

### 🏷️ Carbon Footprint Transparency
- Calculated carbon footprint displayed for each product
- Interactive carbon labels with detailed information
- NLP-driven chatbot for answering carbon footprint questions
- Methodology explanations for carbon calculations

### 🌍 EcoImpact Universe Dashboard
- Personal carbon footprint reduction tracking
- "Planet Guardian" gamification system
- Progress toward sustainability challenges
- Regional and global impact visualization
- "Hero Stats" (CO₂ saved, plastic avoided, Planet Points)
- Global Impact Simulations ("If Everyone Did This…")
- Future Projections ("Time Travel Vision")
- Hyper-Local Stats & Impact ("Local Hero")
- Interactive "Eco-Adventure Map" showing impact locations
- "Sustainability Milestones" (Badges, Certificates)
- "Quick Wins" suggestions for next eco-actions

### 🛒 Green Store
- Curated eco-friendly products across categories
- Product grading based on sustainability metrics
- Vendor registration for eco-friendly sellers
- Pagination with 500+ sustainable products
- Eco-filtering & badging in search results
- Category-based browsing of eco-products

### 👥 Group Buying
- Collective purchasing to reduce packaging and shipping emissions
- Group discounts for sustainable choices (10% over 3000rs for groups ≥ 7 people)
- Community-driven sustainability goals
- Location-based matching (within 2km radius)
- Group shopping referral program
- Collective impact tracking (virtual garden, leaderboards)
- Tiered rewards and charity components for group achievements
- Community Expeditions funded by group tokens

### 📦 Sustainable Packaging
- Options for eco-friendly packaging during checkout
- Packaging impact calculator
- Reduced packaging incentives
- Visualization of packaging waste reduction

### 💳 Carbon Credit System
- Earn carbon credits through sustainable purchases
- Redeem credits for discounts on products or Prime membership
- Carbon credit management in user profile
- Apply credits during checkout process

### 🏆 Sustainability Rewards
- "Unlock Real-World Expeditions" with sustainability tokens
- Virtual expeditions to conservation sites (Amazon Rainforest Trek, Coral Reef Dive, Polar Bear Sanctuary)
- NFT badges for sustainability achievements
- 3D maps of conservation areas you've helped fund

### 💹 Smart Eco-Budget
- Personal "Monthly Eco-Allowance" management
- Smart offset options if you exceed your eco-budget
- Tailored discounts/swaps based on shopping behavior
- Helpful hints/tips for staying within an eco-budget

### 🤖 AI-Powered Features
- Reinforcement Learning (RL) for real-time nudges and personalized messaging
- Machine Learning (ML) clustering for user segmentation and smart offset optimization
- Federated Learning (FL) & Edge AI for privacy-preserving carbon calculations
- Natural Language Processing (NLP) for chatbots and carbon transparency


## 🚀 Installation

### Prerequisites
- Node.js (v18.0.0 or higher)
- pnpm (v8.0.0 or higher)

### Setup Instructions

1. Clone the repository
```bash
git clone https://github.com/saquib5005/amazon-sustainable-shopping.git
cd amazon-sustainable-shopping
```

2. Install dependencies
```bash
pnpm install
```

3. Start the development server
```bash
pnpm dev
```

4. Open your browser and navigate to `http://localhost:5173`

## 📖 Usage

### Product Detail Page Experience

1. View any product to see its green score and carbon footprint
2. Explore eco-friendly alternatives with side-by-side comparisons
3. See the "Carbon vs. Cash" comparison showing environmental savings
4. Interact with carbon labels to learn more about sustainability metrics
5. Receive real-time nudges for greener alternatives

### Search and Filtering

1. Use the search bar at the top of the page with the placeholder "Search your Eco-Alternative"
2. Enter a product name (e.g., "toothbrush")
3. Apply eco-filters to see only sustainable options
4. View green badges and scores directly in search results
5. Compare conventional vs. eco-friendly options

### Checkout Process

1. Review eco-friendly alternatives for items in your cart
2. Choose sustainable packaging options
3. Compare delivery options and their environmental impact
4. View your order's total carbon footprint
5. Apply earned carbon credits for discounts
6. Receive final eco-swap suggestions before purchase

### Exploring the Green Store

1. Navigate to the "Green Store" section from the main navigation
2. Browse through categories of eco-friendly products
3. Use filters to find products based on green score, price, or category
4. View detailed product information including environmental impact

### Using the EcoImpact Dashboard

1. Access your personal dashboard from the main navigation
2. View your carbon footprint reduction metrics and "Hero Stats"
3. Track progress on sustainability challenges and milestones
4. Explore your regional and global impact visualizations
5. View your "Eco-Adventure Map" showing impact locations
6. Check "Quick Wins" for easy sustainability actions

### Group Buying

1. Navigate to the "Group Buying" section
2. Join existing group purchases or create a new one
3. Invite friends within your 2km radius
4. Track the collective environmental impact of your group
5. View your group's virtual garden and leaderboard position
6. Unlock community expeditions with group tokens

### Managing Carbon Credits

1. View your earned carbon credits in your profile
2. Apply credits during checkout for discounts
3. Use credits for Prime membership discounts
4. Track your credit earning history

## 🏗️ Architecture

### High-Level Architecture

The Amazon Sustainable Shopping Experience follows a modern Single Page Application (SPA) architecture with component-based design, context-based state management, and client-side routing.

```
┌─────────────────────────────────────────────────────────────┐
│                  Amazon Sustainable Shopping                │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────────┐  │
│  │             │    │             │    │                 │  │
│  │  Component  │    │   Context   │    │     Routing     │  │
│  │    Layer    │◄───┤    Layer    │◄───┤      Layer      │  │
│  │             │    │             │    │                 │  │
│  └──────┬──────┘    └──────┬──────┘    └─────────────────┘  │
│         │                  │                                │
│         ▼                  ▼                                │
│  ┌─────────────┐    ┌─────────────┐                         │
│  │             │    │             │                         │
│  │    Props    │    │    State    │                         │
│  │  Management │    │  Management │                         │
│  │             │    │             │                         │
│  └─────────────┘    └─────────────┘                         │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Core Architectural Components

#### Component Layer
- **Page Components**: Home, Dashboard, GreenStore, EcoRecommendations, CarbonCashComparison, etc.
- **Shared Components**: Header, SearchBox, ProductCard, etc.
- **UI Components**: Buttons, Modals, Form elements, etc.

#### Context Layer
- **CartContext**: Manages shopping cart state
- **CarbonContext**: Manages carbon footprint calculations
- **UserContext**: Manages user preferences and carbon credits
- **LocalStorage Integration**: Persists cart data between sessions

#### Routing Layer
- **Client-side routing**: Seamless navigation without page reloads
- **Dynamic route parameters**: For product details, search results, etc.

### Data Flow Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                     CartContext Provider                    │
│                                                             │
└───────────────────────────┬─────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                      App Component                          │
│                                                             │
└───────┬─────────────────────┬────────────────────────┬──────┘
        │                     │                        │
        ▼                     ▼                        ▼
┌───────────────┐    ┌────────────────┐      ┌─────────────────┐
│               │    │                │      │                 │
│ Header (Cart  │    │ Product Pages  │      │ Cart Page       │
│  Count)       │    │                │      │                 │
│               │    │                │      │                 │
└───────────────┘    └────────┬───────┘      └─────────────────┘
                             │
                             ▼
                    ┌────────────────┐
                    │                │
                    │ Add to Cart    │
                    │ Functionality  │
                    │                │
                    └────────────────┘
```

### AI/ML Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                     AI/ML Service Layer                     │
│                                                             │
└───────────┬─────────────────┬───────────────────┬───────────┘
            │                 │                   │
            ▼                 ▼                   ▼
┌───────────────┐    ┌────────────────┐    ┌─────────────────┐
│               │    │                │    │                 │
│ RL Engine for │    │ ML Clustering  │    │ NLP for Carbon  │
│ Real-time     │    │ for User       │    │ Transparency    │
│ Nudges        │    │ Segmentation   │    │ & Chatbots      │
│               │    │                │    │                 │
└───────────────┘    └────────────────┘    └─────────────────┘
```

### Folder Structure

```
amazon_sustainable_shopping/
├── public/                  # Static assets
│   ├── images/              # Image assets
│   │   └── products/        # Product images
│   └── index.html           # HTML entry point
├── src/                     # Source code
│   ├── components/          # Reusable UI components
│   │   ├── Header.tsx       # Navigation header
│   │   ├── SearchBox.tsx    # Search component
│   │   ├── CarbonLabel.tsx  # Interactive carbon label
│   │   └── Footer.tsx       # Page footer
│   ├── context/             # React context providers
│   │   ├── CartContext.tsx  # Shopping cart context
│   │   ├── CarbonContext.tsx # Carbon calculation context
│   │   └── UserContext.tsx  # User preferences context
│   ├── lib/                 # Utility functions and data
│   │   ├── productData.ts   # Product data and generation
│   │   ├── carbonCalc.ts    # Carbon footprint calculations
│   │   └── aiService.ts     # AI service integrations
│   ├── pages/               # Page components
│   │   ├── Home.tsx         # Homepage
│   │   ├── Dashboard.tsx    # User dashboard
│   │   ├── GreenStore.tsx   # Eco-friendly product store
│   │   ├── EcoRecommendations.tsx  # Eco-friendly alternatives
│   │   ├── CarbonCashComparison.tsx # Cost vs. environmental impact
│   │   ├── DeliveryImpact.tsx # Delivery options impact
│   │   ├── GroupBuying.tsx  # Group buying feature
│   │   ├── Cart.tsx         # Shopping cart
│   │   └── ...              # Other page components
│   ├── App.tsx              # Main application component
│   └── index.tsx            # Application entry point
├── package.json             # Dependencies and scripts
└── tsconfig.json            # TypeScript configuration
```

## 🛠️ Tech Stack

### Core Technologies

| Technology | Version | Purpose |
|------------|---------|---------|
| TypeScript | 5.x | Type-safe JavaScript development |
| React | 18.x | UI component library |
| Vite | 6.3.5 | Build tool and development server |
| React Router | 6.x | Client-side routing |
| Tailwind CSS | 3.x | Utility-first CSS framework |
| React Icons | Latest | Icon library |

### AI/ML Technologies

| Technology | Purpose |
|------------|---------|
| TensorFlow.js | Client-side ML model execution |
| Reinforcement Learning | Real-time nudges and personalized messaging |
| Machine Learning | User segmentation and smart offset optimization |
| Natural Language Processing | Chatbots and carbon transparency |
| Federated Learning | Privacy-preserving carbon calculations |

### Development Environment

| Tool | Purpose |
|------|---------|
| Node.js | JavaScript runtime |
| pnpm | Package manager |
| TypeScript | Type checking |
| ESLint | Code linting |
| Git | Version control |

### Build and Deployment Pipeline

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│                 │     │                 │     │                 │     │                 │
│  Source Code    │────►│  TypeScript     │────►│  Vite Build     │────►│  Static Site    │
│  (TypeScript)   │     │  Compilation    │     │  Process        │     │  Deployment     │
│                 │     │                 │     │                 │     │                 │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
```

## 📊 User Flow

### Main User Flows

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│                 │     │                 │     │                 │     │                 │     │                 │
│  Landing Page   │────►│  Browse Green   │────►│  View Product   │────►│  Add to Cart    │────►│  Checkout       │
│                 │     │  Store          │     │  Details        │     │                 │     │                 │
│                 │     │                 │     │                 │     │                 │     │                 │
└────────┬────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
         │
         │
         ▼
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│                 │     │                 │     │                 │
│  Search for     │────►│  View Eco       │────►│  Compare        │
│  Products       │     │  Recommendations│     │  Carbon vs Cash │
│                 │     │                 │     │                 │
│                 │     │                 │     │                 │
└─────────────────┘     └─────────────────┘     └─────────────────┘
```

### Product Detail Page Flow

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│                 │     │                 │     │                 │     │                 │
│  View Product   │────►│  See Green      │────►│  View Eco       │────►│  Interact with  │
│  Details        │     │  Score          │     │  Alternatives   │     │  Carbon Label   │
│                 │     │                 │     │                 │     │                 │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
                                                                                 │
                                                                                 │
                                                                                 ▼
                                                                        ┌─────────────────┐
                                                                        │                 │
                                                                        │  Add to Cart    │
                                                                        │                 │
                                                                        │                 │
                                                                        └─────────────────┘
```

### Checkout Process Flow

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│                 │     │                 │     │                 │     │                 │
│  Review Cart    │────►│  Choose         │────►│  Select         │────►│  Apply Carbon   │
│  Items          │     │  Packaging      │     │  Delivery       │     │  Credits        │
│                 │     │                 │     │                 │     │                 │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
                                                                                 │
                                                                                 │
                                                                                 ▼
                                                                        ┌─────────────────┐
                                                                        │                 │
                                                                        │  Complete       │
                                                                        │  Purchase       │
                                                                        │                 │
                                                                        └─────────────────┘
```

## 🤝 Contributing

We welcome contributions to the Amazon Sustainable Shopping Experience project! Here's how you can help:

### Contribution Guidelines

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

### Development Setup

Follow the installation instructions above to set up your development environment.

### Code Style

- Follow the TypeScript and React best practices
- Use functional components with hooks
- Maintain type safety throughout the codebase
- Follow the existing component structure and naming conventions

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Team

- [Saquib Khan](https://github.com/saquib5005) - Project Lead & Developer
- [Firdous Anjum](https://github.com/Firdous-co) - UI/UX Designer

## 🙏 Acknowledgements

- [Amazon](https://www.amazon.com) for hosting the HackOnAmazon challenge
- [React](https://reactjs.org/) for the UI library
- [Tailwind CSS](https://tailwindcss.com/) for the styling framework
- [Vite](https://vitejs.dev/) for the build tool
- All the open-source libraries that made this project possible

---

<div align="center">
  <p>Made with ❤️ for a Sustainable Future</p>
  <p>© 2025 Amazon Sustainable Shopping Experience</p>
</div>
