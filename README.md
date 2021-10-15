# UrbanXTools

## **Language**
[Chinese]()
[Engilish]

##  **Content**
  * [**介绍**](#介绍)
  * [**安装步骤**](#安装步骤)
  * [**演示**](#演示)
  * [**工具内容**](#工具内容)
  * [**许可证**](#许可证)


## **Introduction**
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/intro.png)
### 1. Main Functions
- **Autogeneration of spatial models**: by integrating urban planning logics and computer algorithms, UrbanXTools can rapidly generate rudimentary spatial models for urban design projects. The spatial model will be complied with superior plans and regulations.
- **Assessment of urban design projects**: UrbanXTools can provide instant assessment of urban design projects based on multi-disciplinary features and sustainable development goals.
- **Construction of a feedback loop**: by using parametric design methods, we aim to construct a mechanism for regulatory plans and urban design projects to get instant assessments, feedbacks and modifications. With this mechanism, the efficiency and quality of urban design could be enhanced

### 2. Objectives
- High quality
- Sustainable urban development
### 3. Developers
- Tao Yang, Weizhen Luo, Xuhui Lin, Chengru Deng, Yufei Dong
### 4. Translating Contributor
- Yihan Zhang
### 5. Notifications
- Rhino version 6.14 and above are recommended. 
- Model unit MUST BE METER, and models cannot be generated if your model unit is millimeter (mm)
- Please put your geometric objects, such as roads and land parcels, near the origin of coordinates (0, 0, 0). Confined by computation accuracy of geometric objects in RhinoCommon, the geometric Boolean operation might go wrong if you put your model too faraway from the origin point.
- If you encounter any other problems or have any demands and suggestions, please let us know via Github Issues. We'll try our best to help.


## **Installation**
- Download UrbanXTools：
	- Lanzou NetDisk
		- Link：https://wwe.lanzoui.com/b01tqy68f
		- Password: h5d8
	- Baidu NetDisk
		- Link：https://pan.baidu.com/s/1acBnxjOD2pCm4wnlYHIOzg  
		- Password：gz4u
	- Github
		- Link：https://github.com/CAUPDxUrbanXLab/UrbanXTools/releases
### 1. Enter Releases, choose a compatible version, download the zip file and extract (please choose the latest version)

- Click to enter Releases

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_000.png)

- Within the Releases page, please download:
	- Full version: UrbanXTools_v3.0.0 is recommended
	
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/releaseVersion.png)

- Extract the zip file: UrbanXTools_v3.0.0

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_002.png)

### 2. Open Grasshopper in Rhino, enter Components Folder

- Open Rhino and then Grasshopper, open File --> Special Folders --> Components Folder

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_003.png)

- Copy and paste the whole UrbanXTools_v3.0.0 folder here
- If you already have UrbanXTools_v.1.0.0 or UrbanXTools_v.2.0.0 in this folder, please delete them in advance.


![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_003_1.png)

### 3. Check your UrbanXTools_v3.0.0 folder and then restart Rhino

- Make sure every file listed below are also in your UrbanXTools_v3.0.0 folder

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_004.png)

### 4. Finish

- If you have successfully installed UrbanXTools, you'll get this in your Grasshopper

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_005.png)



## **Samples**
### 1. Network Structure
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E7%A9%BA%E9%97%B4%E7%BB%93%E6%9E%84%E8%AE%A1%E7%AE%97%E6%BC%94%E7%A4%BA.gif)

[Sample: NetworkAnalysis](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/1_NetworkAnalysis)

### 2. Aided Regulatory Planning
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%85%AC%E6%9C%8D%E8%A6%86%E7%9B%96%E6%BC%94%E7%A4%BA.gif)

[Sample: AidedRegulatoryPlanning](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/2_FacilityLocation)

### 3. Urban Design Autogeneration
- Residential buildings

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90%E6%BC%94%E7%A4%BA_%E4%BD%8F%E5%AE%85%E8%A1%8C%E5%88%97%E5%BC%8F%2B%E7%82%B9%E5%BC%8F.gif)

- Commercial buildings + Warehouses + Factories

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90%E6%BC%94%E7%A4%BA_%E5%95%86%E4%B8%9A%2B%E4%BB%93%E5%82%A8%2B%E5%B7%A5%E5%8E%82.gif)

[Sample: UrbanDesign_SingleSite](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/3_UrbanDesign)

[Sample: UrbanDesign_MultiSitesSites](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/3_UrbanDesign)

### 4. Coverage Analysis of Public Facilities

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%B5%84%E6%BA%90%E8%8D%B7%E8%BD%BD.gif)

[Sample: FacilityLocation](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/4_ResourcesDemand)

### 5. Sustainability Analysis of Urban Design Projects

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%87.png)

