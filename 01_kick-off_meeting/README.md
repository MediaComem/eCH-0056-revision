# Kick-off meeting
## Meeting notes

## Date & Time

11-10-2018 09:30 - 16:00

## Attendees

| First & Last names | Organisation                         |
|--------------------|--------------------------------------|
| Beat Tschanz       | SGS, swisstopo (KOGIS)               |
| Frank Gottsmann    | Geostandards.ch, swisstopo (KOGIS)   |
| Jens Ingensand     | HEIG-VD                              |
| Marco Bernasocchi  | OPENGIS.ch                           |
| Maria Klonner      | swisstopo                            |
| Maxime Collombin   | HEIG-VD                              |
| Oliver Grimm       | Geowerkstatt                         |
| Pasquale Di Donato | swisstopo (KOGIS)                    |
| Pia Bereuter       | FHNW                                 |
| Raphaël Bovier     | swisstopo                            |
| Raphaëlle Arnaud   | swisstopo                            |
| Rémy Baud          | swisstopo                            |
| Stefan Ziegler     | Amt für Geoinformation Kt. Solothurn |

## Next meeting

| 04-11-2022 | Vector Data |
|------------|-------------|

## Core Project Team

The meeting started with an introduction of the revision project and the members of the Core Project Team (CPT):

| First & Last names  | Organisation                       |
|---------------------|------------------------------------|
| Frank Gottsmann     | Geostandards.ch, swisstopo (KOGIS) |
| Peter Staub         | Geostandards.ch, KGK               |
| Jens Ingensand      | HEIG-VD                            |
| Olivier Ertz        | HEIG-VD                            |
| Maxime Collombin    | HEIG-VD                            |
| Pasquale Di Donnato | swisstopo (KOGIS)                  |
| Beat Tschanz        | SGS, swisstopo (KOGIS)             |

## Stakheolders' round of introductions

Stakeholders were invited to introduce themselves as well as their specific interests in the revision project.

| First & Last names  | Needs and considerations           |
|---------------------|------------------------------------|
| Beat Tschanz       |- In order to guarantee the interconnection between cantonal, national and federal data infrastructures, the legal aspect is important.<br>- It must also be ensured that the geoservices are accessible and usable.<br>- A new direction needs to be given to download services.<br>- A transitional phase must be considered.<br>- The review process must be clear and consensual.|
| Marco Bernasocchi  |- Standardisation is an important topic for clients.<br>- Standardisation is a very important topic for the OSGeo board.<br> - It must ensure the interoperability of software solutions.<br>- How far should the "Helvetisation" go? |
| Maria Klonner      |- It is important to consider the IFC standard.<br>- What could be the influence on cadastral surveying?|
| Oliver Grimm      |- A lot of work has been carried out on INTERLIS.<br>- It is important to keep a practical perspective on standardisation.<br>- Methodology is important.|
| Pasquale Di Donato |- The eCH-0056 process should be simple and agile.<br>-"Helvetisation" is not appropriate.|
| Pia Bereuter       |Standardisation, interoperability and semantics are important topics for academic research.|
| Raphaël Bovier     |- Swisstopo disseminates all kinds of data.<br>- Geoservices are increasingly important.<br>- The geoservices of the BGDI must comply with the eCH-0056 standard.<br>- It is difficult to guarantee a high level of performance within the current normative framework.<br>- It is important that standards are up to date with new technologies.<br>- Big data standards should be considered|
| Raphaëlle Arnaud   |- Standardisation is important for Geocat.ch<br>- The revision of the GM03 standard is underway.<br>- The next workshop will take place in November.<br>- Do not overcomplicate the standard.<br>- Keep it as simple as possible.|
| Rémy Baud          |- Tiled services (esp. tile matrices) are important for the military geodata infrastructure.<br>- It is important to look at new technologies.<br>- The ecH-0056 standard must be adapted.<br>- Swisstopo can provide data |
| Stefan Ziegler     |- It is important to consider users and service providers.<br>- How far should the "Helvetisation" go?<br>- "Helvetise" as little as possible|

## Presentation of GeoStandards.ch

