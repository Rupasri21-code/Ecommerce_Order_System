# Ecommerce_Order_System
CLI-based E-commerce Order Engine simulating real backend systems. Supports product &amp; inventory management, multi-user carts, order processing, payment handling, rollback, concurrency control, fraud detection, logging, and event-driven operations ensuring consistency and scalability.
# 🛒 E-Commerce Order Engine (CLI-Based)

#📌 Project Overview
This project is a CLI-based **E-Commerce Order Engine** that simulates the backend functionality of real-world online shopping platforms like Amazon or Flipkart. It is designed to handle product management, multi-user carts, order processing, payment simulation, and system reliability using concepts like concurrency control, transactions, and rollback mechanisms.

 #🚀 Features

### 🛍️ Product & Inventory Management
- Add new products with unique IDs
- Update and validate stock levels
- Prevent negative stock and duplicates
- View all available products
- Low stock alert system



# 🛒 Multi-User Cart System
- Separate cart for each user
- Add, remove, and update cart items
- Real-time stock synchronization
- Stock reservation when adding items



### 🔒 Concurrency Handling
- Simulates multiple users accessing the same product
- Uses locking to prevent race conditions
- Ensures no overselling of inventory

---

#📦 Order Processing
- Convert cart into order
- Validate cart before checkout
- Atomic transaction handling (all-or-nothing)
- Automatic cart clearing after order placement

#💳 Payment Simulation
- Simulates payment success and failure
- Handles failures with rollback
- Maintains system consistency

# 🔄 Transaction Rollback
- Restores stock if payment fails
- Cancels incomplete orders
- Ensures data integrity

#🔁 Order Management
- View all orders
- Cancel orders with stock restoration
- Prevent duplicate cancellations
- Track order status

---

# 🎟️ Discount & Coupon Engine
- Discount for orders above ₹1000
- Additional discount for bulk quantity
- Supports coupon codes:
  - `SAVE10` (10% off)
  - `FLAT200` (₹200 off)

---

#🔔 Inventory Alerts
- Displays low stock products
- Prevents purchase when stock is zero

---

#📜 Audit Logging System
- Logs all system activities
- Maintains timestamp-based records

# 🚨 Fraud Detection
- Detects multiple orders within a short time
- Flags suspicious user behavior



#⚡ Event-Driven System
- Simulates event queue processing
- Handles events like order creation and updates

#🔁 Idempotency Handling
- Prevents duplicate order processing
- Handles repeated user requests safely

# 💥 Failure Injection
- Random failure simulation for testing
- Ensures system recovery and stability

# 🧠 Design Approach
- Built using **Python**
- Uses **modular and service-based design**
- Implements **thread-safe operations using locks**
- Ensures **data consistency with transactions and rollback**
- Simulates **microservice architecture**

# ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Rupasri21-code/Ecommerce_Order_System.git
