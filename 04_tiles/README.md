# Tiles
## Meeting notes

## Date & Time

20-12-2022 09:30 - 16:00

## Attendees

| First & Last names  | Organisation  |
|---------------------|---------------|
| Frank	Gottsmann	  | swisstopo     |
| Jens	Ingensand	  |HEIG-VD        |
| Jürgen	Hansmann  |	swisstopo     |
| Ken	Kaufmann      |	Ruag          |
| Luke Seelenbinder   |	Stadia Maps	  |
| Marco	Bernasocchi	  | OPENGIS.ch    |
| Maxime	Collombin | HEIG-VD       |
| Pasquale	Di Donato |	swisstopo     |
| Pia	Bereuter      |	FHNW          |
| Rémy	Baud          |	swisstopo     |

## Next meeting

| 24.01.23 | Metadata |
|----------|----------|

## Presentation

The workshop starts with a presentation by Jens Ingensand on the current state of standards, specifications and implementations.
Following the presentation, the following exchanges took place.

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Rémy Baud           | - some clients (ESRI) do not support the zoom levels defined in the eCH-0056 standard |
| Jens Ingensand      | - Indeed, issues had already been identified in the [OGC Testbed 13](https://docs.opengeospatial.org/per/17-041.pdf)|
| Rémy Baud           | - It works for raster, not for vector tiles, and for 3D tiles it might be a problem<br> - Can OGC API tiles be produced from WMTS?|
| Jens Ingensand      | - Yes, there is software that allows you to do this |
| Maxime Collombin    | - It is important to distinguish between tile generation and OGC API Tiles  |
| Jürgen Hansmann     | - Should the definition of zoom levels be the same for raster and vector? |
| Jens Ingensand      | - Yes, it should be the same for raster and vector but it still needs to be tested|
| Frank Gottsmann     | - What are the industry's needs? |
| Luke Seelenbinder   | - exclusively visualization, some parameters are not mandatory|
| Maxime Collombin    | - Is it consistent to consider a top left corner outside the EPSG:2056 reference frame ? |
| Pia Bereuter        | - This should not be a problem |
| Rémy Baud           | - We'll just have empty tiles but that's not a problem |
| Pia Bereuter        | - The definition of the tile matrix should be provided with the service |
| Pasquale Di Donnato | - We would like to define only one tiling schema (Raster & Vector)<br> - We can have custom resolution levels<br> - We need to do a POC|
| Jürgen Hansmann     | - It is important to have the input of Petr Pridal |
| Jens Ingensand      | - Jens says he wrote to him but apparently to the wrong address
| Jürgen Hansmann     | - I will send him an email

## POC (Proof of concept)

Quelles sont les questions auxquelles on doit répondre?

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Ken Kaufmann        | - We must consider everything that is used and make an inventory of what is missing. <br> - the precision is not important but we must know if the precision is not good |
| Pasquale Di Donnato | - We must define the zoom levels for the cantons and municipalities |
| Pia Bereuter        | - Currently the zoom levels defined in eCH-0056 are not accessible anywhere. <br> - They should be made more easily accessible |
| Pasquale Di Donnato | - We should define a tile matrix and publish it to the OGC registry |
| Luke Seelenbinder   | - In the context of client-level integration, it would be interesting to consider the most widely used solutions
<br> - OpenLayers is not widely used.<br>- It would be interesting to consider ESRI
| Jens Ingensand      | - Jens mentions that this should be feasible with the ESRI JS API |
| Luke Seelenbinder   | - Luke recommends using a solution that works with PostGIS as a backend |
| Pasquale Di Donnato | - Pasquale proposes to test the combination of services configured with different resolution and top left corners. |
| Pasquale Di Donnato | - Pasquale mentions that according to the [documentation](https://docs.opengeospatial.org/is/17-083r4/17-083r4.html#toc56) that it should be possible to define resolution levels that do not necessarily take into account the power of 2. |
| Jürgen Hansmann     | - Jürgen proposes to combine WMTS (with vector & raster data), OGC API Tiles (vector & raster) with different tiling schemas. |
| Rémy Baud           | - Rémy proposes to integrate services from major data providers such as Google, Bing.           |
| Pasquale Di Donnato | - It is not necessarily coherent. We need to focus on the OGC standards and the needs of the NGDI.
| Frank Gottsmann     | - What should be the deadline ? |
| Pasquale Di Donnato | - End of Q1 (end of march)      |
| Rémy Baud           | - It is important to bring ESRI into the loop.|
| Pasquale Di Donnato | - It could be done as soon as the tileset has been defined and validated (at the end of the POC) |

### Proposed changes to eCH-0056

Pasquale Di Donnato presents the proposed changes to section 6.8: Web Map Tile Service (WMTS) of the eCH-0056 document.

| Rule    | Description                                                    |
|---------|----------------------------------------------------------------|
| WMTS-02 | no longer necessary (superfluous)                              |
| WMTS-04 | to be deleted                                                  |
| WMTS-06 | to be deleted                                                  |
| WMTS-08 | to be deleted as already defined in the OGC API Tiles standard |
| WMTS-07 | to be deleted in favour of a general rule for tiled services   |

## Conclusion

The meeting ended at around 12:30.
The CPT members would like to warmly thank all the stakeholders for their active participation and look forward to future exchanges in the revision of the eCH-0056 standard.