The session continued with the presentation of [Geostandards.ch](https://geostandards.ch/) by Frank Gottsmann.

The associated presentation items can be found [here](https://mediacomem.github.io/eCH-0056-revision/01_kick-off_meeting/index.html#9).

In terms of highlights, it was mentioned that the leaderships of the themes: *Standardisierung* and *Tools* have yet to be assigned.

## Legal framework 

Frank Gottsmann then spoke about the legal aspects of the eCH-0056 standard.

The associated presentation items can be found [here](https://mediacomem.github.io/eCH-0056-revision/01_kick-off_meeting/index.html#19).

The following exchanges followed:

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Pasquale Di Donato |- NGDI organisations should comply with the eCH-0056 standard                                       |
| Frank Gottsmann    |- They can't be forced to do so.                                                                    |
|Raphaël Bovier      |- NGDI, BGDI, MGDI Geoservices are quite compliant, but there are services that are not included in eCH-0056<br>- It is important to update the standard so that they can be compliant.<br>- The eCH-0056 standard should be adapted more regularly so that the (N-B-M)GDI can offer compliant services.<br>- Can non-approved standards be incorporated into the process?                                                              |
|Beat Tschanz        | - Geoservices would also work without a standard.<br>- We need to define the standards that are useful.<br>- It is important to ensure that they are used.<br>- Currently, the impact of eCH-0056 is not "pervasive".<br> Weneed to think about how do we achieve that impact.<br>- Propose best practice can make sense.|
| Stefan Ziegler     |- The current process (6 years) is too long.<br>Standards should not be made on theory but based on practice.<br>- Nobody uses Atom Feeds.|
| Pia Bereuter       |- Standards should be developed on the basis of a needs analysis.                                   |
| Beat Tschanz       |-  An official standard of representation should be defined.<br>- The standardisation process needs to be redefined and updated|

```mermaid
stateDiagram
    direction LR
    Geostandards.ch --> eCH#8211;0056 
    BGDI,#10240;MGDI,#10240;NGDI --> Geostandards.ch  
```

## Which standard to choose ?

A discussion took place on the standards to be considered in the revision of the eCH-0056 document.

| First & Last names |                     Considerations                  |
|--------------------|-----------------------------------------------------|
|   Raphaël Bovier   | - The standards should be choosen according to the associated national SDI (NGDI, BGDI, MGDI) and associated data & services |
|    Beat Tschanz    | Portrayal und Download Services are to be considered|
| Marco Bernasocchi  | - According to the OGC, OGC APIs are build on the legacy of WxS.<br>- Preferring only OGC APIs would be wrong.<br>- What are the weak points of the WMS standard?|
| Stefan Ziegler     | - Printing                                          |
| Raphaël Bovier     | - How do we make way for new standards?<br>- Do we simply want to update existing standards or see what the need is?<br>- We are missing out on new technologies (e.g. 3D Mesh).|
| Marco Bernasocchi  | - Should we consider "nice to have"?                |
| Beat Tschanz       | - Minimal requirements should be defined<br>- The availability and quality of services should be considered.<br>- Atom feeds are not used and can therefore be deleted.|
| Stefan Ziegler     | - No one follows the recommendations for mapping metadata (GM03) elements.|
| Raphaël Arnaud     | - The section on metadata in eCH-0056 refers to the harmonisation of metadata described in the GM03 standard currently under revision.                                           |
| Pasquale Di Donnato | - Geopackage should not be considered as a standard  |
| Frank Gottsmann    | - A more agile and faster process must be defined<br>- It is proposed to include the standards under development in a backlog in an annex to eCH-0056.|

## Document structure and process adaptation

A discussion took place on the drafting process and the current structure of the eCH-0056 document.

| First & Last names |                     Considerations                  |
|--------------------|-----------------------------------------------------|
| Beat Tschanz       | - The revision process should be iterative and propose minor and major changes.<br>- The document structure has to ba adapted.|
| Pia Bereuter       | - Comprehensibility is important.<br>- Standard should point the way.<br>- Configuration options should be integrated.|
| Maria Klonner      | - Best practice should be the basis                 |
| Frank Gottsmann    | - Maturity is an important indicator.<br>- In order to integrate new standards not yet validated, a variant would be that version 3.0 remains in use and that a version 4.0 is complementary.|
| Beat Tschanz       | - The current structure of eCH-0056 is too restrictive and does not lend itself well to some standards.|
| Oliver Grimm       | - eCH-0056 should be a guide and propose a gentle impact to clarify open questions| 
| Beat Tschanz       | - Versions should be prescribed including minor changes (release management).<br>- Minimal requirements should remain : Download / Search / Display.<br>- But the process should definitively be more agile.|
| Frank Gottsmann    | - The process will be adapted.<br>- It will take into account specific national needs<br>- A selection of standards will be considered as backlog to allow for a continuous revision process.| 

## Selection of standards

A discussion took place on some additional elements to be included to the eCH-0056 document.

### Discussion

| First & Last names  |                     Considerations                                   |
|---------------------|----------------------------------------------------------------------|
| Maria Klonner       | - Reference frame & Height reference system should not be forgotten. |
| Pasquale Di Donnato | - Delivering INTERLIS-GML via WFS is a very complex task and it's not supported by every GIS Server.                 |
| Beat Tschanz        | - STAC can be used to upload INTERLIS files                          |
| Stefan Ziegler      | - One should have feature services that can be used.                 |
| Beat Tschanz        | - Adress and transformation services must be considered              |
| Pasquale Di Donnato | - Address services should be integrated                              |
| Raphaël Bovier      | - COG should be considered to ensure optimised data downloads        |

### Decisions

The discussions resulted in the following decisions:

| Standard type |             Standard            |                           Decision                              |
|:-------------:|:-------------------------------:|-----------------------------------------------------------------|
|     Vector    |         OGC API Features        | - Should be integrated into the document<br>- Could replace WFS |
|     Vector    |               STAC              | - To be discussed during the dedicated Workshop.                |
|     Raster    |           OGC API Maps          | - Should be integrated in a backlog or annex document           |
|     Raster    |        OGC API Coverages        | - Should be integrated in a backlog or annex document           |
|     Raster    |           OGC API EDR           | - Should be integrated the document                             |
|     Tiles     |          OGC API Tiles          | - Should be integrated in a backlog or annex document           |
|     Tiles     |          Tiling Schema          | - Should be integrated in a backlog or annex document           |
|    Metadata   |               GM03              | - Dedicated standard under revision.                            |
|    Styling    |          OGC API Styles         | - Should be integrated in a backlog or annex document           |
|    Styling    | Symbology Conceptual Core Model | - Should be integrated in a backlog or annex document           |
|    Diverses   |           OGC GeoPose           | - Should be integrated in a backlog or annex document           |
|    Diverses   |          OGC Geopackage         | - To be discussed during the dedicated Workshop.                |
|    Diverses   |        OGC API Processes        | - To be discussed during the dedicated Workshop.                |
|    Diverses   |       OGC SensorThings API      | - To be discussed during the dedicated Workshop.                |
|    Diverses   |           Linked Data           | - To be discussed during the dedicated Workshop.                |
|    Diverses   |   Cloud Optimized Data Formats  | - To be discussed during the dedicated Workshop.                |
|    Diverses   |         Reference frame         | - Remove LV03                                                   |
|    Diverses   |            Atom Feeds           | - To be discussed.                                               |


### Additional standards and case studies

In addition to this list, it was decided to consider additional use cases and standards that might be interesting to study. 

These use cases and standards will be discussed in dedicated workshops.

|       Use case, data type      |                                                                                     Standard, Link[^1]                                                                                    |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 3D point clouds                | [COPC](https://copc.io/)                                                                                                                                                                  |
| 3D picture                     | [GeoPose](https://github.com/opengeospatial/GeoPose)                                                                                                                                      |
| Height reference system        | [LN02](https://www.swisstopo.admin.ch/en/knowledge-facts/surveying-geodesy/reference-frames/local/ln02.html)                                                                              |
| Address service, Geocoding API | [Geocoding API](https://www.ogc.org/projects/groups/geocodeapiswg)                                                                                                                        |
| Building 3D models             | [IFC](https://www.iso.org/standard/70303.html), [CityGML](https://www.ogc.org/standards/citygml), [CityJSON](https://docs.ogc.org/cs/20-072r2/20-072r2.html)                              |
| 3D mesh                        | [OGC WCS](https://docs.opengeospatial.org/is/17-089r1/17-089r1.html), [OGC API Coverages](https://ogcapi.ogc.org/coverages/), [OGC API 3D GeoVolumes](https://ogcapi.ogc.org/geovolumes/) |
| Data historization             | ?                                                                                                                                                                                         |
| Positioning service (swipos)   | [swipos-GIS/GEO](https://www.swisstopo.admin.ch/en/geodata/geoservices/swipos/swipos-dienste/swipos-gisgeo.html)                                                                          |
| Quality                        | [INTERLIS 2](https://www.interlis.ch/en/dokumentation/interlis-2), [eCH-118](https://ech.ch/de/ech/ech-0118/2.0)                                                                          |
| [Calculation and transformation service](https://www.swisstopo.admin.ch/fr/cartes-donnees-en-ligne/calculation-services.html)| [OGC API - Processes](https://ogcapi.ogc.org/processes/)                                   |
|                 ?               |[Cloud Optimized GeoTIFF](https://www.ogc.org/standards/requests/254)                                                                                                                                          |

[^1]: this list can of course be extended (e.g. with the results of the [GeoUnconference #4](https://github.com/GeoUnconference/discussions/discussions/8#discussioncomment-3857483))

## Miscellaneous

| First & Last names |                     Considerations                           |
|--------------------|--------------------------------------------------------------|
| Raphaël Arnaud     | - An invitation (outlook) to the workshops would be appreciated.|
| Pasquale Di Donnato| - It is proposed to use github to review the report. <br>- The current version will be converted to asciidoc and integrated into a repository.git |

## Conclusion

The meeting ended at around 16:00.
The CPT members would like to warmly thank all the stakeholders for their active participation and look forward to future exchanges in the revision of the eCH-0056 standard.
