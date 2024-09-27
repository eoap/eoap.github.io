# References

## Common Workflow Language (CWL)

CWL User Guide, a guide to introduce you to writing workflows using the CWL open standards

* User guide available at: https://www.commonwl.org/user_guide/

**Specification and standards**

* Common Workflow Language specification: https://www.commonwl.org/specification/
* Common Workflow Language Standards, v1.2: https://www.commonwl.org/v1.2/
* Common Workflow Language Standards, v1.1: https://www.commonwl.org/v1.1/
* Common Workflow Language Standards, v1.0.2: https://www.commonwl.org/v1.0/

## OGC documents

* OGC 20-089r1 Best Practice for Earth Observation Application Package: https://docs.ogc.org/bp/20-089r1.html
* OGC 20-073: OGC Earth Observation Applications Pilot: Summary Engineering Report: http://docs.opengeospatial.org/per/20-073.html
* OGC 20-042: OGC Earth Observations Applications Pilot: Terradue Engineering Report: http://docs.opengeospatial.org/per/20-042.html

## SpatioTemporal Asset Catalogs

* **STAC Item** is the core atomic unit, representing a single spatiotemporal asset as a GeoJSON feature plus datetime and links: https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md
* **STAC Catalog** is a simple, flexible JSON file of links that provides a structure to organize and browse STAC Items. A series of best practices helps make recommendations for creating real world STAC Catalogs: https://github.com/radiantearth/stac-spec/blob/master/catalog-spec/catalog-spec.md
* **STAC Collection** is an extension of the STAC Catalog with additional information such as the extents, license, keywords, providers, etc that describe STAC Items that fall within the Collection: https://github.com/radiantearth/stac-spec/blob/master/collection-spec/collection-spec.md
* **STAC API** provides a RESTful endpoint that enables search of STAC Items, specified in OpenAPI, following OGC's WFS 3: https://github.com/radiantearth/stac-api-spec