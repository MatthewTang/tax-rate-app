# Hong Kong Tax Rate App

## Project Overview

The Hong Kong Tax Rate App is an interactive infographic web application designed to help users understand Hong Kong's salaries tax system for the 2025/26 assessment year. This comprehensive tool provides visual insights into tax calculations, effective tax rates, and personalized tax-saving strategies.

The application features an intuitive interface that displays how tax liability changes across different income levels, highlighting Hong Kong's progressive tax system. Users can explore detailed tax data through interactive charts and receive AI-powered personalized tax savings advice based on their income level.

Key highlights include:
- **Tax Savings Advisor**: AI-powered recommendations for potential tax deductions and savings strategies
- **Interactive Charts**: Visual representation of tax payable amounts and effective tax rates across income levels
- **Detailed Data Breakdown**: Comprehensive table showing precise tax calculations for different monthly income brackets
- **2025/26 Assessment Year**: Up-to-date calculations based on current Hong Kong tax regulations

## Features

- **🤖 AI-Powered Tax Savings Advisor**
  - Personalized tax optimization tips based on income level
  - Interactive modal interface for easy access
  - Recommendations for MPF contributions, charitable donations, and education expenses
  - Powered by Google Gemini API for intelligent suggestions

- **📊 Interactive Charts**
  - **Tax Payable Chart**: Bar chart showing absolute tax amounts by income level
  - **Effective Tax Rate Chart**: Line chart illustrating the progressive nature of Hong Kong's tax system
  - Responsive design with hover tooltips for detailed information

- **📋 Detailed Tax Data Table**
  - Complete breakdown of monthly income, annual income, tax payable, and effective rates
  - Covers income ranges from HK$10,000 to HK$70,000 per month
  - Formatted for easy reading and comparison

- **💡 Key Statistics Dashboard**
  - Prominent display of important tax facts and figures
  - Highlights maximum effective tax rate and standard allowances
  - Quick reference for common tax scenarios

- **📱 Responsive Design**
  - Mobile-friendly interface using TailwindCSS
  - Optimized for various screen sizes and devices
  - Clean, modern design with accessible color schemes

## Installation

### Prerequisites
No special prerequisites are required. The application runs entirely in the browser using modern web technologies.

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/MatthewTang/tax-rate-app.git
   cd tax-rate-app
   ```

2. **Open the application**
   Simply open the `index.html` file in your web browser:
   ```bash
   # Option 1: Open directly in browser
   open index.html
   
   # Option 2: Use a local server (recommended)
   python -m http.server 8000
   # Then navigate to http://localhost:8000
   ```

### Dependencies

The application uses the following external libraries loaded via CDN:
- **TailwindCSS**: For responsive styling and layout
- **Chart.js**: For interactive data visualizations
- **Google Fonts (Inter)**: For typography
- **Google Gemini API**: For AI-powered tax advice (requires API key)
- **Sentry Browser SDK**: For error monitoring and performance tracking (optional)

No installation or package management is required as all dependencies are loaded from CDN.

### Configuration (Optional)

#### AI Tax Savings Advisor
To enable the AI Tax Savings Advisor feature:
1. Obtain a Google Gemini API key from the Google AI Studio
2. Replace the empty `apiKey` variable in the JavaScript section of `index.html`
3. The feature will work without an API key but will show an error message

#### Sentry Error Monitoring
The application includes Sentry error monitoring for tracking and debugging issues:

1. **Create a Sentry Account**
   - Sign up at [sentry.io](https://sentry.io)
   - Create a new project for JavaScript/Browser applications

2. **Configure Sentry DSN**
   - Copy your project's DSN from the Sentry dashboard
   - In `index.html`, replace `'YOUR_SENTRY_DSN_HERE'` with your actual DSN
   - Update the environment setting from 'development' to 'production' for live deployments

3. **Test Error Monitoring**
   - Use the "🐛 Test Error Monitoring" button to verify Sentry integration
   - Check your Sentry dashboard to see captured errors and performance data

4. **Optional: Customize Sentry Configuration**
   - Adjust sample rates for performance monitoring and session replay
   - Modify user context and tags as needed for your use case
   - Configure additional integrations in the Sentry.init() call

**Note**: The application will function normally even if Sentry is not configured. All Sentry-related code includes error handling to prevent disruption of the main application.

## Usage

### Main Interface

1. **Language Selection**: Use the language selector in the top-right corner to switch between English and Traditional Chinese (繁體中文)

2. **View Tax Statistics**: The homepage displays key tax information including the highest effective tax rate (12.19%) and standard basic allowance (HK$132,000)

3. **Explore Charts**:
   - **Tax Payable Chart**: Shows how absolute tax amounts increase with income
   - **Effective Tax Rate Chart**: Demonstrates the progressive nature of Hong Kong's tax system

4. **Review Detailed Data**: Use the comprehensive table to see exact figures for different income levels

### Tax Savings Advisor

1. **Access the Advisor**: Click the "Get Personalized Tax Savings Tips" button
2. **Select Income Level**: Choose your monthly income from the dropdown menu
3. **Generate Tips**: Click "Generate My Tips" to receive AI-powered advice
4. **Review Recommendations**: Read personalized suggestions for tax optimization
5. **Test Error Monitoring**: Use the "🐛 Test Error Monitoring" button to verify Sentry integration (when configured)

### Interactive Features

- **Chart Tooltips**: Hover over chart elements to see detailed values
- **Responsive Tables**: Scroll horizontally on mobile devices to view all table columns
- **Modal Interface**: Full-screen modal for distraction-free tax advice

### Data Coverage

The application covers monthly income ranges from HK$10,000 to HK$70,000, showing:
- Annual income calculations
- Tax payable amounts
- Effective tax rates
- Progressive tax impact

## License

This project is currently **unlicensed**. All rights are reserved by the author. If you wish to use, modify, or distribute this code, please contact the repository owner for permission.

## Contribution

### How to Contribute

Contributions to improve the Hong Kong Tax Rate App are welcome! Here are ways you can help:

1. **Report Issues**: Found a bug or have a suggestion? Open an issue on GitHub
2. **Improve Documentation**: Help make the README or code comments clearer
3. **Enhance Features**: Add new visualizations, improve the UI, or extend functionality
4. **Update Tax Data**: Help keep tax rates and allowances current with Hong Kong regulations

### Development Guidelines

1. **Fork the Repository**: Create your own fork to work on changes
2. **Make Targeted Changes**: Focus on specific improvements rather than broad rewrites
3. **Test Thoroughly**: Ensure changes work across different browsers and devices
4. **Maintain Style**: Follow the existing code style and formatting
5. **Update Documentation**: Include any necessary documentation updates

### Areas for Contribution

- **Tax Data Updates**: Keep calculations current with latest Hong Kong tax regulations
- **Additional Features**: New chart types, export functionality, or comparison tools
- **Accessibility**: Improve screen reader compatibility and keyboard navigation
- **Performance**: Optimize loading times and chart rendering
- **Internationalization**: ✅ English and Traditional Chinese support implemented

### Submitting Changes

1. Create a descriptive pull request explaining your changes
2. Include screenshots for UI changes
3. Ensure the application still functions correctly
4. Be responsive to feedback and suggestions

For major changes, please open an issue first to discuss your proposed modifications with the maintainers.

---

**Disclaimer**: This application is for informational purposes only and does not constitute financial or tax advice. Please consult with qualified professionals for official tax guidance. Tax calculations are based on 2025/26 assessment year rates and assume only the basic allowance with no other deductions.