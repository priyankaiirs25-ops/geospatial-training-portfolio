# Practical 01 — DEM terrain analysis in QGIS

<em>Status: tutorial outline in progress. This practical is not marked as tested yet.</em>

## Aim

Create a simple terrain-analysis map from a Digital Elevation Model (DEM) using QGIS. The exercise is designed for a beginner and uses an independent example area rather than unpublished research data.

## Learning outcomes

By the end, a learner should be able to:

1. Explain what a DEM represents and identify its basic raster properties.
2. Add a DEM to QGIS and inspect its coordinate reference system (CRS), pixel size, extent, and NoData value.
3. Generate slope, aspect, and hillshade layers.
4. Apply suitable symbology and compare the terrain derivatives.
5. Prepare a map layout with a title, legend, scale bar, north arrow, data source, and CRS information.
6. Save the QGIS project and export a map.

## Software and data

- **Software:** QGIS (use a current Long Term Release where possible).
- **Input:** a small, openly licensed DEM tile covering the chosen practice area.
- **Suggested example area:** Mount Abu, Rajasthan. This is a teaching example and is not connected to the author's unpublished research.
- **Possible data catalogue:** [USGS EarthExplorer](https://earthexplorer.usgs.gov/). Check the dataset's access conditions, attribution requirements, and download format before use.

Do not upload large source rasters to this repository. Add a data-source note and, where licensing permits, a small sample or a link to the original provider.

## Workflow

### Part A — Prepare the data

1. Download a DEM tile for the selected example area from a recognised data provider.
2. Extract the downloaded archive if necessary.
3. Keep the original DEM unchanged. Work from a copy in a clearly named project folder.
4. Record the dataset name, provider, date accessed, native CRS, and pixel size.

### Part B — Inspect the DEM in QGIS

1. Open QGIS and create a new project.
2. Add the DEM using **Layer → Add Layer → Add Raster Layer**.
3. Open **Layer Properties → Information**.
4. Record the raster CRS, extent, dimensions, pixel size, band count, and NoData value.
5. Confirm that the project CRS is appropriate for the area and the measurements being made. Do not assume that changing the project CRS reprojects the raster.

### Part C — Generate terrain derivatives

Use the Processing Toolbox and search for the relevant algorithms:

- **Hillshade** — creates a shaded-relief visualisation from elevation.
- **Slope** — calculates the rate of elevation change, usually expressed in degrees or percent.
- **Aspect** — calculates the compass direction of the steepest downslope direction.

Before running each tool, inspect its input, output path, units, and other parameters. Record the settings used so another learner can reproduce the result.

### Part D — Style and compare

1. Apply a suitable single-band pseudocolour ramp to the DEM.
2. Style slope so low and high gradients can be distinguished.
3. Style aspect with a cyclic colour ramp or another clearly explained scheme.
4. Display the hillshade with suitable contrast; if overlaying it with the DEM, adjust transparency carefully.
5. Check that NoData areas are not being displayed as valid terrain.

### Part E — Make the final map

Create a print layout containing:
- a clear map title;
- the DEM or terrain-derivative map;
- legend and scale bar;
- north arrow where appropriate;
- data provider and dataset name;
- CRS, units, and map author;
- a short note explaining what the map shows.

Export the layout as a PNG or PDF.

## Quality-control checklist

- [ ] The DEM covers the intended area and has no unexpected gaps.
- [ ] CRS and pixel size have been checked and recorded.
- [ ] Slope units are stated on the map or in its caption.
- [ ] Aspect is interpreted as direction, not slope steepness.
- [ ] Hillshade is treated as a visualisation, not an elevation measurement.
- [ ] The map includes data attribution and essential map elements.
- [ ] The QGIS project reopens with its data paths intact.

## Troubleshooting notes to add after testing

Record the actual error, its cause, and the fix observed during the practical. Useful cases to investigate include:
- raster appears in the wrong location;
- raster is all one colour or appears blank;
- processing output is not created;
- slope values or units look unexpected;
- exported layout has missing layers or an unreadable legend.

## Evidence to add after completing the practical

Add original screenshots captured during the exercise:
1. DEM loaded in QGIS;
2. raster information/properties;
3. slope, aspect, and hillshade outputs;
4. final print layout;
5. exported map.

Do not add screenshots until the corresponding steps have been completed and checked.

## Data and attribution record

Complete this section after choosing and downloading the dataset.

- Dataset:
- Provider:
- Download page:
- Date accessed:
- Native CRS:
- Pixel size:
- Licence / terms:
- Required attribution:
