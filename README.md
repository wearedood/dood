# DOOD - Decentralized Organization Operations Dashboard

A comprehensive dashboard for managing decentralized autonomous organizations (DAOs) with advanced governance, treasury management, and community engagement features.

## 🎆 Overview

DOOD provides a unified interface for DAO operations, enabling seamless governance participation, proposal management, treasury oversight, and community coordination. Built with modern Web3 technologies and designed for scalability across multiple blockchain networks.

## ✨ Key Features

### 🗳️ Governance & Voting
- **Proposal Creation**: Submit and manage governance proposals
- **Voting Mechanisms**: Support for various voting systems (token-weighted, quadratic, etc.)
- **Delegation**: Delegate voting power to trusted community members
- **Execution**: Automated proposal execution upon approval

### 💰 Treasury Management
- **Multi-sig Wallets**: Secure treasury management with multi-signature support
- **Asset Tracking**: Real-time portfolio monitoring across multiple chains
- **Budget Allocation**: Transparent fund distribution and tracking
- **Yield Strategies**: Automated treasury optimization

### 👥 Community Features
- **Member Profiles**: Comprehensive contributor profiles and reputation
- **Discussion Forums**: Integrated governance discussions
- **Notification System**: Real-time updates on proposals and activities
- **Analytics Dashboard**: Community engagement metrics

### 🔗 Multi-Chain Support
- **Ethereum**: Full EVM compatibility
- **Polygon**: Low-cost transactions
- **Arbitrum**: Layer 2 scaling
- **Base**: Coinbase's L2 solution
- **Optimism**: Optimistic rollup support

## 🛠️ Technology Stack

### Frontend
- **React 18**: Modern UI framework
- **TypeScript**: Type-safe development
- **Next.js 14**: Full-stack React framework
- **Tailwind CSS**: Utility-first styling
- **Framer Motion**: Smooth animations

### Blockchain Integration
- **ethers.js**: Ethereum interaction
- **wagmi**: React hooks for Ethereum
- **RainbowKit**: Wallet connection
- **The Graph**: Decentralized indexing

### Backend & Infrastructure
- **Node.js**: Server runtime
- **PostgreSQL**: Primary database
- **Redis**: Caching and sessions
- **IPFS**: Decentralized storage
- **Vercel**: Deployment platform

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- npm or yarn
- MetaMask or compatible Web3 wallet

### Installation

```bash
# Clone the repository
git clone https://github.com/wearedood/dood.git
cd dood

# Install dependencies
npm install

# Copy environment variables
cp .env.example .env.local

# Configure your environment
# Edit .env.local with your API keys and configuration
```

### Environment Configuration

```env
# Blockchain Configuration
NEXT_PUBLIC_ALCHEMY_API_KEY=your_alchemy_key
NEXT_PUBLIC_INFURA_PROJECT_ID=your_infura_id
NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID=your_walletconnect_id

# Database
DATABASE_URL=postgresql://username:password@localhost:5432/dood
REDIS_URL=redis://localhost:6379

# IPFS
IPFS_GATEWAY_URL=https://gateway.pinata.cloud
PINATA_API_KEY=your_pinata_key
PINATA_SECRET_KEY=your_pinata_secret

# Authentication
NEXTAUTH_SECRET=your_nextauth_secret
NEXTAUTH_URL=http://localhost:3000
```

### Development

```bash
# Start development server
npm run dev

# Run tests
npm test

# Build for production
npm run build

# Start production server
npm start
```

## 📚 API Documentation

### Governance Endpoints

```typescript
// Create a new proposal
POST /api/proposals
{
  "title": "Proposal Title",
  "description": "Detailed description",
  "actions": [...],
  "votingPeriod": 7 // days
}

// Vote on a proposal
POST /api/proposals/:id/vote
{
  "vote": "for" | "against" | "abstain",
  "reason": "Optional voting reason"
}
```

### Treasury Endpoints

```typescript
// Get treasury balance
GET /api/treasury/balance

// Create spending proposal
POST /api/treasury/spend
{
  "recipient": "0x...",
  "amount": "1000",
  "token": "USDC",
  "purpose": "Development funding"
}
```

## 🔐 Security

- **Smart Contract Audits**: All contracts audited by leading security firms
- **Multi-sig Requirements**: Critical operations require multiple signatures
- **Time Delays**: Governance actions have mandatory delay periods
- **Emergency Pause**: Circuit breakers for emergency situations
- **Regular Security Reviews**: Continuous security monitoring

## 🤝 Contributing

We welcome contributions from the community! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### Development Workflow

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Add tests for new functionality
5. Ensure all tests pass (`npm test`)
6. Commit your changes (`git commit -m 'Add amazing feature'`)
7. Push to the branch (`git push origin feature/amazing-feature`)
8. Open a Pull Request

### Code Standards

- Follow TypeScript best practices
- Use ESLint and Prettier for code formatting
- Write comprehensive tests
- Document new features
- Follow semantic commit messages

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links & Resources

- **Documentation**: [docs.wearedood.com](https://docs.wearedood.com)
- **Discord Community**: [discord.gg/wearedood](https://discord.gg/wearedood)
- **Twitter**: [@wearedood](https://twitter.com/wearedood)
- **Blog**: [blog.wearedood.com](https://blog.wearedood.com)
- **Governance Forum**: [forum.wearedood.com](https://forum.wearedood.com)

## 📊 Roadmap

### Q1 2025
- [ ] Multi-chain governance implementation
- [ ] Advanced analytics dashboard
- [ ] Mobile application beta

### Q2 2025
- [ ] Cross-chain treasury management
- [ ] AI-powered proposal analysis
- [ ] Integration with major DeFi protocols

### Q3 2025
- [ ] Decentralized identity integration
- [ ] Advanced voting mechanisms
- [ ] Enterprise features

---

**Built with ❤️ by the WeAreDood community**

*Empowering decentralized organizations worldwide*
