---
author:
- David Kirschenheuter
date: '20.06.2018'
subtitle: Karten ohne Lizenzprobleme
title: 'Mittagskolloquium: Open-Data und andere Daten für Archäologische Karten'
---

\
[****]{}

[Problemfeld 1]{}

-   **Hintergrundkarten**

    -   Zur Visualisierung werden oft Hintergrundkarten benötigt

[Problemfeld 1]{}

-   **Hintergrundkarten**

    -   Zur Visualisierung werden oft Hintergrundkarten benötigt

[Problemfeld 2]{}

-   **Fernerkundungsdaten (z.B. Höhendaten, Landnutzung)**

    -   Für (landschaftsarchäologische) Analysen werden Rasterdaten
        benötigt\
        \

    -   Woher nehmen, wenn nicht stehlen?

        -   [Google? OSM (OpenStreetMap)? Fachbehörden?]{}

[Hintergrundkarten]{}

-   **OSM-Daten beziehen:**

    -   Mehr zu OSM: <http://learnosm.org/de/osm-data/>

    -   Geofabrik: [www.geofabrik.de](www.geofabrik.de) als Shape-File

        -   [Nachteil: große Datenmenge]{}

        -   [Nachteil: Shapefiles nur für kleine Regionen]{}

        -   [Vorteil: Daten sind bereits gefiltert/klassifiziert]{}

    -   Hot Export Tool: <https://export.hotosm.org>

        -   [Nachteil: Registrierung bei OSM erforderlich]{}

        -   [Nachteil: Nur begrenzte Anzahl an Datenmengen auf ein mal
            herunterladbar]{}

        -   [Vorteil: Daten können vor dem Download gefiltert werden
            -&gt; keine großen Downloads, schnelles Verarbeiten]{}

[Hintergrundkarten]{}

-   **OSM-Daten beziehen:**

    -   QGIS

        -   [Nachteil: Rohdaten, große Datenmengen.]{}

        -   [Nachteil: Download scheitert manchmal, dann via geofabrik
            als .osm.bz2 herunterladen]{}

        -   [Vorteil: Daten liegen lokal als Datenbank vor, erlaubt
            Filterung]{}

        -   [Vector-&gt;Openstreetmap-&gt;Download Data]{}

        -   [Vector-&gt;Openstreetmap-&gt;Import Topology from XML]{}

        -   [Vector-&gt;Openstreetmap-&gt;Export Topology to
            SpatialLite]{}

[Fernerkundungsdaten]{}

-   **Höhendaten**\
    Hillshades, Höhenlage, Exposition, Hangneigung, Topographische
    Dominanz

    -   Lidar: Bis zu 1m -&gt; Landesamt für Denkmalpflege

    -   SRTM: Bis zu 25m -&gt; Deutsches Zentrum für Luft- und Raumfahrt
        (DLR)

    -   Projekt Copernicus: Open Data, im Aufbau

[Fernerkundungsdaten]{}

-   **SRTM**\

    -   SRTM-Daten vom DLR:

        -   [Infos:
            <http://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5515/9214_read-17716/>]{}

        -   [Download nach Registrierung:
            <https://geoservice.dlr.de/egp/>]{}

        -   30m Auflösung, nur Mosaic, d. h. keine flächendeckenden
            Daten

    -   SRTM-Daten aus den USA (Geological Survey = USGS)

        -   [Infos: <https://lta.cr.usgs.gov/SRTM1Arc>]{}

        -   [Download nach Registrierung:
            <https://earthexplorer.usgs.gov/>]{}

        -   [30m Auflösung, weltweit flächendeckende Daten]{}

[Fernerkundungsdaten]{}

-   **SRTM-Daten nutzen**\

    -   Download als TIFF

    -   Import in QGIS als Rasterdatei

    -   Ggf. Reprojizieren

    -   Raster -&gt; Analysis -&gt; DEM (Terrain Models)\
        -&gt; Hillshade, Slope, TPI, Aspect...

    -   Raster -&gt; Extraction -&gt; Contour... = Höhenlinien bzw.
        Isolinien

[Fernerkundungsdaten]{}

-   **SRTM-Daten nutzen**\

    -   Werte extrahieren, z.B. Höhenangaben für Fundstellen:

        -   [Vektordaten laden]{}

        -   [Toolbox öffnen]{}

        -   [z.B. SAGA “Add- Raster values to points”]{}\

        -   Points = Fundstellen und Grid = Raster

        -   Ergebnis kann z.B. als .csv exportiert und dann in
            Statistikprogrammen ausgewertet werden

[Fernerkundungsdaten]{}

-   **Bodenkunde**

    -   Zur Analyse der Bodenformen- und typen eignen sich
        bodenkundliche Karten\
        \
        Bodenübersichtskarte 1:200.000 (BGR, Bundesanstalt für
        Geowissenschaften und Rohstoffe 2008)

[Fernerkundungsdaten]{}

-   **Bodenkunde**

    -   Download als Shapefile im Productcenter des BGR
        <https://produktcenter.bgr.de/terraCatalog/Start.do>

    -   anschließend mit einem Point-Sampling-Tool in QGIS (u.A. “Add
        Grid Values to Points” die Werte an den Fundstellen ermitteln
        und mit statistischen Programmen auswerten

[Fernerkundungsdaten]{}

-   **Moderne Landnutzung**

    -   Daten zur modernen Landnutzung: CORINE Landcover

    -   Auskunft über Erhaltung und Vollständigkeit der prähistorischen
        Landschaft

    -   Download an mehreren Stellen, z.B. beim Copernicus-Projekt:
        <https://land.copernicus.eu/pan-european/corine-land-cover/clc-2012?tab=download>

[Fernerkundungsdaten]{}

-   **Klimadaten**

    -   Worldclim.org: Fick et al 2017.

    -   Niederschlag, Temperatur, Wind, Sonne, “Bioclimatic variables”
        AuflÃ¶sung 1km

    -   Download als GeoTIFF: <http://www.worldclim.org/>

    -   Auswertung: vergleiche SRTM-Höhendaten!

[TArchIT-GitHub-Seite]{}

-   **Zum Rekapitulieren**
