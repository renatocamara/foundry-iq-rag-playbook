# Lab assets

Files provided with the official TechLab environment (originally under `C:\FabricIQLab` on the lab VM), plus the storage content that the lab environment pre-provisions.

| Folder | Content | Where it is used |
|---|---|---|
| `Ontology/` | `retail_ontology_package.iq`, `fabriciq_ontology_accelerator-0.1.0-py3-none-any.whl`, `Zava Black Friday Return Policy.docx` | Uploaded to the **Files** section of the Fabric Lakehouse (Task 1.3) |
| `Notebooks/` | `Generate Lakehouse Data.ipynb` | Imported into the Fabric workspace to create the Lakehouse tables (Task 1.4) |
| `agents-build/` | `agents.py`, `parameters.env`, `requirement.txt` | Creates the Rewards Campaign, Sales Associate, and Inventory agents (Task 4.3) |
| `storage/customerloyalty/` | `customer-loyalty-data.txt` | Blob container `customerloyalty`, indexed by the `customer-loyalty-data` knowledge source (Task 3.1) |
| `storage/returnpolicy/` | `Zava Black Friday Return Policy.docx` | Blob container `returnpolicy` found in the lab environment (not used by the lab steps) |

> The official lab also pre-provisions a product catalog in Azure Cosmos DB (`ProductCatalogDB` / `ProductCatalog`, 68 items), indexed as `product-catalog-index`. A synthetic equivalent is available in [`../data/cosmos/ProductCatalog.json`](../data/cosmos/ProductCatalog.json).

## Notes

- `parameters.env` ships with a model name that may not exist in your project. Set it to one of your deployments before running `agents.py`.
- Fill `parameters.env` locally and do not commit real endpoints or connection IDs.
