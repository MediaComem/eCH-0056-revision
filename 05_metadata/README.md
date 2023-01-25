# Metadaten
## Meeting notes

## Date & Time

24-01-2023 09:30 - 12:30

## Attendees

| First & Last names  | Organisation   |
|---------------------|----------------|
| Raphaël Arnaud      | swisstopo      |
| Maxime Collombin    | HEIG-VD        |
| Pasquale	Di Donato |	swisstopo      |
| Romelli Fidi        | Kt.Schaffhausen|
| Michel Gysi         | swisstopo      |
| Frank	Gottsmann	  | swisstopo      |
| Oliver Grimm        | Geowerkstatt   |
| Jens Ingensand	  | HEIG-VD        |
| Ken Kaufmann        |	Ruag           |

## Next meeting

| 23.02.23 | Styles & misc topics |
|----------|-------------|

## Presentation

The workshop starts with a presentation by Jens Ingensand of the results of the last workshop and the current status of standards, specifications and implementations.
Pasquale Di Donato then presented the results of the POC aimed at creating a tile service from custom resolution levels compliant with the swisstopo WMTS.
The choice fell on sourcepole's [t-rex](https://t-rex.tileserver.ch/) solution for the server part (backend) & [OpenLayers 7.2](https://openlayers.org/) for the client part (frontend).
It specifies that a [file](https://github.com/t-rex-tileserver/t-rex/tree/master/tile-grid) available in the source code allows tiles to be generated according to a custom tile matrix.

Following the presentation, the following exchanges took place.

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Romelli Fidi        | - Is it possible to establish a connection in QGIS ?                         |
| Pasquale Di Donato | - It doesn't work with QGIS but it should work with Leaflet. |
| Maxime Collombin    | - He mentions that it is possible to establish a connection to an OGC API Tiles collection in QGIS thanks to its GDAL driver.<br> - He also mentions that an [example](https://ogc.heig-vd.ch/oa-tiles/OGC-API-Tiles/#access-ogc-api-tiles-from-qgis-through-gdal) is included in the NGDI-20-60 OGC API Testbed Platform.  |
| Maxime Collombin    | - He proposes to integrate the tile matrix set into the OGC registry. |
| Pasquale Di Donato | - He agrees but proposes to do so once version 4.0 of eCH-0056 is published. |

Maxime Collombin follows with a presentation on Metadata.
Following the presentation, the following exchanges took place.

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Pasquale Di Donato | - He mentioned that section 6.4 was missing from the presentation material. |
| Maxime Collombin    | - He projects the linked information via the browser and will modify the slides. |

Pasquale Di Donato then presented the associated recommendations.
Following the presentation, the following exchanges took place.

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Pasquale Di Donato | - He mentioned that the META-04 recommendation is not possible for the WMS and WMTS standards and that this requires an extension. |
| Maxime Collombin    | - He mentions that it is possible with pygeoapi (early implementation of OGC API Records). |
| Maxime Collombin    | - He  asks if we should  keep the META-04 recommendation for the revision (which will probably not include OGC API Records.) |
| Pasquale Di Donato | - He proposes to keep the recommendation but as optional. |
| Romelli Fidi        | - Romedi asked if it is possible to reference metadata and associated services for each layer of a WxS service. |
| Pasquale Di Donato | - He says yes and then makes a demonstration using the swisstopo WMS.  |
| Oliver Grimm        | - He asks if it is coherent to provide metadata for each collection/layer? |
| Oliver Grimm        | - He proposes to modify META-01 & META-02 to make them more generic. |
| Raphaëlle Arnaud    | - She proposes to delete the mapping for all the WxS services and to update the GM03 Profil accordingly. |
| Pasquale Di Donato | - He agrees with the proposal and mentioned that one should ask less to get more.  |
| Pasquale Di Donato | - He mentions that the url for accessing collections is poorly constructed and should include metadata information (e.g.`collections/metadata/collectionId`) |

Raphaëlle Arnaud follows with a presentation on GM03.
Following the presentation, the following exchanges took place.

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Maxime Collombin    | - Maxime asks how much harvesting is involved in Geocat. |
| Raphaëlle Arnaud    | - She mentions that 30% of the information is entered via the Geocat interface and 70% obtained by harvesting. |
| Jens Ingensand      | - He proposes to add recommandations about harvesting & SEO in the eCH-0056. |

The discussion then turned to the question of the eCH process and the integration of the new OGC standards.

| First & Last names  | Considerations                         |
|---------------------|----------------------------------------|
| Pasquale Di Donato  | - He mentions that the eCH-0056 should be more flexible and integrates changelog. |
| Pasquale Di Donato  | - He asks what to do with the newly approved OGC standards. |
| Romedi Fidi         | - He asks what should be done with the standards being currently in a draft status. |
| Oliver Grimm        | - He mentions that the eCH-0056 process should be more agile & tools ready. |
| Jens Ingenand       | - He mentions that all of the OGC API standards are not all on the same level. Some are apporved, others are still in a draft stage. |
| Pasquale Di Donato  | - He asks more specifically what to do with OGC API Features. |
| Romedi Fidi         | - He mentions that it is important to know the new standards and mechanisms for the cantons. |
| Ken Kaufmann        | - He asks which software manufacturers already support these standards. |
| Jens Ingenand       | - He mentions that this was mentioned in the context of the presentation of the HEIG-VD at the last FOSS4G edition. |
| Oliver Grimm        | - He proposes to add recommendations as soon as a new OGC standard is adopted. |
| Romedi Fidi         | - He mentions that the recommendations are not binding enough. |
| Pasquale Di Donato  | - He proposes to add `or <standard reference>` for new standards rather than recommendations. |
| Maxime Collombin    | - He proposes proposes to add a reference to the versions of the eCH-0056 document in the "Conformance Declaration" endpoint of the related standards. |
| Pasquale Di Donato  | - He asks if it is not an extension to the standard if we do this. |
| Maxime Collombin    | - He replies that the standard mentions that the implementation must contain a declaration of conformity but that there is a degree of freedom as to its content. |
| Frank Gottsmann     | - He proposes to raise this need for agility in the eCH-0056 process at the IMS kick-off meeting. |
| Oliver Grimm        | - He mentions that one should be able to state that from now on the standard is there and the tool support is there. <br> - He proposes to add a modulisarisation to the eCH-0056 processes like OGC APIs. |
| Ken Kaufmann        | - He asks what is the degree of acceptance of new standard. <br> - He adds that the financial impact should not be underestimated and that one should motivate people with the use of new standard. <br> - He then says that one should think how to reduce the resistance to change. <br> - It finally adds that it is important to keep existing systems running long enough. |
|Romedi Filli         | - He suggests to presents the NGDI OGC API Testbed Platform in a KGK dedicated workshop. |

The disscussion finally turned to the organisation of next meeting. It will be dedicated to the challenges of styling & cartographic representations. For the sake of efficiency, other themes will potentially be addressed.

## Conclusion

The meeting ended at around 14:30.
The CPT members would like to warmly thank all the stakeholders for their active participation and look forward to future exchanges in the revision of the eCH-0056 standard.
