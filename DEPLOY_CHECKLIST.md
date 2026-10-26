# Business Portal — Deploy Checklist

## Theme
- Dark Green + Light Green + White only
- Responsive dashboard UI

## Roles
- Super Admin
- Admin
- Buyer
- Seller
- Manufacturer
- Wholesaler
- Supplier
- Retailer
- Business Owner / Directory
- Support Staff

## Important
This package is configured for Netlify/Vite. Firebase production credentials are intentionally not embedded.

Before production use:
1. Add Firebase Web config to environment variables.
2. Configure Firebase Authentication providers.
3. Create Firestore and Storage rules using the included blueprint/rules.
4. Run `npm install` and `npm run build` locally or in Netlify.
5. Deploy `dist` using the Netlify build settings in `netlify.toml`.

Demo role switching is intended for development/testing and should be disabled or protected before public production use.
