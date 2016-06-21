---
title: Team TARDIS
layout: page
concept: Time Adorned Resource Descriptions in Science (TARDIS)
---

*Working to bring the CSIRO geologic time RDF resources into several data holdings


# Team Members

  * Douglas Fils  -- Consortium for Ocean Leadership / Open Core Data
  * Bob Arko -- IEDA / SESAR
  * Alexandra Noronha -- University of Texas  
  * Anders Noren -- CSDCO 
  * Shannon Peters -- Macrostrat


# Project Goal

To take the resources from https://www.seegrid.csiro.au/wiki/CGIModel/GeologicTime
and use them to add properties to resources.  Examples are Open Core data files, 
SESAR samples and more.  

# Questions

  * How to "age" the CSDCO data:  Neotoma age models, Geo Deep Dive possible
  * Connect CSIRO/ICS and Macrostrat concepts ID's via GeoLink Graph


# Links

  * SESAR GeoLink RDF for time
  * Macrotrat;  API timescales: https://macrostrat.org/api/defs/timescales API intervals: https://macrostrat.org/api/defs/intervals 
  * CSIRO   https://www.seegrid.csiro.au/wiki/CGIModel/GeologicTime

# Steps  
  * SESAR
    * 30K samples with ages..  mix of assignment and analytic  (don't know when one or other)
    * put in prov even if it is "unknown"
    * put in URI's from SESAR graph (sample URI is associated with age URI)  (using GeoLink hasGeologicAge)
    * above is available at http://data.geolink.org/sparql in SESAR graph
  * Open Core
    * use age models to find age range of core and assign with CSIRO ICS 2014  (using GeoLink hasGeologicAge)
    * publish to GeoLink graph class dataset / digitalobject
  * General
    * create cross link to Macrostrat resources and place in GeoLink
    * Demo the utility how?

 # RDF notes

 A resource with time looks like

 ```
 <http://host.geolink.org/sesar/id/dataset/ffaf89d9-8e7f-4770-b049-224d87eb2850>
     a <http://schema.geolink.org/1.0/base/main#Dataset> ;
     rdfs:label "RC1307, Coring>PistonCorer"
     geolink:hasCruise <http://lod.bco-dmo.org/geolink/id/deployment/57413>
     geolink:hasTitle
     geolink:hasAbstract

 ```


