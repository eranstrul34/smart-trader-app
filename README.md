# Smart Trader App

This repository contains a simple static market watch list example.

The watchlist displays recommended stocks and lets you choose the sort order of the daily change from high to low or low to high. It also includes a search box to filter by symbol name. On page load the watch list fetches real-time quotes from Yahoo Finance so the quote and daily change values are up to date.

Open `watchlist.html` in a web browser to view a table of sample symbols, quotes, and daily changes. Clicking a row opens an analysis page for the selected symbol. The page now displays the company's name, symbol and logo above the chart. Next to the price chart is a section explaining the RSI/resistance, Bollinger cross, average trade volume and historic high/low values.

At the bottom of the watch list is a comparison chart. Drag any row from the table onto the chart to load that symbol's last month of prices. Multiple symbols can be dragged onto the chart to compare their performance.
