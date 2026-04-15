# Real-World Examples of Testing Types
This document provides practical examples of various testing types as defined in the "Testing dot com" methodology (by Roman Savin).

| Testing Type | Context / Website | Test Description | Expected Result |
| :--- | :--- | :--- | :--- |
| **Functional** | *Amazon / E-commerce* | Add a product to the cart and click the "Checkout" button. | The user is redirected to the shipping and payment page. |
| **Negative** | *Payment Form* | Enter an expired credit card (e.g., 05/2022) into the payment field. | System displays an error: "Your card has expired." |
| **UI (User Interface)** | *Apple.com* | Check the layout on a mobile screen (375px width). | Elements do not overlap; text is readable without horizontal scrolling. |
| **Usability** | *Google Search* | Evaluate how easy it is for a new user to find "Search by Image" (Google Lens). | The feature icon is intuitive and accessible within 1-2 clicks. |
| **Localization** | *Netflix* | Switch the language from English to German or French. | All labels and button texts are correctly translated and fit within the UI boundaries. |
| **Compatibility** | *Any Web App* | Open the same dashboard in Safari (macOS) and Chrome (Windows). | The web application looks and functions identically across both environments. |
| **Smoke Testing** | *Online Banking* | Perform a simple login and check the balance after a system update. | Basic "mission-critical" features work; the system is stable for further testing. |
| **Security** | *User Account* | Attempt to access another user's profile settings by manually changing the User ID in the URL. | Access is denied; the system redirects to a 403 Forbidden page. |
| **Performance** | *Ticketing Site* | Simulate 5,000 users clicking "Buy Ticket" at the exact same second. | The server responds within 3 seconds without crashing (no 504 Gateway Timeout). |
| **Regression** | *Instagram* | Test the "Direct Message" feature after an update was made to "Reels". | New changes in Reels did not break the existing messaging functionality. |

---
