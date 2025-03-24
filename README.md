FoodKiosk - Flask Web Application

This project is a web-based food kiosk application built using Python and the Flask framework.

## Description

The FoodKiosk application provides a user interface for customers to browse a menu, add items to an order, manage their cart, and complete the payment process. It includes:

*   A menu listing with categorized items
*   A shopping cart with item quantity management
*   Order summary and total calculation
*   Payment integration with Razorpay
*   User login and registration
*   Token number generation for orders

 Features

Browse menu items categorized by:
    *   Popular
    *   Chicken
    *   Burgers
    *   Sides
    *   Beverages
    *   Desserts
*   Add items to a shopping cart
*   Adjust item quantities in the cart (increment/decrement)
*   Remove items from the cart
*   View a real-time order summary with subtotal, tax, service fee, and total amount
*   Generate a unique token number for orders
*   Process payments using Razorpay
*   User login and registration using forms
*   Responsive layout with Tailwind CSS

 Prerequisites

Before running this application, ensure you have the following installed:

*   **Python 3.6+**
*   **pip** (Python package installer)

## Installation

1.  **Clone the Repository:**
    ```bash
    git clone [repository URL]
    cd foodkiosk_flask
    ```

2.  **Create a Virtual Environment:** (Recommended)
    ```bash
    python3 -m venv venv
    ```

3.  **Activate the Virtual Environment:**
    *   On Windows:
        ```bash
        venv\Scripts\activate
        ```
    *   On macOS and Linux:
        ```bash
        source venv/bin/activate
        ```

4.  **Install Dependencies:**
    ```bash
    pip install Flask razorpay python-dotenv
    ```

## Configuration

1.  **Environment Variables:**
    *   Create a `.env` file in the root directory:
        ```
        .env
        ```
    *   Add the following environment variables:
        ```
        FLASK_SECRET_KEY=YourSecretKey
        RAZORPAY_KEY_ID=YourRazorpayKeyId
        RAZORPAY_KEY_SECRET=YourRazorpayKeySecret
        ```
        *   Replace `YourSecretKey` with a strong, randomly generated secret key.
        *   Replace `YourRazorpayKeyId` and `YourRazorpayKeySecret` with your actual Razorpay API keys.
    *   **Note:** Ensure that your `.env` file is added to your `.gitignore` file to prevent accidental exposure of sensitive information.
2. **Configure the database:
Update the SQL path where your database created,

## Running the Application

1.  **Start the Flask App:**
    ```bash
    python app.py
    ```

2.  **Open in Browser:**
    Open your web browser and navigate to `http://127.0.0.1:5000/`.

 Payment Integration

This project uses the Razorpay payment gateway. To properly configure the payment integration:

1.  **Sign up for a Razorpay account:** Create an account at [https://razorpay.com/](https://razorpay.com/).
2.  **Obtain API Keys:** Get your API keys (Key ID and Key Secret) from the Razorpay dashboard.
3.  **Update Environment Variables:** Put all details in ENVIROMENT variables.
4.  **Test Mode:** For testing, use Razorpay's test mode and test keys. Make sure to use live API keys for production.

*Important Notes*
-Ensure you configured and saved the secret key and test mode is well implemented.

 License

This project is licensed under the [License Name] License - see the [LICENSE.md](LICENSE.md) file for details.
