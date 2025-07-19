SmartTrader App Specification
===========================

Target platform: Android APK

## Goal
A mobile app that shows real time financial data from Yahoo Finance with simple technical analysis and stock recommendations.

## Technology stack
- Flutter (Dart)
- Yahoo Finance API (or library such as yahoo_fin or yfinance via a backend)
- Firebase (Crashlytics and future notifications)
- LocalStorage for saving favorites

## Modules
1. **Home Screen**
   - Stock search bar with autocomplete
   - List of top movers or stocks by sector (e.g., NETFLIX, APPLE, TESLA)
   - Ability to mark favorites

2. **Stock Detail Screen**
   - Stock name, symbol, current price, daily change
   - Price chart (7 days / month / year)
   - Moving averages (SMA, EMA)
   - Support and resistance calculation
   - Simple formula to suggest BUY, SELL or NEUTRAL

3. **Favorites**
   - List of user-marked stocks
   - Remove stocks from favorites

## API
Use Yahoo Finance endpoints or an intermediary service:
- `/quote` – current price
- `/chart` – price history
- `/recommendation` – analyst recommendations (optional)

## Functionality
- API calls with error handling
- Loading indicators
- Persist favorites locally
- English language interface

## Key files
- `main.dart` – app entry point
- `home_screen.dart` – search and top movers display
- `stock_detail_screen.dart` – view stock info
- `favorites_screen.dart` – manage favorites
- `stock_service.dart` – API layer
- `stock_utils.dart` – technical analysis calculations

## Notes
- Simple UI, no user registration required
- Focus on fast UX and efficient API usage
- Initially Android only
