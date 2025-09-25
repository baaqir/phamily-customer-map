# Customers Map (Phamily)

An interactive USA map showing customer distribution by state (hover a state to see customer names) and customer dots.

## How to run locally
Open `customers_map.html` in a browser.

## Deploy to Vercel (static hosting)

1. Create a new GitHub repo and add `customers_map.html` to the root.
2. In Vercel, **New Project** → **Import Git Repository** → pick your repo.
3. Set **Framework Preset** to **Other** and **Output Directory** to `/` (root).
4. Deploy. Vercel will serve the static HTML at your project URL.

### Alternative: Next.js wrapper
If you want this embedded in a Next.js app:
- Create a page that injects the HTML, or
- Use `react-plotly.js` to render the same figure directly in React.

## Data
The map is generated from `customers.csv` with the following expected columns:

- `Organization Name`
- `Customer Type`
- `City`
- `State` (two-letter codes, e.g., CA, NY; supports multi-state like `KY, IN`)
- `Org Specialty`

