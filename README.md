# Node.js Google Sheets API Integration

This project demonstrates how to integrate the Google Sheets API with a Node.js application. It allows users to read from and write data to a Google Sheet.

## Features

- **Write Data**: Add new rows to a Google Sheet.
- **Read Data**: Retrieve data from a specified range in the Sheet.

## Prerequisites

- [Node.js](https://nodejs.org/)
- A Google Cloud Platform account with the Sheets API enabled
- A service account key file (JSON) from Google Cloud Console

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/adanzweig/nodejs-google-sheets.git
   cd your-repository
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Set Up Your Credentials**

   Place your Google service account key file (e.g., `google.json`) in the root directory.

## Usage

- **Writing Data to Google Sheets**

  Call the `writeToSheet` function with an array of data. Each sub-array represents a row.

  ```javascript
  const dataToWrite = [['Name', 'Age', 'Location'], ['Alice', 30, 'New York']];
  writeToSheet(dataToWrite);
  ```

- **Reading Data from Google Sheets**

  Simply call the `readSheet` function. It retrieves data from the specified range in the sheet.

  ```javascript
  readSheet().then(data => console.log(data));
  ```

## Configuration

- Update the `spreadsheetId` in `index.js` to point to your target Google Sheet.
- Adjust the range in the `writeToSheet` and `readSheet` functions as needed.

## Contributing

Contributions, issues, and feature requests are welcome!

## License

This project is licensed under the [MIT License](LICENSE).