[Sample: Resources Demand](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/5_SpatialAnalysis)

### 6. Exposure Rate Analysis of Urban Design Projects (2D)

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%873D.png)

[Sample: ExposureRates2D](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

### 7. Exposure Rate Analysis of Urban Design Projects (3D)

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%873D_mesh.png)

[Sample: ExposureRates3D](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

### 8. Exposure Rate Analysis of Urban Design Projects (3D_Mesh)

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/VisSyntax.png)

[Sample: ExposureRates3D_mesh](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

### 9. Visual Graph Network Analysis of Urban Design Projects

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/VisSyntax.png)

[Sample: ExposureRates3D_visualGraphNetwork](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)


## **Tools**

### 1. Network Structure

> Network_RoadsSplitter

- **Purpose**：
    - Clean and split the curves to handle degeneracies, such as overlaps, identical shapes, invalid curves, etc.
- **Input**：
    - Original curves
- **Output**：
    - Cleaned and split curves
- **Sample**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)

> NetworkStructure_Computing3D
- **Purpose**: 
    - This command computes network properties, including angular distance and metric distance in space syntax. You may choose different radius for calculation.
    - Betweenness: Within a certain distance, this command finds the shortest paths between any pair of points and counts the number of times each road segment is passed.
    - Closeness: Within a certain distance, compute the average distance from this point to a specified destination point along the shortest paths.
- **Input**: 
    - Road network of 2D or 3D geometries
    - Radius
    - Merging or not
- **Output**: 
    - Metric choice
    - Metric integration
    - Metric mean depth
    - Metric total depth
    - Angular choice
    - Angular integration
    - Angular mean depth
    - Angular total depth
    - Normalized angular choice(NACH)
    - Normalized angular integration(NAIN)
    - Cleaned road-segments
- **Sample**:

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


NetworkStructure_SiteAccessibility
- **Purpose**:
    - This command computes the accessibility scores of sites
- **Input**:
    - Cleaned road segments
    - Accessibility scores of each road segment
    - Curves of site boundaries
- **Output**:
    - Polygons generated by site boundaries
    - Accessibility scores of sites, with the same sequence as polygons above
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


NetworkStructure_RoadDensity
- **Purpose**: 
    - Compute road density within the given boundary
- **Input**: 
    - Roads to be computed
    - Boundary
- **Output**: 
    - Road Density (numeric data)
    - Road Density (unit: km/km²）
    - Road segments "cookie-cut" (intersected) by the given boundary
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


2. Regulatory Planning
RegulatoryPlanning_GeneratingSites
- **Purpose**:
    - Automatically generate sites polygon based on the input road network
- **Input**:
    - A list of primary roads
    - A list of secondary roads (optional)
    - A list of tertiary roads (optional)
    - A list of branch roads (optional)
    - Width of roads in the order from primary roads to branch roads
    - Radius for rounding the site corners
    - The boundary within which sites will be generated
- **Output**:
    - All generated site polygons
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


RegulatoryPlanning_ClusteringBlocks
- **Purpose**:
    - Clustering a set of sites based on the shortest-path distance matrix by using Hierarchical Agglomerative Clustering (HAC) algorithm
- **Input**:
    - Roads
    - Sites
    - Diameters for each clustering levels
- **Output**:
    - Links for visualizing the hierarchical relationships among the clusters
    - Id for each site in the tree structure to represent the hierarchy of all clusters
    - An object containing all the information of the clustering results to be used in the RegulatoryPlanning_LanduseAllocation component
- **Sample**:
 
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)

RegulatoryPlanning_ClusteringPoints
- **Purpose**:
    - Clustering a set of sites based on the euclidean distance matrix among all centroids of the sites by using Hierarchical Agglomerative Clustering (HAC) algorithm
- **Input**:
    - Centroids of each site
    - Diameters for each clustering levels
- **Output**:
    - Links for visualizing the hierarchical relationships among the clusters
    - Id for each site in the tree structure to represent the hierarchy of all clusters
    - An object containing all the information of the clustering results to be used in the RegulatoryPlanning_LanduseAllocation component
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)

RegulatoryPlanning_LanduseAllocation
- **Purpose**:
    - Automatically allocating landuse to each of the sites
- **Input**:
    - Sites
    - Accessibility scores with different radius for each site (Recommended: 3 branches)
    - The object containing all the information of clustering results, which is obtained from the RegulatoryPlanning_ClusteringBlocks component
    - Landuse structure, with the order representing their priority, and their values indicating their proportion of area among all the sites respectively (Format: R:0.2)
