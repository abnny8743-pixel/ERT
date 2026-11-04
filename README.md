# ERT

WER

## Pages

This is a static HTML site with no build step or dependencies. The pages are linked in this order:

| Order | File | Title | Next page |
|-------|------|-------|-----------|
| 1 | `index.html` | Landing page (`الصفحة الأولى`) | `address.html` (via link) |
| 2 | `address.html` | Address details (`بيانات العنوان`) | `billing.html` (via link) |
| 3 | `billing.html` | Billing | `paymen.html` (redirects with `window.location.href`) |
| 4 | `paymen.html` | Payment | `code.html` (redirects with `window.location.href`) |
| 5 | `code.html` | Verification | — |

## Running locally

Open `index.html` in a browser, or serve the folder with any static server, for example:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000/index.html`.
