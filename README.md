# Shorten URL - Backend Application

## Project Description

Shorten URL is a backend application designed to shorten long URLs and provide analytics to track the number of clicks on the shortened URLs. This application is built using Node.js, Express.js, Mongoose, MongoDB Compass, and Postman.

## Features

- **URL Shortening**: Convert long URLs into shorter, more manageable links.
- **Click Analytics**: Track the number of clicks on each shortened URL to provide insights into link performance.

## Technologies Used

- **Node.js**: JavaScript runtime for building the server-side application.
- **Express.js**: Web application framework for Node.js to create the backend server.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js.
- **MongoDB Compass**: GUI for managing and interacting with the MongoDB database.
- **Postman**: API client for testing and debugging the application.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/shorten-url.git
    cd shorten-url
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Set up environment variables**:
    Create a `.env` file in the root directory and add the following variables:
    ```env
    MONGO_URI=your_mongodb_connection_string
    BASE_URL=your_base_url
    PORT=your_port_number
    ```

4. **Run the application**:
    ```bash
    npm start
    ```

## API Endpoints

### Shorten URL

- **Endpoint**: `/api/url/shorten`
- **Method**: POST
- **Description**: Shortens a long URL.
- **Request Body**:
    ```json
    {
      "longUrl": "https://example.com/very/long/url"
    }
    ```
- **Response**:
    ```json
    {
      "shortUrl": "http://your_base_url/shortcode"
    }
    ```

### Get Analytics

- **Endpoint**: `/api/url/:code`
- **Method**: GET
- **Description**: Redirects to the original URL and increments the click count.
- **Response**:
    - Redirects to the original long URL.

- **Endpoint**: `/api/url/analytics/:code`
- **Method**: GET
- **Description**: Retrieves the analytics data for a shortened URL.
- **Response**:
    ```json
    {
      "clicks": 10
    }
    ```

## Testing

You can use Postman to test the API endpoints. Import the collection from the `postman` directory in the repository and run the requests to see the API in action.

## Database

The application uses MongoDB to store the URL mappings and click analytics. MongoDB Compass can be used to view and manage the database entries.

## Contributing

Feel free to submit issues or pull requests if you have any suggestions or improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for using Shorten URL! If you have any questions or need further assistance, please open an issue on GitHub.

---![Screenshot 2024-06-27 193036](https://github.com/Shubhr457/Backend-App-shortenURL/assets/136572711/d613d517-03bf-468d-a7de-0fbe8d9d9241)
![Screenshot 2024-06-27 193011](https://github.com/Shubhr457/Backend-App-shortenURL/assets/136572711/47f4076d-bf29-40fd-b7f1-cafa1760cbbc)
![Screenshot 2024-06-27 192951](https://github.com/Shubhr457/Backend-App-shortenURL/assets/136572711/b61e4f5e-b984-46e0-bd03-49c65608fac8)


*Developed by Shubh Rathore*
