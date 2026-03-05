This project automates the **end-to-end process of placing an order** on the [Automation Testing Practice Site](https://practice.automationtesting.in/).  
It validates **product details, basket totals, checkout totals, and the order confirmation message**.

---

## 👤 Devloped By
**Pranusha Naika**  
Email: pranushanaika@gmail.com  


---

## 🛠 Tech Stack
- **Programming Language:** Java  
- **Automation Framework:** Selenium WebDriver  
- **Test Framework:** TestNG  
- **Browser Driver:** ChromeDriver  
- **IDE:** Eclipse / IntelliJ IDEA  
- **Build Tool (optional):** Maven  

---

## 📂 Project Structure

Automation/
├── Firstproject.java # Main test script containing the automation code
├── README.md # Project instructions and details
└── pom.xml (optional) # Maven dependencies


---

## 📝 Test Scenario
1. Open the demo site: `https://practice.automationtesting.in/`.
2. Scroll and select a product from the listing page.
3. Capture **Product Title** and **Price** from the listing page.
4. Add the product to the basket.
5. View the basket and verify the **product title** and **price** match the listing page.
6. Update the product quantity and validate that **total price** is updated correctly.
7. Proceed to checkout.
8. Fill mandatory billing details:
   - First Name, Last Name
   - Company, Email, Phone
   - Address, City, Country, State, Postcode
9. Verify checkout total matches basket total.
10. Select **Cash on Delivery** as payment method and place the order.
11. Verify the confirmation message: *“Thank you. Your order has been received.”*

---

## ⚙ Setup & Execution

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd <repo-folder>
2. Setup ChromeDriver

Download ChromeDriver matching your Chrome version from ChromeDriver Downloads
.

Add it to your system PATH, or set it in code:

System.setProperty("webdriver.chrome.driver", "path/to/chromedriver.exe");
3. Run the Test

Using IDE (Eclipse/IntelliJ):

Right-click Firstproject.java → Run As → TestNG Test

Using Maven (optional):

mvn test
🔍 Example Console Output
Listing Product Name: Selenium Ruby
Listing Product Price: ₹500.00
Basket Product Name: Selenium Ruby
Basket Product Price: ₹500.00
✅ Product name and price verified successfully.
Quantity: 4
Basket Total Numeric: 2000.0
✅ Basket total matches Listing Price × Quantity
Checkout Total: ₹2000.00
✅ Total matches between Basket and Checkout.
Order Message: Thank you. Your order has been received.
✅ Order placed successfully.
