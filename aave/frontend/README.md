# Openfort Wallet App

A React + Vite application that demonstrates Openfort's embedded wallet functionality with a beautiful, centered UI.

## Features

- 🚀 **React + Vite** - Fast development and building
- 💳 **Openfort Embedded Wallet** - Non-custodial wallet creation and management
- 🎨 **Beautiful UI** - Centered wallet button with gradient design
- 🔐 **Shield Security** - Advanced wallet recovery and security features
- ⛽ **Gas Sponsorship** - All transactions sponsored by Openfort policy
- 🌐 **Base Sepolia** - Testnet support for development

## Prerequisites

Before running this app, you need:

1. **Openfort Project** - Already created with API keys
2. **WalletConnect Project ID** - Get one from [WalletConnect Cloud](https://cloud.reown.com/sign-in)

## Setup

### 1. Install Dependencies

```bash
npm install
```

### 2. Environment Configuration

The `.env` file is already configured with your Openfort project details. You just need to:

1. Get your WalletConnect Project ID from [WalletConnect Cloud](https://cloud.reown.com/sign-in)
2. Update `VITE_WALLET_CONNECT_PROJECT_ID` in the `.env` file

### 3. Run the Development Server

```bash
npm run dev
```

The app will be available at `http://localhost:5173`

## How It Works

### Wallet Creation
- Users click the OpenfortButton to start wallet creation
- Openfort handles authentication (email, social, etc.)
- A non-custodial embedded wallet is created
- All transactions are sponsored by your Openfort policy

### Security Features
- **Shield Recovery**: Uses Shamir Secret Sharing for secure key management
- **Password Recovery**: Users can recover wallets with passwords
- **Non-custodial**: Users maintain full control of their private keys

### Gas Sponsorship
- All user transactions are sponsored by your Openfort policy
- Policy ID: `pol_a330c062-8f01-4ef7-8a31-8dbea09b004a`
- Chain: Base Sepolia (Chain ID: 84532)

## Project Structure

```
src/
├── App.tsx              # Main application component
├── App.css              # Styling for the wallet interface
├── Providers.tsx        # Openfort, Wagmi, and TanStack providers
└── main.tsx             # Application entry point
```

## Customization

### Styling
- Modify `src/App.css` to change the visual appearance
- The wallet button is centered with a gradient background
- Responsive design for mobile and desktop

### Configuration
- Update chain configuration in `src/Providers.tsx`
- Modify wallet recovery methods
- Change authentication providers

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## Troubleshooting

### Common Issues

1. **WalletConnect Project ID Error**
   - Make sure you have a valid WalletConnect Project ID
   - Update the `.env` file with the correct ID

2. **Openfort API Key Issues**
   - Verify your publishable key is correct
   - Check that your project is active in Openfort dashboard

3. **Chain Configuration**
   - Ensure Base Sepolia is supported in your Openfort project
   - Verify the chain ID matches your policy configuration

## Next Steps

- [Openfort Documentation](https://docs.openfort.io/)
- [React SDK Guide](https://docs.openfort.io/products/embedded-wallet/react)
- [WalletConnect Cloud](https://cloud.reown.com/sign-in)

## License

This project is open source and available under the MIT License.
