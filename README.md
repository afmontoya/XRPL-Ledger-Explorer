# XRPL Ledger Explorer

A lightweight, browser-based explorer for the XRP Ledger that allows users to view account balances, transaction history, and current ledger information.

## Features

- Real-time connection to the XRP Ledger
- View current ledger index and transaction count
- Check account balances
- Display recent transactions for any XRP address
- Direct links to XRPScan for detailed transaction information

## Demo

View account information by entering any valid XRP address. A test account is provided by default:
```
rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/xrpl-ledger-explorer.git
cd xrpl-ledger-explorer
```

2. Serve the files using any web server. For example, using Python:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

3. Open your browser and navigate to:
```
http://localhost:8000
```

## Technical Details

- Built with vanilla JavaScript and HTML/CSS
- Uses the XRPL JavaScript library (xrpl.js)
- Connects to public XRPL nodes via WebSocket
- No backend required - runs entirely in the browser

## Dependencies

- XRPL.js library (loaded via unpkg CDN)
- Modern web browser with JavaScript enabled
- Internet connection to access the XRP Ledger

## Usage

1. Open the application in your web browser
2. Wait for the connection to the XRPL network (indicated by the Ledger Details section)
3. Enter an XRP address in the input field
4. Click "Check Balance" to view the account information
5. View the account's recent transactions below the balance information

## API Endpoints

The application connects to the XRP Ledger using the following endpoints:

- WebSocket Server: `wss://xrplcluster.com`
- Explorer Links: `https://xrpscan.com/tx/{hash}`

## Error Handling

The application includes error handling for:
- Invalid XRP addresses
- Network connection issues
- Failed API requests
- Data parsing errors

## Browser Support

Tested and working in:
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Security

This application connects directly to the XRP Ledger and only performs read operations. No private keys or sensitive information are ever requested or stored.

## Acknowledgments

- XRP Ledger Foundation for maintaining the public nodes
- XRPL.js team for the JavaScript library
- XRPScan for transaction lookup services

## Support

For support, please open an issue in the GitHub repository or contact the maintainers directly.
