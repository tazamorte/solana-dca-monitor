# Solana DCA Transaction Monitor

A robust monitoring and analytics platform for DCA (Dollar Cost Averaging) transactions on the Solana blockchain.

![Solana DCA Monitor](https://raw.githubusercontent.com/solana-labs/solana/master/web3.js/examples/solana-banner.png)

## 🚀 Features

- **Real-time Transaction Monitoring**: Stream transactions via WebSocket for instant updates
- **Analytics Dashboard**: Track DCA performance, volume rankings, and historical data
- **Self-hosted Solana RPC**: Control your own infrastructure with optimized costs
- **Multi-Token Support**: Monitor transactions across various token pairs
- **Flexible Filtering**: Filter by transaction type, value, and timeframe

## 📊 Dashboard

The platform provides comprehensive analytics:
- Token volume rankings
- Transaction history with filtering
- Performance metrics and trends

## 💻 Tech Stack

### Frontend
- Next.js with App Router
- Tailwind CSS + shadcn/ui
- Zustand for state management

### Backend
- FastAPI (Python)
- Azure SQL Serverless
- Azure Redis Cache

### Blockchain
- Self-hosted Solana RPC Node
- Solana Web3.js for transaction handling

## 🛠️ Getting Started

### Prerequisites
- Node.js 20+
- Python 3.12+
- Azure account (for deployment)

### Local Development
```bash
# Clone the repository
git clone https://github.com/tazamorte/solana-dca-monitor.git
cd solana-dca-monitor

# Install dependencies
pnpm install
pip install -r requirements.txt

# Start development servers
pnpm dev
```

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.