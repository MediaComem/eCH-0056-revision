# Vector Data
## Meeting notes

## Date & Time

04-11-2022 09:30 - 16:00

## Attendees

| First & Last names | Organisation                         |
|--------------------|--------------------------------------|
| Beat Tschanz       | SGS, swisstopo (KOGIS)               |
| Frank Gottsmann    | Geostandards.ch, swisstopo (KOGIS)   |
| Jens Ingensand     | HEIG-VD                              |
| Maxime Collombin   | HEIG-VD                              |
| Oliver Grimm       | Geowerkstatt                         |
| Peter	Staub        | Geostandards.ch, KGK                 |
| Romelli Fidi       | Kt.Schaffhausen                      |
| Zimil Bordoloi     | Stadt Luzern                         |

## Meeting notes

Frank Gottsmann presents the format of meeting notes on GitHub. This seems to fit everyone. Frank add that a issue should be opened for any modification request.

## Opinion KGK

Peter Staub clarified the position of the KGK, which had been forwarded in advance of the kick-off meeting because neither he nor Dominic Kottsman could attend.

| First & Last names | Considerations                         |
|--------------------|----------------------------------------|
| Peter Staub        | - It is important to consider which standards and versions are useful.<br>- What is no longer relevant?<br>- What's up (in production)?<br>- Important to consider WxS standards in new eCH-0056 version.    |
| Jens Ingensand     | - OGC API Maps is not a validated standard yet.|
| Romedi Filli       | - Should WxS standards still be used?          |
| Maxime Collombin   | - the document ecH-0056 must comply with the requirements<br>- The revision process should be scalable and linked to technological developments. | 
| Beat Tschanz       | - It is important to identify what is not or what is no longer relevant.<br>- One must anticipate technological change.                          |
| Zimil Bordoloi     | - It is important to identify what is not or what is no longer relevant.<br>- One must anticipate technological change.<br>- Software developments should be considered.<br>- The reviewing process should be agile.<br>Standards also condition the softwares development.                        |
| Romedi Filli       | - swisstopo no longer wants Atom feeds.<br>- STAC should be included in the eCH-0056 new version.<br>- An important thing is that we can stick to standards.<br>With STAC something is coming and Atom Feeds can then drop out.|

## GeoIG und GeoIV

Beat Tschanz reminds that the eCH-0056 standard is cited in the GeoIV and that it specifies which standards are to be considered.

## Grafik Unconference

Frank Gottsmann presents a [sketch](https://github.com/GeoUnconference/discussions/discussions/8#discussioncomment-3912691) which is the result of the reflections of a small group that participated in GeoUnconference #4.

Peter and Oliver made the following additions:

| First & Last names | Considerations                         |
|--------------------|----------------------------------------|
| Peter Staub        | - Linked data (jsonld) allow to connect the different services. | 
| Oliver Grimm       | - OGC APIs are becoming more webby and could serve that purpose. |    

## OGC API Building Blocks

Jens Ingensand specifies that OGC API Commons is the common architecture.

## Goals of the workshop

Frank Gottsmann reminds that the goal is to define what works well and what works less well.

## Evaluation Matrix

Frank Gottsmann presents the evaluation matrix.

## Presentation of the NGDI 20-60 project

Jens Ingensand mentions that the results of the project will be presented at the next swisstopo kolloquium taking place in december.

## STAC

Romedi Filli states that STAC can document raster data as well as any other format.

## Search Service:

Oliver Grimm proposes to add a section on SEO optimization as well as citing the [Section 11](https://www.w3.org/TR/sdw-bp/#why-are-traditional-sdi-not-enough) of the Spatial Data on the Web Best Practices.


## OGC API testbed plaform

The testbed platform is considered as a good tool to test the OGC APIs.
It would be great if it could be maintained any longer on.

## Transformation Dienste

In addition to the discussion on transformation services at the kick-off meeting, the following additions were made:

| First & Last names | Considerations                         |
|--------------------|----------------------------------------|
| Beat Tschanz       |- [Reframe](https://www.swisstopo.admin.ch/fr/cartes-donnees-en-ligne/calculation-services/reframe.html) is a tool for the cantons<br>- There is no point in mentioning it in the eCH-0056 document. |
| Maxime Collombin   |- What about integrating INTERLIS validations as OGC API Processes?|

## Kick-off meeting: décisions

The results of the kick-off meeting were presented and the following discussion took place.

| First & Last names | Considerations                         |
|--------------------|----------------------------------------|
| Zimil Bordoloi     | - OGC API Maps is not very advanced and should be integrated in the backlog document.|
| Jens Ingensand     | - OGC API Tiles is quite advanced, might be soon approved.|
| Beat Tschanz       | - What is the use of Atom Feeds?       |
| Jens Ingensand     | - Atom Feeds are not really used.      |
| Beat Tschanz       | - OGC API Styles is not very advanced and should be integrated in the backlog. |
| Romedi Filli       | - MGM & Darstellungsmodelle are important    |
| Jens Ingensand     | - mentions the following [discussion](https://github.com/GeoUnconference/discussions/discussions/8#discussioncomment-3054970) in the GeoUnconference forum.    | 
| Beat               | - Darstellungsmodelle are not really used. |

## Standards & uses cases

The results of the kick-off meeting were presented and the following discussion took place.

| First & Last names | Considerations                         |
|--------------------|----------------------------------------|
|Maxime Collombin    | - The information about data Historization must be updated<br>- [OGC API Features](https://docs.opengeospatial.org/is/17-069r4/17-069r4.html#_parameter_datetime) includes the `datetime` parameter|
| Beat Tschanz       | - Data historization should not to be considered<br>- REFRAME should not to be considered<br>- the notion of standard quality too<br>- Point clouds should not be considered<br>- 3D pictures should not be considered<br>- LN02 should be removed<br>- Adressservices should be looked at<br>- 3D Gebäudemodelle should not be considered<br>- 3D Mesh: should be looked at<br>- Positioning services should be removed as well as section 6.13<br>- Quality: INTERLIS files via STAC                        |

## Evaluation criteria

A discussion took place on the standards to be considered in the context of the eCH-0056 revision.

| First & Last names | Considerations                         |
|--------------------|----------------------------------------|
| Peter Staub        | - One should integrates the notion of transaction<br>- WFS-T is not part of the actual eCH-0056 version and can be integrated in the new version<br>- OGC API Features transaction is not yet validated but could be potentially integrated in the new version.     |
| Oliver Grimm       | - We need to be more specific<br>- The use cases are important too. |
| Jens Ingenand      | - Some of the standards discussed today will be dealt with in more detail in future workshops. | 
| Frank Gottsmann    | There should be an iterative revision of the eCH-0056 document to better accommodate the [OGC standards Roadmap](https://www.ogc.org/roadmap).                                                     |
| Beat Tschanz       | - The project core team should define what can be adapted and standardised<br>- many other services are not in the list<br>- 3 aspects are crucial<br>- metadata<br>- projection systems<br>- search services<br>- the recommandations must be result-oriented.     |
| Zimil Bordoloi     | - Demand is strong for geoservices.     |
| Beat Tschannz      | - We should look at OGC AP Tiles<br>- For Atom Feeds there is a discussion about file download (INTERLIS).|
| Romedi Fili        | - Regarding the practice GML-schema is not used. |
| Beat Tschanz       | - INTERLIS files should be included to STAC services.<br>- OGC API Styles should be included in the backlog. |

## Conclusion

The meeting ended at around 16:00.
The CPT members would like to warmly thank all the stakeholders for their active participation and look forward to future exchanges in the revision of the eCH-0056 standard.

