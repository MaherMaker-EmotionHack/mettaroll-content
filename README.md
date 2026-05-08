# Mettaroll Content

CMS content for [mettaroll.com](https://mettaroll.com) — managed via [Decap CMS](https://decapcms.org/).

## Structure

```
content/           # Markdown + YAML source files
  en/              # English content
  ar/              # Arabic content
  de/              # German content
  nl/              # Dutch content
  settings/        # Site-wide settings (general.yml)
public/uploads/    # Media assets (images uploaded via CMS)
admin/             # Decap CMS admin UI (config.yml + index.html)
```

## Editing Content

1. Go to [mettaroll.com/admin/](https://mettaroll.com/admin/)
2. Log in with your GitHub account
3. Edit pages, products, team members, or UI strings
4. Save — changes are committed to this repo automatically
5. The website rebuilds and deploys within ~3-5 minutes

## Local Development

To run the CMS locally:

```bash
npx decap-server
```

Then open `http://localhost:4200/admin/` (requires the main site running locally).

## Collections

| Collection | Path | Description |
|---|---|---|
| Pages | `content/{lang}/pages/` | Home, About, Contact, Products, Privacy Policy |
| Products | `content/{lang}/products/` | Individual product pages |
| Product Categories | `content/{lang}/product-categories/` | Category groupings |
| Team | `content/{lang}/team/` | Team member profiles |
| UI Strings | `content/{lang}/ui.yml` | Navigation, buttons, labels |
| Settings | `content/settings/general.yml` | Site-wide configuration |