- **Output**:
    - Sites, wihch may be split after the landuse allocation to fulfill the requirement of landuse structure
    - Allocated landuse for each site, with the same sequence as the sites above
    - Actual landuse structure
    - The object containing all the results of landuse allocation, which is useful for the RegulatoryPlanning_FarAllocation component
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


RegulatoryPlanning_FarAllocation
- **Purpose**:
    - Automatically allocating floor area ratio (FAR) to each of the sites
- **Input**:
    - The object containing all the results of landuse allocation, obtained from the RegulatoryPlanning_LanduseAllocation component
    - Total building area for the overall urban design
    - Building area structure, represented by the percentage of building area of each category of landuse
- **Output**:
    - Allocated FAR for each site
- **Sample**:
 
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


3. Urban Design
UrbanDesign_SiteParameter
- **Purpose**: 
    - This command autogenerates site parameters based on roads, accessibility scores and site info.
- **Input**:
    - Cleaned roads
    - Accessibility scores for each road segment
    - Curves of site boundaries
- **Output**:
    - Initial parameters for all the sites
- **Sample**:

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)

UrbanDesign_SiteParameterExtra
- **Purpose**:
    - This command allows you to adjust site parameters, such as FAR and building density
- **Input**:
    - Initial parameters of all sites, obtained from the UrbanDesign_SiteParameter component
    - Landuse Type (R:0, C:1, GIC:2, M:3, W:4)
    - FAR
    - Density
    - Mixed Ratio
    - Building Styles
        - For residential buildings: 0-Rows, 1-Dots
        - For non-residential buildings: 0-Dots, 1-Groups, 2-Mixed
    - Orientation of buildings (Unit: Radians)
- **Output**: 
    - Adjusted parameters for each site
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


UrbanDesign_SiteGeneratePlans
- **Purpose**:
    - This command autogenerates building entities.
- **Input**:
    - Adjusted parameters for all sites, obtained from UrbanDesign_SiteParameterExtra component
    - City ID
- **Output**: 
    - The object containing results of the design, which is useful for the Sustainability Analysis module
    - Curves of original site boundaries (not split)
    - FARs
    - Building densities
    - Subsite boundaries
    - Setback boundaries for each site
    - Outline curves of the floor layer of each building
    - Outline curves of each building roof
    - Numbers of levels of each building
    - Brep geometries of each building
    - Functions of each brep of each building, corresponding to building breps
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


4. Facility Analysis
FacilityAnalysis_ConnectToNetwork
- **Purpose**:
    - Connect all sites to their nearest road segments
- **Input**:
    - Cleaned road network
    - Sites
- **Output**: 
    - Generic parameters, which is useful for the FacilityAnalysis_CoverageArea component
    - New road segments after computing the connection
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


FacilityAnalysis_CoverageArea
- **Purpose**:
    - Compute facilities' coverage area by shortest-path distances in the road network based on a given radius
- **Input**: 
    - Generic parameters, obtained from the FacilityAnalysis_ConnectToNetwork component
    - Sites where public facilities locate
    - Service radius of the facilities, which is defined as shortest paths within the road network
- **Output**:
    - Sites within facilities' coverage area
    - Centroids of all covered sites
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


5. Sustainability Analysis
SustainabilityAnalysis_Energy
- **Purpose**:
    - Compute the energy consumption for each building in the autogenerated plan
- **Input**:
    - Generic parameters containing the original results of the design, obtained from UrbanDesign_SiteGeneratePlans component
- **Output**: 
    - Energy consumption of each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_EnergyCarbonEmissions
- **Purpose**:
    - Compute the carbon emissions for generating the given amount of energy
- **Input**:
    - Energy consumption (Unit: kWh/year)
- **Output**: 
    - Carbon emissions for generating the given amount of energy (Unit: tCO2/year)
- **Sample**:

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_Water
- **Purpose**: 
    - Compute the water consumption for each building in the autogenerated plan
- **Input**: 
    - Generic parameters containing the original results of the design, obtained from UrbanDesign_SiteGeneratePlans component
- **Output**: 
    - Water consumption of each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_Waste
- **Purpose**: 
    - Compute waste production for each building in the autogenerated plan
- **Input**: 
    - Generic parameters containing the original results of the design, obtained from UrbanDesign_SiteGeneratePlans component
- **Output**: 
    - Waste production of each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_WasteCarbonEmissions
- **Purpose**: 
    - Compute the carbon emissions for waste treatment
- **Input**: 
    - Domestic waste generation which requires further treatment (Unit: tons/year)
    - Method of waste treatment (0-"waste_landfill", 1-"waste_incineration", 2-"waste-composting")
- **Output**: 
    - Carbon emissions for waste treatment (Unit: tons CO2/year)
- **Sample**:
 
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_EnergyCustom
- **Purpose**: 
    - Compute energy consumption of buildings based on the custom input
