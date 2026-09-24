# Playbook data

Synthetic data created for this playbook. It follows the same shape as the data used in the official lab, with extra fields where they help the RAG quality demos.

| File | Destination | Notes |
|---|---|---|
| `cosmos/ProductCatalog.json` | Cosmos DB `ProductCatalogDB` / `ProductCatalog` (partition key `/id`) | 68 products, same fields as the official index, plus `ProductDescription` and `FormattedPriceWithDollarSign` |
| `blob/customerloyalty/Zava_Customer_Loyalty_Profiles.md` | Blob container `customerloyalty` | 10 loyalty profiles. Joe is Platinum with 32.40% |
| `blob/customerloyalty/Zava_Loyalty_Program.md` | Blob container `customerloyalty` | Tier rules, discount ranges, and Black Friday campaign |
