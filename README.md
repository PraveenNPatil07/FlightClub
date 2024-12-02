
# FlightClub(Flight Price Tracker)

Flight Price Tracker is a Python-based project designed to monitor flight prices and notify users of low-cost deals. It integrates with Google Sheets for data storage, searches for direct and indirect flights using a flight API, and sends notifications via email or WhatsApp when affordable flights are found.


## Features

- Google Sheets Integration: Manage destination and customer data seamlessly.
- Direct and Indirect Flight Search: Finds both direct and         stopover flights for the specified routes.
- Notification System: Alerts users through email and WhatsApp about low-price flight deals.
- Customizable Origin Airport: Easily set the starting point for flight searches.


## How It Works

1. Retrieve Data: Fetch destination and customer email data from Google Sheets.
2. Update IATA Codes: Automatically update missing IATA codes for destinations in the sheet.
3. Search Flights: Query for flights from the specified origin to destinations over a six-month period.
4. Find Best Deals: Compare prices to the target price and identify the cheapest options.
5. Notify Users: Send notifications with flight details when cheaper options are found.

## Screenshots
![Email](https://github.com/user-attachments/assets/6797ee27-2b30-4354-af67-d16478b9586b)
![Whatsapp & SMS message](https://github.com/user-attachments/assets/3e2739be-c171-4a9f-9f32-a200978f5ef5)

## Prerequisites

- Python 3.7+
- Google Sheets API credentials
- Flight search API key (e.g., Tequila by Kiwi.com)
- Twilio API credentials for WhatsApp or SMS notifications (optional)
## Installation

1. Clone the repository:

```bash
git clone https://github.com/PraveenNPatil07/FlightClub.git
cd flight-price-tracker
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Set up environment variables:
- Create a .env file in the project directory.
- Add your API keys and credentials:
```bash
SHEET_API_KEY=your_google_sheets_api_key
FLIGHT_API_KEY=your_flight_search_api_key
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
```
    
## Usage
1. Update the Google Sheet with your destination data and customer emails.
2. Run the script:
```bash
python main.py
```
3. Check your notifications for updates on low-price flights.
