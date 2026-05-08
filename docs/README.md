# Esquina Latina Market — Store Data

## catalog.json

Complete product catalog exported from Shopify. Use this file to understand what products exist in the store for design decisions.

### Structure
```json
{
  "total": 151,
  "vendors": ["Brazil", "Colombia", "Costa Rica", "El Salvador", "Guatemala", "Honduras", "Nicaragua", "Peru"],
  "categories": ["Coffee", "Juice", "Soda", "Nail Polish", ...],
  "products": [
    {
      "title": "Product Name",
      "vendor": "Brazil",
      "tags": ["Coffee"],
      "status": "ACTIVE",
      "price": "7.59",
      "compare_at_price": null,
      "available": true,
      "inventory": 12,
      "image": "https://cdn.shopify.com/..."
    }
  ]
}
```

### Countries (vendors)
| Country | Flag Code | Shopify Collection Handle |
|---------|-----------|--------------------------|
| Brazil | br | `brazil` |
| Colombia | co | `colombia` |
| El Salvador | sv | `el-salvador` |
| Costa Rica | cr | `costa-rica` |
| Guatemala | gt | `guatemala` |
| Honduras | hn | `honduras` |
| Peru | pe | `peru` |
| Nicaragua | ni | `nicaragua` |

### Categories (tags)
`Achocolatados em Pó`, `Baking`, `Bebidas Lácteas`, `Biscoitos`, `Bread`, `Cereals`, `Chips`, `Chocolate`, `Coffee`, `Cookies`, `Energy Drink`, `Flours & Starches`, `Grains`, `Juice`, `Limpeza Doméstica`, `Nail Polish`, `Pasta`, `Sauce`, `Seasoning`, `Soda`, `Soups`, `Sweet Snacks`

## Notes for Claude Design
- Flag images come from `https://flagcdn.com/w80/{code}.png`
- Store URL: `esquinalatinamarket.com` (Shopify: `rbxipr-4d.myshopify.com`)
- Design tokens are in `snippets/css-variables.liquid`
- Main color: `#fafaf9` background, `#0f0f0f` foreground (neutral modern)
- Font: Plus Jakarta Sans (Google Fonts)
