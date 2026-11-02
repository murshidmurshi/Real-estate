# PropIntel — lightweight competitor comparison

A small Next.js frontend for comparing real estate listings captured from public webpages with a bookmarklet. It analyzes the captured listing details with Mistral; it does not use Mistral web search and has no database or backend.

## Run

- `npm install`
- `npm run dev`
- Open the local URL printed by Next.js.

## Use

1. Enter your own website and competitor listing URLs (or add suggested Dubai competitors).
2. Drag **PropIntel Capture** to the browser bookmarks bar.
3. Visit a listing/search page on each domain and click the bookmarklet. Paste each copied JSON object into **Captured page data**, one object per line.
4. Choose **Analyze & compare all websites**. Mistral processes only the captured content and the entered URLs; it does not browse or fetch pages.

Results, captures, and the API key are saved in this browser. Browser-entered API keys can be viewed by scripts running on localhost; use a server-side proxy before public deployment. Captured pages may expose only details rendered in the page DOM, and results reflect asking prices rather than completed transactions.
