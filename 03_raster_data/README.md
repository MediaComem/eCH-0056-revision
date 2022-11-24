# Raster Data
## Meeting notes

## Date & Time

22-11-2022 09:30 - 14:30

## Attendees

| First & Last names | Organisation                         |
|--------------------|--------------------------------------|
| Frank Gottsmann    | Geostandards.ch, swisstopo (KOGIS)   |
| Jens Ingensand     | HEIG-VD                              |
| Jürgen Hansmann    | swisstopo                            | 
| Marco Bernasocchi  | OPENGIS.ch                           |
| Maxime Collombin   | HEIG-VD                              |
| Oliver Grimm       | Geowerkstatt                         |
| Pasquale Di Donato | swisstopo (KOGIS)                    |
| Rémy Baud          | swisstopo                            |
| Romelli Fidi       | Kt.Schaffhausen                      |
| Stefan Ziegler     | Amt für Geoinformation Kt. Solothurn |
| Zimil Bordoloi     | Stadt Luzern                         |

## Next meeting

| 22-12-2022 | Tiles       |
|------------|-------------|

## OGC API Maps

Jens Ingensand presents the main differences between WMS and OGC API Maps and points out that the standardisation process is not very advanced for OGC API Maps.
An important point is that the GetFeatureInfo operation would no longer be included in OGC API Maps. More information can be found [here](https://github.com/opengeospatial/ogcapi-maps/issues/81).

The following exchanges take place:

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| All                | - The participants were surprised.                                                                 |
| Stefan Ziegler     | - The GetFeatureInfo operation is very important for the users.<br>The core team should mentions this need to the OGC.|
| Romelli Fidi       | - This issue should not affect the next version of eCH-0056.                                       |

### OGC API EDR

Jens Ingensand presents the OGC API EDR and its main components.

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Pasquale Di Donato |- Pasquale asks if it is possible to use this standard to obtain elevation profiles.<br>He mentions that the solution currently in place does not comply with OGC standards.|
| Maxime Collombin   |- Maxime proposes to implement a small POC on the TB Platform.                                      |
| Rémy Baud          |- Rémy asks for clarification on the resource queries.                                              |
| Maxime Collombin   |- Further information can be found [here](https://docs.ogc.org/is/19-086r5/19-086r5.html#toc28).    |

### WMTS vs OGC API Tiles

Jens Ingensand presents OGC API Tiles and mentions that it has just been approved. He points out the TileSet is the main component of this standard.

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| All                | - It is agreed that this should be included in the next version of eCH-0056.                       |
| Pasquale Di Donato | - How to integrate both WMTS and OGC API Tiles in the revision?                                    |
| Marco Bernasocchi  | - The same question arises for WFS and OGC API Features.                                           |
| Frank Gottsmann    | - Frank proposes to address this issue later.                                                      |
| Pasquale Di Donato | - Pasquale asks if the resolution levels are appropriate.                                          |
| All                | - Everyone confirms that this is the case.                                                         |

### Cloud-Natives formats

Jens Ingensand presents different examples of cloud native formats.

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| All                | - Everyone agrees that it should not be integrated into the eCH-0056 document.                     |
| Stefan Ziegler     | - Stefan argues that it is not relevant to address recommendations for encodings otherwise there will be requests for any kind of format.|
| Marco Bernasocchi  | - Organisations and individuals use formats that meet their needs.                                 |
| All                | - Examples & showcases on the TB platform could however be interesting.                            |

### Evaluationskriterien Matrix

Jens presents the evaluation matrix defined during the first workshop.

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Pasquale Di Donato | - Some points are clear, others less so.<br> - What does "suche" mean?<br> - Is it at the level of a collection or an item?<br> - What is meant by "Vernetzung"?<br> - Aspect to be better defined.<br> - It is currently a bad idea to address linked data. |
| Stefan Ziegler     | - Proposes to keep a technology watch and not to lose sight of good practices for the future.<br> - Who is responsible for technology watch?|
| Frank Gottsmann    | - SOGI Fachgruppe                                                                                   |
| Pasquale Di Donato | - What is KGK's opinion on AtomFeeds?<br> - Do you agree to delete it?                              |
| Romedi Filli       | - Ok                                                                                                |
| Jens Ingensand     | - What is your opinion Stefan?<br> - Can you tell us more about your [article](https://www.linkedin.com/pulse/graalvm-polyglot-superpowers-1-spatiotemporal-asset-stefan-ziegler/?trackingId=HSb33M3ASMuz8mMrHubFLw%3D%3D)?                       |
| Stefan Ziegler     | - AtomFeeds was a very good idea.<br> - The flop is that it couldn't be put into practice.           |

## Proposals for changes from the Core Project Team 

Jens Ingensand presents the proposals for changes from the Core Project Team.

### CRS-02

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Jens Ingensand     | - IS [PROJ](https://proj.org/) enough?                                                             |
| All                | - Specialists should be consulted before making a decision.                                        |

### LANG-01

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| All                | - Ok                                                                                               |

### LANG-02

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| All                | - Not necessary to make a distinction                                                              |

### LANG-04

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| All                | - To be deleted                                                                                    |

#### WMTS-07

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Rémy Baud          | - Is it possible to define additional levels of resolution (x2)?<br> - Why do we have gaps?<br> - Mentions a problem with the tiles origin.        |
| Jens Ingensand     | - The resolution levels are indexed to the national map which is the reference for all base maps.|
| Pasquale Di Donato | - We need someone who is an expert to tell us if the levels of resolution are consistent.        |
| Jens Ingensand     | - Mentions a tiles overlay problem for the TileSet defined on the Geoserver service of the TB platform.|
| Marco Bernasocchi  | - Mentions that this problem is mentioned in the [WMTS specification (p. 8-9)](https://portal.ogc.org/files/?artifact_id=35326).|
| Maxime Collombin   | - Will check whether this is also included in the OGC API Tiles specification and discuss it with SWG members if appropriate.|
| Oliver Grimm       | - Mention that the definition of the tileset is an important point to guarantee an optimal display of the different services (WMTS & OGC API Tiles)|

## Miscellaneous

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Pasquale Di Donato | - It would be nice to test the [OGC 3D Tiles](https://docs.opengeospatial.org/cs/18-053r2/18-053r2.html) specification.|
| Pasquale Di Donato | - Mentions a need regarding address research.                                                       |
| Maxime Collombin   | - Mentions the [Geocoding API SWG](https://www.ogc.org/projects/groups/geocodeapiswg).              |
| Jens Ingensand     | - Jens points out that no standards currently exist.                                                |

## OGC API TB Platform

An exchange finally takes place on the subject of the NGDI 20-60 OGC API Testbed Platform.

| First & Last names |                     Considerations                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------|
| Jürgen Hansmann    | - Jürgen asks for more details about the NGDI 20-60 project.                                         |
| Jens Ingensand     | - The project is integrated into the resources dedicated to the INDG.<br>- It resulted in the deployment of the test platform.<br>- The results were presented during the last FOSS4G edition and will be presented during the next swisstopo kolloquium.<br>- However, the project has come to an end and no further funding is available. |
| Jürgen Hansmann    | - Jürgen asks if the platform will be maintained.                                                   |
| Romelli Fidi       | - Romelli asks how the interaction with the OGC will continue and how the TB platform will be maintained.|
| Jens Ingensand     | - This will depend on the funding.                                                                       |

## Conclusion

The meeting ended at 14:30.
The Core Project Team members would like to warmly thank all the stakeholders for their active participation and look forward to future exchanges in the revision of the eCH-0056 standard.
