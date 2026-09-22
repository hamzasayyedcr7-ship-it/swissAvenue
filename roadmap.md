# Roadmap

- [x] Build shared storefront shell and frontend state (ink/ivory/brass palette, matching the existing homepage and design tokens — not the sky-blue placeholder originally noted here)
- [x] Add 54-product sample catalogue and coordinated product imagery
- [x] Build searchable, filterable, sortable shop
- [x] Build product detail routes
- [x] Build cart page and cart side panel
- [x] Build wishlist page and move-to-cart flow
- [x] Preserve and adapt existing Swiss Avenue homepage content
- [ ] Validate responsive layouts and Phase 1 interactions

## Phase 2 — Database + auth

- [x] Full schema + RLS policies (`supabase/migrations/0001_init.sql`)
- [x] Supabase browser client (anon key) + server-only client (service role)
- [x] Real sign up / login / logout / forgot password / reset password
- [x] Account page: profile summary, saved addresses (add/delete), logout
- [ ] Migrate the static `src/lib/products.ts` catalogue into the `products` table (storefront still reads local data for now)
- [ ] Sync guest localStorage cart/wishlist into `cart_items`/`wishlist_items` on login
- [ ] Admin auth + role check + dashboard shell
- [ ] Order history on the account page (depends on Phase 3 checkout existing)

## Phase 3 — Checkout + payments (not started)

- [ ] Real checkout flow (address, shipping, coupon, totals)
- [ ] Order-creation server function (recomputes totals/stock server-side)
- [ ] Razorpay order creation + signature verification + webhook handling
- [ ] Cash on Delivery path
- [ ] Order confirmation + tracking

## Phase 4 — Admin dashboard, polish, SEO, deployment (not started)

