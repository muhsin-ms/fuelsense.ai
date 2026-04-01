# FuelSense 2.0 - Trip Cost Projection Dashboard

FuelSense is a smart, serverless web application designed to help Indian commuters estimate their trip costs accurately. It integrates Google Maps for routing and real-time infrastructure data.

## 🚀 Features

- **100+ Vehicle Profiles**: Pre-mapped data for Indian cars and two-wheelers.
- **Dynamic Fuel Rates**: Scrapes live market prices for Petrol and Diesel.
- **Smart Radar**: Automatically finds gas stations or EV charging points along your route.
- **Best/Worst Case Projection**: Provides a price range based on traffic and driving conditions.
- **GitHub Actions Ready**: Automated deployment to GitHub Pages.

## 🛠️ Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/fuelsense.git
   cd fuelsense
   ```

2. **Configure API Keys**:
   - Open `js/config.js`.
   - Paste your **Google Maps API Key** into the `GOOGLE_MAPS_KEY` field.
   - Alternatively, use the in-app settings menu to save keys locally in your browser.

3. **Run Locally**:
   Simply open `index.html` in any browser or use a local server:
   ```bash
   python -m http.server 8000
   ```

## 📦 Deployment to GitHub Pages

This project is pre-configured for **GitHub Actions** deployment:

1. Push your code to the `main` branch.
2. In your GitHub Repo: Go to **Settings > Pages**.
3. Under **Build and deployment > Source**, select **"GitHub Actions"**.
4. Your site will be live at `https://your-username.github.io/your-repo-name/`.

## 🔒 Security Note
If your repository is public, ensure you **do not** commit your API keys to `js/config.js`. Users should enter their own keys via the UI, which are stored securely in their `localStorage`.
