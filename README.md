# Professional GIS Project Experience - TRC Companies
Geospatial Analysis for Power &amp; Utility, Transportation, and Renewable Energy industries - Through the ArcGIS platform, daily analysis of construction impacts on land use, terrain, wildlife, natural resources, and environmental changes, helping clients make well-informed decisions. 

# VISUAL SCOPE INDEXES FOR LINEAR ROUTE ANALYSIS

# Monthly Visual Scope creation for American Electric Power:
Visual scope map indexes are used for environmental impact assessments of transmission line reroutes, structure replacements, or removals
focusing on surrounding landscapes and communities, primarily in the Midwest or Southern United States.

Strip Map Index geoprocessing tool used to create a map series of existing or proposed electric transmission lines compared with hydrological,
property parcels, and geological data layers.
  - Converted AutoCAD files of proposed transmission centerlines and structures into shapefiles to display in ArcGIS Pro.
  - Symbolized structures based on material (steel or wood), by type (tangent, running angle, dead end, & substations), and status (removal or install).
    - Utilized USGS Karst Areas, Hydrographical data such as NWI wetlands, NHD streams, and FEMA Flood Hazard Layers, Rextag pipeline and powerline infrastructure, rail lines and road networks, and local property parcel data.
  - Calculated the total linear feet of the proposed transmission line, and the linear feet of portions intersecting wetland types, geological features, or crossings of surrounding power and gas infrastructure.
  - Each visual scope has an overview title page, orienting the client to the general location of the route.
  - Utilized SQL & Python script within ArcGIS to manipulate labeling, title block formatting, and dynamic text for data driven pages.

# National Grid Resource Mapping:
Presentation of TRC Delineated wetland data alongside proposed National Grid transmission lines for Environmental Resource Figures.

  - Assisted TRC wetland biologists in the field for the Wetland Delineation effort. Helped field crews locate the boundaries of wetlands and waterbodies through soil tests.
  - Plotted the boundary points through a sub-meter GPS – points of hydrography features were then later digitized within ArcGIS pro for analysis and map making.
  - Environmental data is symbolized based on National Grid standards.
  - Timber matting area estimates: resource figures allow the client to visualize the proximity of wetland and stream features to the transmission line to pinpoint areas where timber-matting may be necessary.
    - Timber matting is commonly used in transmission line projects to help stabilize work areas for heavy machinery and protect the ground underneath.
    - Once the locations of matting are picked out, typically overlapping wetlands, for a cost estimate.
- Conducted optimal access road planning for transmission line maintenance:
    - Access line data is provided in kmz., dwg., or shapefile form from the client for cost estimates and environmental impact assessment.
 
# ENVIRONMENTAL CONTAMINATION AND NATURAL DISASTER RESPONSE:

# Central Maine Power Company & Avangrid - Climate Vulnerability Assessment
Analyzed the relationship of CMP transmission lines, transformers, structures, and substations with FEMA Floodplains and NOAA Sea Level Rise data to identify risk zones, assess vulnerability, and visualize impacts of severe flood events.
  - Utilized ArcGIS pro model builder to create a workflow to intersect transmission line features with floodplain shapefiles and calculate the linear distance of overlap.
    - Transmission lines were then dissolved by section number to expose the linear feet of each section within flood layers.
  - Evaluated substations, poles, transformers, and underground manhole points in comparison to FEMA and NOAA layers.
The climate vulnerability assessment helped pinpoint locations at risk of flood damage and expose assets in need of design modifications.

# Environmental Contamination Response Mapping
GIS analysis and figure creation for a chemical spill restoration effort. Disturbed/contaminated area polygons were created based on soil and water sample points from TRC field services.
Restoration phase maps were produced to present impacted areas, prioritize remediation zones, and help the client visualize all phases of site recovery.
  - Converted a digital elevation model into contour lines to predict the flow of groundwater chemicals on site.
  - Processed disturbed area polygons with field collected data to make acreage calculations for site impact analysis.

# WIND POWER DEVELOPMENT PLANNING:

# Setback analysis for Greenbacker on Howard Wind Farm - Repowering Project in New York
The repowering project involved upgrading/replacing old turbines with more efficient models - improving energy output and lowering maintenance costs.

Prior to the setback analysis, highlighted sensitive receptor points, or locations of residence, schools, government buildings, small structures on project parcels and adjacent non-participating parcels.
  - Identifying receptors through the county parcel data helps the client minimize disturbances on the local community and ecosystem. 

Applied buffers to all wind turbine locations based on New York state laws relating to the total height of the WTG (Wind Turbine Generator) in ArcGIS pro:
  - 1.2 times the WTG height from the exterior of a participating residence receptor point.
  - 2.2 times the WTG height from the exterior of a non-participating residence point.
  - 1.1 times the WTG height from the nearest non-participating property, right of way of all public roads, and above-ground utilities. 
  - 1.5 times the WTG height from non-participating permanent non-residential structures (garages, barns, commercial buildings etc.)
  - 100 feet from NYSDEC wetlands

