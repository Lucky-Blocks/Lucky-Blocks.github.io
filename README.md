🚀 Project Setup

Built a Node.js + Express backend (server.js) with:

Stripe Checkout integration (secure payments).

SQLite database for storing orders and reviews.

Webhook support to record successful orders.

Admin endpoint to view all orders with authentication.

Created .env for secrets:

STRIPE_SECRET_KEY (no you dont get these lol)

STRIPE_WEBHOOK_SECRET

ADMIN_PASSWORD

Ensured .env, node_modules, and orders.db are in .gitignore.

🖥️ Frontend (Public)

Designed index.html with a modern store layout:

Product grid with images, titles, and prices.

Quick View modal for product details.

Cart system (add multiple items before checkout).

Stripe “Buy Now / Checkout” buttons integrated with backend.

Dynamic product sorting & search.

Customer reviews panel with rotating reviews under cart.

Contact dropdown in top-right with phone/email info.

Footer with branding + credits (© 2025 Lucky Loot Boxes).

Added additional pages:

success.html – Order confirmation page with order details + review form.

cancel.html – Checkout cancellation page.

out-of-stock.html – For unavailable items.

favicon.png and numbered product images (1.png–7.png).

📦 Backend Features

Order handling: (THESE WILL BE IMPLEMENTED TO THE MAIN SITE. THEY ARE NOT HERE DUE TO SECURITY REASONS)

On checkout success, Stripe webhook saves order info (email, items, total, date) to SQLite.

Review handling:

POST /add-review → allows customers to submit a review after purchase.

GET /reviews → returns all reviews for shuffle display on homepage.

Admin:

/orders endpoint with password-protected access.

🌐 Hosting & GitHub

Set up GitHub repository (Lucky-Blocks.github.io).

Uploaded frontend files (index.html, assets, success/cancel pages, etc.).

Left out server.js, .env, and orders.db since GitHub Pages cannot run a backend.

Next step: host backend separately (Render / Railway / Heroku) and connect it to the GitHub Pages frontend.

⭐ Key Features for Customers

Fully functional shopping cart.

Secure checkout powered by Stripe.

Post-purchase review system (reviews added live).

Customer-friendly UI: modern design, quick view, sorting, responsive layout.

Trust-building: review shuffle + 5-star panel + footer credits + contact options.
