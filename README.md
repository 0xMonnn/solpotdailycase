# Solpot Bot - Multi-Account Daily Case Automation

An automation bot for claiming daily cases on Solpot with multi-account support.
## Prerequisites

- Node.js >= 14.x
- NPM >= 6.x
## Installation

1. Clone the repository:

```bash
git clone https://github.com/0xMonnn/solpotdailycase.git
cd solpotdailycase
```

2. Install dependencies:

```bash
npm install
```

3. Edit `data.txt` file in the root directory and add your account cookies (one per line):

```
cookie_account_1
cookie_account_2
cookie_account_3
```

### How to Get Your Cookie

1. Open Chrome DevTools:
   - Press `F12` or
   - Right-click anywhere and select "Inspect" or
   - Press `Ctrl + Shift + I` (Windows/Linux) or `Cmd + Option + I` (Mac)

2. Go to Network tab in DevTools:

   - Click on the "Network" tab
   - Make sure "Preserve log" is checked

3. Get the cookie:
   - Go to any page on Solpot
   - In Network tab, find any request to `solpot.com`
   - Click on the request
   - In the Headers section, scroll down to find "Cookie"
   - Copy the entire value that starts with `solpotsid=`

Example of cookie format:
```
solpotsid=x%3Au%3A3A75fe516857...rest_of_cookie_value
```

**Note**: Do not share your cookies with anyone. They provide full access to your account.

### Main Configuration Options
## 🔧 Usage

1. Start the bot:

```bash
node main.js
```
## Important Notes

1. **Security**

   - Keep your `data.txt` file secure
   - Don't share your cookies
   - Use at your own risk

2. **Rate Limiting**

   - The bot includes a delay between accounts to prevent rate limiting
   - Modify `TIME.DELAY_BETWEEN_ACCOUNTS` if needed

3. **Cookies**
   - Update cookies in `data.txt` if they expire
   - One cookie per line
   - Make sure there are no empty lines

## License

This project is licensed under the MIT License - see the LICENSE file for details.