With the ‘arcpy’ window in ArcGIS pro, Python commands were used to symbolize the buffers based on their spatial relationship. Buffers were symbolized in green and labeled as “pass” if they did not intersect with features related to the constraint laws.
  - Any overlapping buffers of features subject to set back laws were labeled “fail” and symbolized in red. 

The wind farm consisted of 27 turbines spaced over 5,000 acres. Created a grid index map series, and a assigned a page query to show only one turbine per map. 

# Wetland Delineation Report for Enel Green Power: 
Creation of four figures for a typical TRC Wetland Delineation Report:

The wetland delineation report helps identify wetlands and soil types on site, to ensure infrastructure development follows local environmental regulations and built in a safe/stable location.
  - Figure i: USGS Topographic Site Location Map 
  - Figure ii: Soil Composition Map - Soils data extracted from the USDA Web Soils Survey; soil polygons are symbolized by ‘Hydric Rating’.
    - Acreage and percent coverage calculations made for soil types intersecting the project area.
  - Figure iii: State and Federal Wetland Resource Map - Displays on site DEC wetlands & streams, NHD flowlines, and NWI wetlands.
  - Figure iv: TRC Delineated Resources Map - TRC field services conduct a site survey on the 100-acre property in Jefferson County, NY, marking hydrographic data points with sub-meter GPS accuracy. Wetland and vernal pool vertices, streams, and various land cover types were digitized in ArcGIS Pro. Once all features are processed, accurate acreage calculations can be made for on–site wetland polygons and linear feet calculations for stream-lines. 
    - Buffered all hydrological features based on state setback laws and wetland jurisdictional status.
    - Calculated linear feet and acreage for both State & Federal and TRC Delineated streams and wetlands.

# Wind Farm Impact Analysis for Invenergy:
Provided GIS analysis and figure production for a Tier 1 and Tier 2 environmental assessments to evaluate site suitability and potential impacts of a large-scale 100,000-acre Wind Farm in the state of Iowa.

  - The tier 1 phase consists of an initial desktop assessment for potential environmental and wildlife risks before the field service efforts.
    - The preliminary GIS work begins with creation of a site location figure to orient the client on the geographic position of the survey area.
    - Figure 2: A land cover types map using raster imagery from the U.S. National Land Cover dataset
      - The land cover raster was converted to a shapefile and clipped by the 10-mile survey area buffer.
      - A separate Forested Landcover type figure was created with forested polygons symbolized by acreage intervals (0-5, 5-20, 20–50, >50)
    - Figure 3: Consisted of national hydrography data such as National Hydrography Dataset streams & waterways, and National Wetland Inventory waterbodies & wetlands.
    - Figure 4: Habitat & Conservation Map contained polygon shapefiles of Iowa state protected county, easement, and proclamation lands
  - The tier 2 phase was designed for ‘Site Characterization’ and required TRC field collected data for map production.
    - Survey data for Raptor Nest Locations, Preferred Eagle Habitat Locations, and field verified Active Eagle nest coordinates were collected and mapped in ArcPro
    - For the raptor nest survey figure, nests were symbolized by status (unoccupied/occupied) and species (Bald Eagle, Red Tail Hawk, or unknown).
      - Buffer occupied Eagle nests based on Iowa state setback laws.

# SOLAR INFRASTRUCTURE PLANNING:

# Ground mount and Rooftop Solar and Electric Vehicle Carport planning for the New York State Energy Research and Development Authority:
Towns and counties across New York have varying constraint laws and specific zoning regulations for solar development.

  - Utilized the ArcGIS pro and ArcMap software to present buildable areas for solar infrastructure in comparison to NY Rextag power networks, NYSDEC wetlands and streams, FEMA floodplains, and digital elevation models. 
    - Proper NY solar setbacks were applied to adjacent parcel boundaries, onsite structures, wetlands, and slopes greater than 15% to highlight the optimal buildable area.
    - Acreage calculations were conducted for buildable area and onsite DEC wetland polygons.

# Solar Site Suitability analysis for Sol America: 
  - USGS Site Location Maps, Environmental Constraint Maps, and Vernal Pool Survey figures created for properties in the state of Maine volunteering for solar panel installation.
  - Environmental Constraint maps consist of spatial data from the Maine Department of Inland Fisheries & Wildlife, the Maine Land Use Planning Commission, and TRC Delineated Resources. 
  - Additional Vernal Pool Survey maps with data collected by TRC wetland scientists were created to monitor biodiversity and preserve ecosystem health on-site.



