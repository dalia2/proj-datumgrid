# PROJ-DATUMGRID

The files in this package can be unpacked in the PROJ data directory.
For an installed PROJ this may be /usr/local/share/proj or /usr/share/proj
on unix style operating systems.

Note that this package includes "CTable2" format grid shift files for
NAD27 in the USA and require PROJ 4.8.0 or newer.  On the plus side there
is no need to compile ascii files into binary files with this version as
CTable2 files are not system dependent (as distinct from the CTable files
produced in PROJ 4.7.0 and older).

## About the Datum Grid package

The datum grid package for PROJ is maintained on the OSGeo proj-datumgrid
repository on [GitHub](https://github.com/OSGeo/proj-datumgrid).
All grids in the package are released under
permissives licenses. New grids are accepted into the package as long as
they are released under a license that is compatible with the [Open Source
Definition](https://opensource.org/osd-annotated) and the source of the grid
is clearly stated and verifiable. Suitable licenses include:

  * Public domain
  * X/MIT
  * BSD 2/3/4 clause
  * CC0
  * CC-BY (v3.0 or later)
  * CC-BY-SA (v3.0 or later)

## Horizontal grids

2-dimensional transformation grids for horizontal datum shifts.

### Australia: AGD66 -> GDA94

*Source*: [ICSM](https://github.com/icsm-au/transformation_grids)  
*Format*: NTv2  
*License*: [Creative Commons Attribution 4.0]((https://creativecommons.org/licenses/by/4.0/))

Full national coverage two-way transformation file – see Appendix B
in the [GDA2020 Technical Manual](http://www.icsm.gov.au/gda/tech.html) for details.

* A66_National_13_09_01.gsb

### Australia: AGD66 -> GDA94

*Source*: [ICSM](https://github.com/icsm-au/transformation_grids)  
*Format*: NTv2  
*License*: [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)

Full coverage two-way transformation file in those states that
originally adopted AGD84 - West Australia, South Australia, Queensland
- see Appendix B in the [GDA2020 Technical Manual](http://www.icsm.gov.au/gda/tech.html)
for details.

* National_84_02_07_01.gsb

### Australia: GDA94 -> GDA2020

*Source*: [ICSM](https://github.com/icsm-au/transformation_grids)  
*Format*: NTv2  
*License*: [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)

Full national coverage two-way transformation files – See Sections 3.2
and 3.7 in the [GDA2020 Technical Manual](http://www.icsm.gov.au/gda/tech.html) for details.
Table 3.4 details which grid to use.

* GDA94_GDA2020_conformal.gsb
* GDA94_GDA2020_conformal_and_distortion.gsb

### USA: NAD27 -> NAD83

*Source*: USGS  
*Format*: CTable2  
*License*: Public Domain

* alaska - Alaska
* conus - Conterminous U.S.
* hawaii - Hawaii
* prvi - Puerto Rico, Virgin Is.
* stgeorge - St. George Is, Alaska
* stlrnc - St. Lawrence Is., Alaska
* stpaul - St. Paul Is., Alaska

### USA: NAD83 -> NAD83

*Source*: USGS  
*Format*: CTable2  
*License*: Public Domain

Grid data for high precision conversion of geographic coordinates from
NAD83 to NAD83.

* FL - Florida
* MD - Maryland
* TN - Tennessee
* WI - Wisconsin
* WO - Washington, Oregon, N. California

### Canada: NAD27 -> NAD83

*Source*: [Natural Resources Canada](http://www.nrcan.gc.ca/earth-sciences/geomatics/geodetic-reference-systems/18766)  
*Format* NTv1  
*License*: Public Domain
* ntv1_can.dat

Grid conversion from NAD27 to NAD83 in Canada

### France: NTF -> RGF93

Grid transformation from NTF to RGF93 in France.

*Source*: [IGN](http://www.ign.fr/)  
*Format*: NTv2  
*License*: Public Domain

* ntf_r93.gsb

### Germany: DE_DHDN -> ETRS89

*Source*: [BKG](http://crs.bkg.bund.de/crseu/crs/descrtrans/BeTA/de_dhdn2etrs_beta.php)  
*Format*: NTv2  
*License*: Free redistribution is allowed and welcome

Grid transformation from DE_DHDN to ETRS89 in Germany.

* BETA2007.gsb

## Vertical grids

1-dimensional transformation grids for vertical datum shifts.

### Denmark: GRS80 ellipsoidal heights -> DVR90 heights

*Source*: [Agency for Data Supply and Efficiency](https://github.com/NordicGeodesy/NordicTransformations)  
*Format*: GTX  
*License*: [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)

Transform ellipsoidal heights to the local height system DVR90. The horizontal
grid coordinates are referenced to ETRS89.

* dvr90.gtx

### Faroe Islands: GRS80 ellipsoidal heights -> FVR09

*Source*: [Agency for Data Supply and Efficiency](https://github.com/NordicGeodesy/NordicTransformations)  
*Format*: GTX  
*License*: [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)

Transform ellipsoidal heights to the local height system FVR09. The horizontal
grid coordinates are referenced to ETRS89.

* fvr09.gtx

### Greenland: GRS80 ellipsoidal heights -> GVR2016

*Source*: [Agency for Data Supply and Efficiency](https://github.com/NordicGeodesy/NordicTransformations)  
*Format*: GTX  
*License*: [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)

Transform ellipsoidal heights to the local height system GVR2016. The horizontal
grid coordinates are referenced to GR96.

* gvr2016.gtx
