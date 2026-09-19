# SHOP — HTML/CSS/JavaScript + Supabase

Complete static-first ecommerce application. Plain HTML/CSS/ES modules for the UI; Supabase Auth/Postgres/Storage/RLS for backend; Vercel functions for Razorpay server operations.

## Setup
1. Create a fresh Supabase project.
2. Run `supabase/reset.sql` once in SQL Editor.
3. Sign up one account, then make it admin using the SQL comment at the bottom of reset.sql.
4. Put the public Supabase URL and anon/publishable key in `js/config.js`. Never put a service-role key in browser files.
5. Deploy this folder to Vercel.
6. Add Vercel environment variables RAZORPAY_KEY_ID, RAZORPAY_KEY_SECRET, RAZORPAY_WEBHOOK_SECRET for payments.
7. Configure Supabase Auth site URL and Google provider if Google login is wanted.

Customer pages: home, shop, product, cart, checkout, orders, account, login/signup.
Admin pages: dashboard, products, categories, inventory, orders, customers, delivery, coupons, offers, payments, reports, settings.
Delivery page: assigned deliveries and status update.