- **Input**:
    - Building breps
    - Building functions of each brep
- **Output**:
    - Energy consumption for each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_WaterCustom
- **Purpose**: 
    - Compute water consumption of buildings based on the custom input
- **Input**: 
    - Building breps
    - Building functions of each brep
- **Output**: 
    - Water consumption for each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_WasteCustom
- **Purpose**: 
    - Compute waste production of buildings based on the custom input
- **Input**:
    - Building breps
    - Building functions of each brep
- **Output**:
    - Waste production for each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


SustainabilityAnalysis_Population
- **Purpose**:
    - Estimated population of each residential building
- **Input**:
    - Building breps
- **Output**: 
    - Estimated population of each building
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


6. Visibility Analysis
VisibilityAnalysis_ExposureRate2D
- **Purpose**: 
    - By analyzing its relationship to road intersections, this command returns 2D exposure rate for ground floor commerce, which could be a quantified spatial feature considered in commercial site selection process.
- **Input**: 
    - Building breps
    - Preset view points
    - Normalize or not
    - Radius of viewshed
    - Subdivision (higher value will lead to higher accuracy but also longer runtime)
- **Output**:
    - Outlines of building breps
    - Exposure rate for brep outlines
- **Sample**:

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)

 

VisibilityAnalysis_GenerateMeshBuilding
- **Purpose**:
    - Convert buildings from Rhino Brep to DMesh according to subdivision. This command aims to improve computational efficiency.
- **Input**: 
    - Rhino Brep of buildings
    - Subdivision (default as -1) (higher value will lead to higher accuracy but also longer runtime)
- **Output**: 
    - GenerateMesh Class
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


VisibilityAnalysis_GenerateMesh
- **Purpose**:
    - Convert geometry from Rhino Mesh to DMesh. This command aims to improve computational efficiency.
- **Input**: 
    - Mesh
- **Output**: 
    - GenerateMesh Class
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


VisibilityAnalysis_ExposureRate3DBuildings
- **Purpose**:
    - By analyzing its relationship to view points, this command returns 3D exposure rate for buildings, which could be a quantified spatial feature considered in commercial site selection process.
- **Input**: 
    - Preset view points
    - GenerateMesh Class
    - View range in each point as radius (default as 300)
- **Output**:
    - Colored side mesh of each building
    - Uncolored top mesh and bottom mesh
    - Count of each mesh got intersected
    - Exposure rates for each view point
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


VisibilityAnalysis_ExposureRate3DMesh
- **Purpose**:
    - By analyzing its relationship to view points, this command returns 3D exposure rate for mesh entities which could be a quantified spatial feature considered in commercial site selection process.
- **Input**: 
    - Preset view points
    - GenerateMesh Class
    - View range in each point as radius (default as 300)
- **Output**:
    - Colored Mesh
    - Count of each mesh got intersected
    - Exposure rates for each view point
- **Sample**:
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


VisibilityAnalysis_VisualCalc
- **Purpose**:
    - Compute the visibility of road network by interpolating points in 3D context
- **Input**:
    - Preset road network
    - GenerateMesh Class
    - Subdivision of roads to be divided (Unit: meter, default: 500m)
    - View range in each point as radius (default as 300)
    - Output Mesh or not
- **Output**: 
    - Cleaned roads, which is useful in the VisibilityAnalysis_VisualSyntaxComputing component
    - Viewpoints on roads
    - Visibility properties of each road
    - Colored mesh (depending on whether you choose to output mesh)
- **Sample**:
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


VisibilityAnalysis_VisualSyntaxComputing
- **Purpose**: 
    - Compute visual graph network analysis by input road network and corresponding scores in 3D context
- **Input**: 
    - Cleaned roads, obtained from the VisibilityAnalysis_VisualCalc component
    - Corresponding scores of each road
    - Radius (default as -1, which leads to global calculation)
- **Output**:
    - Visual total depth
    - Visual mean depth
    - Visual integration
    - Visual choice
    - Normalized visual integration
    - Normalized visual choice
- **Sample**:
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)


### 6. WaterPipeNetwork_Calculation（Coming Soon）
<details>
<summary> WaterPipeNetwork Parameters</summary>

> Water_InpFileToGeometry
- **Purpose**：
- **Input**：
- **Output**：
- **Sample**：

> Water_CalculateSiteDemand
- **Purpose**：
- **Input**：
- **Output**：
- **Sample**：

> Water_NetworkOptimization
- **Purpose**：
- **Input**：
- **Output**：
- **Sample**：

</details>


## **License**
### ***GNU General Public License v.3***
*Copyright (C) 2020  Tao Yang, Weizhen Luo, Xuhui Lin, Chengru Deng*

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
