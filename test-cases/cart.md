| ID | Summary | Pre-conditions | Step-by-Step Instruction | Expected Result |
| :-- | :--- | :--- | :--- | :--- |
| **1** | Add product to cart | A random item is selected and its Product Detail Page is loaded. | 1. Click the **"Add to Cart"** button.<br>2. Open the **Cart** page. | Product is displayed in the cart with the correct name, image, and price.<br>Cart icon badge updates to **"1"**. |
| **2** | Change product quantity | At least one product is in the cart. | 1. Change quantity from "1" to "2" using the **"+"** button or input field.<br>2. Wait for the page to update. | The **"Subtotal"** and **"Total"** prices are doubled and displayed correctly. |
| **3** | Remove product from cart | At least one product is in the cart. | 1. Click the **"Remove"** (trash icon) button next to the product. | Product is removed from the list.<br>Cart is empty, and a **"Your cart is empty"** message appears. |
| **4** | Apply discount coupon | Products are in the cart; user has a valid coupon code `SAVE10`. | 1. Enter `SAVE10` in the **Promo Code** field.<br>2. Click **"Apply"**. | Discount is applied.<br>**"Total"** price decreases by 10%.<br>A success message **"Coupon applied"** is shown. |
| **5** | Proceed to Checkout | Products are in the cart. | 1. Click the **"Checkout"** button. | User is redirected to the **Shipping/Payment** information page.<br>Cart data is preserved. |
