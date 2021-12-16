# UrbanXTools

## **Language**
[中文]
[Engilish](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/README.md)

##  **更新**
  * 增加三维实现曝光率选择范围
  * 提升道路网计算效率

##  **目录**
  * [**介绍**](#介绍)
  * [**安装步骤**](#安装步骤)
  * [**演示**](#演示)
  * [**工具内容**](#工具内容)
  * [**许可证**](#许可证)


## **介绍**
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/intro_02.png)
### 1. 主要功能
- **自动生成城市设计体块**：基于城市规划设计逻辑和计算机算法，快速生成符合上位规划管控指标的城市设计方案草模；
- **城市设计方案的评估**：基于多专业协同理念和可持续发展目标，即时对城市设计方案进行评估；
- **构建反馈机制**：依托参数化设计方法，建立控规详规与城市设计方案快速评估、反馈、修改的机制，提高设计效率与方案质量

### 2. 目标
- 高质量
- 可持续城市发展
### 3. 研发人员
- 杨滔、罗维祯、林旭辉、邓成汝、董雨菲
### 4. 注意事项
- 推荐使用Rhino version 6.9及以上版本；
- 模型单位必须使用米（model unit: meter），如使用毫米则无法进行方案自动生成；
- 如方案距离工作视图原点较远时，由于Rhinocommon几何运算精度限制，几何布尔运算有一定概率出现问题，因此请将路网地块等几何数据移动至原点（0，0，0）附近；
- 如有运行问题或功能需求，可在github issue里提出，开发者会尽力解决。

## **安装**
- 下载链接：
	- 蓝奏云盘
		- 链接：https://wwe.lanzoui.com/b01tqy68f
		- 密码: h5d8
	- 百度网盘
		- 链接：链接：https://pan.baidu.com/s/1acBnxjOD2pCm4wnlYHIOzg  
		- 密码：gz4u
	- Github下载
		- 链接：https://github.com/CAUPDxUrbanXLab/UrbanXTools/releases
### 1. 进入Release界面，选择合适版本，下载zip文件，解压并取出(版本号以最新版为准)

- 点击进入Release界面

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_000.png)

- 进入Release界面
	- 完全版：推荐选择 UrbanXTools_v3.0.0（已经包含以下多种版本）
	
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/releaseVersion.png)

- 取出文件夹：UrbanXTools_v.3.0.0

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_002.png)

### 2. 打开Rhino，打开Grasshopper，进入Component File

- 打开Rhino，打开Grasshopper，点击 File --> Special Folders --> Components Folder 

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_003.png)

- 将文件夹：UrbanXTools_v.3.0.0 置入
- 如果文件夹中存在 UrbanXTools_v.1.0.0，或 UrbanXTools_v.2.0.0 请将该文件夹全部删除，置入UrbanXTools_v.3.0.0

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_003_1.png)

### 3. 检查文件夹内容完整性，重启Rhino

- 确保文件夹里，有如下文件

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_004.png)

### 4. 顺利置入

- 如顺利置入，界面如下

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_005.png)




## **示例**
### 1. 网络结构分析
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E7%A9%BA%E9%97%B4%E7%BB%93%E6%9E%84%E8%AE%A1%E7%AE%97%E6%BC%94%E7%A4%BA.gif)

[案例: NetworkAnalysis](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/1_NetworkAnalysis)

### 2. 辅助控规
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/6_RegulatoryPlanning.png)

[案例: FacilityLocation](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/6_RegulatoryPlanning)

### 3. 城市设计方案自动生成
- 居住建筑

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90%E6%BC%94%E7%A4%BA_%E4%BD%8F%E5%AE%85%E8%A1%8C%E5%88%97%E5%BC%8F%2B%E7%82%B9%E5%BC%8F.gif)

- 商业建筑+仓库+工业建筑

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90%E6%BC%94%E7%A4%BA_%E5%95%86%E4%B8%9A%2B%E4%BB%93%E5%82%A8%2B%E5%B7%A5%E5%8E%82.gif)

[案例: UrbanDesign SingleSite](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/3_UrbanDesign)

[案例: UrbanDesign_MultiSitesSites](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/3_UrbanDesign)

### 4. 公共服务设施覆盖分析

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%B5%84%E6%BA%90%E8%8D%B7%E8%BD%BD.gif)

[案例: FacilityLocation](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/2_FacilityLocation)

### 5. 城市设计方案的可持续性分析

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/7_ResourceDemand.png)

[案例: Resources Demand](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/4_ResourcesDemand)

### 6. 城市设计方案曝光度分析（2D）

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/8_Exposure.png)

[案例: ExposureRates2D](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

### 7. 城市设计方案曝光度分析（3D）

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%873D.png)

[案例: ExposureRates3D](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

### 8. 城市设计方案曝光度分析（3D Mesh）

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%873D_mesh.png)

[案例: ExposureRates3D_mesh](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

### 9. 城市设计方案视觉图结构计算

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/VisSyntax.png)

[案例: ExposureRates3D_visualGraphNetwork](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)

## **工具**

### 1. 网络结构
 NetworkStructure_RoadsSplitter
- **目的**：
    - 清洗并分割所有道路曲线。处理的情况包括：重叠、形状相同、无效曲线等
- **输入**：
    - 待清洗和分割的道路曲线
- **输出**：
    - 完成清洗和分割的道路曲线
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadsSplitter.png)

NetworkStructure_Computing3D
- **目的**：
    - 计算道路网络性质。可选择按米制和按角度制衡量距离的方式，及不同的计算半径
    - 介数中心性（betweenness）：在指定的计算半径范围内，找出网络中任意两点的最短路径，并计算每段道路被所有这些最短路径所经过的次数
    - 紧密中心性（closeness）：在指定的计算半径范围内，从该点到所有其他点的平均最短路径距离
- **输入**：
    - 二维或三维的路网曲线
    - 计算半径
    - 是否需要合并道路（若某一节点仅与两条道路相连，则可把该节点两旁的道路合并为同一条道路）
- **输出**：
    - Metric choice
    - Metric integration
    - Metric mean depth
    - Metric total depth
    - Angular choice
    - Angular integration
    - Angular mean depth
    - Angular total depth
    - Normalized angular choice (NACH)
    - Normalized angular integration (NAIN)
    - 清洗过后的道路曲线
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_Computing.png)
 

NetworkStructure_SiteAccessibility
- **目的**：
    - 计算地块可达性
- **输入**：
    - 被清洗过的道路中心线
    - 各道路中心线所对应的可达性数值
    - 地块曲线
- **输出**：
    - 由地块曲线围合得到的地块面
    - 地块可达性得分
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_SiteAccessibility.png)
 

NetworkStructure_RoadDensity
- **目的**：
    - 基于用户给定的边界范围，计算路网密度
- **输入**：
    - 道路网曲线
    - 边界范围
- **输出**：
    - 道路网密度（纯数值）
    - 道路网密度（单位：km/km2）
    - 道路网位于边界范围以内的部分
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_RoadDensity.png)

2. 辅助控规
RegulatoryPlanning_GeneratingSites
- **目的**：
    - 在给定的边界范围内，基于道路网自动生成地块
- **输入**：
    - 城市快速路
    - 主干道（可选）
    - 次干道（可选）
    - 支路（可选）
    - 道路宽度列表（按照从城市快速路到支路的顺序）
    - 地块倒圆角的半径
    - 边界范围
- **输出**：
    - 地块面
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_GeneratingSites.png)
 

RegulatoryPlanning_ClusteringBlocks
- **目的**：
    - 基于层次聚类算法及最短路径距离矩阵，对地块进行聚类
- **输入**：
    - 道路中心线
    - 地块
    - 各等级生活圈的服务半径
- **输出**：
    - 表达聚类组团之间层级关系的连线
    - 树形结构中各个地块的ID，用于表达所有聚类组团的层级
    - 包含所有聚类结果的对象，可用于RegulatoryPlanning_LanduseAllocation组件中
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_ClusteringBlocks.png)
 

RegulatoryPlanning_ClusteringPoints
- **目的**：
    - 基于层次聚类算法及各地块中心点之间的直线距离矩阵，对地块进行聚类
- **输入**：
    - 各地块的中心点
    - 各等级生活圈的服务半径
- **输出**：
    - 表达聚类组团之间层级关系的连线
    - 树形结构中各个地块的ID，用于表达所有聚类组团的层级
    - 包含所有聚类结果的对象，可用于RegulatoryPlanning_LanduseAllocation组件中
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/NA_ClusteringPoints.png)

RegulatoryPlanning_LanduseAllocation
- **目的**：
    - 自动给各个地块赋予用地性质属性
- **输入**：
    - 地块面
    - 各个地块不同计算半径下的可达性数值（推荐：3个分支）
    - 包含所有聚类结果的对象。该对象从RegulatoryPlanning_ClusteringBlocks组件中获取
    - 用地平衡表。其中，用地性质按照用户设定的优先级高到低的顺序进行排序；各类用地性质后紧跟的数值表示其对应的用地面积占总用地面积的百分比（格式：“R:0.2”，不含引号）
- **输出**：
    - 被分割后的地块面（为了尽可能地满足用地平衡表的要求，完成用地性质属性的分配后，其中部分地块会被分割）
    - 每个地块面被赋予的用地性质属性（与上述地块面的顺序保持一致）
    - 计算结果对应的用地平衡表
    - 包含用地性质分配所有计算结果的对象，该对象将用于RegulatoryPlanning_FarAllocation组件中
- **示例**：
 
  ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RP_LanduseAllocation.png)

RegulatoryPlanning_FarAllocation
- **目的**：
    - 自动给各个地块赋予容积率属性
- **输入**：
    - 包含用地性质分配所有计算结果的对象。该对象从RegulatoryPlanning_LanduseAllocation组件中获取
    - 整个城市设计方案的总建筑面积
    - 建筑面积结构，通过各用地性质对应的建筑面积所占总建筑面积百分比来表达
- **输出**：
    - 每个地块面被赋予的容积率属性
- **示例**：
 
  ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RP_FARAllocation.png)

3. 城市设计
UrbanDesign_SiteParameter
- **目的**：
    - 基于道路网、可达性数值、场地信息，自动生成地块参数
- **输入**：
    - 被清洗的道路中心线
    - 各道路中心线所对应的可达性数值
    - 地块边界曲线
- **输出**：
    - 各地块的参数
- **示例**：

 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/UD_SiteParameter.png)

UrbanDesign_SiteParameterExtra
- **目的**：
    - 设置和调整地块参数（容积率、建筑密度等）
- **输入**：
    - 各地块的基础参数，从UrbanDesign_SiteParameter组件中获取
    - 用地性质（R:0, C:1, GIC:2, M:3, W:4）
    - 容积率
    - 建筑密度
    - 混合度
    - 建筑组合形式
        - 居住建筑：0-行列式，1-点式
        - 非居住建筑：0-点式；1-围合式；2-混合式
    - 建筑朝向（单位：弧度）
- **输出**：
    - 各地块设置后的参数
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/UD_SiteParameterExtra.png)

UrbanDesign_SiteGeneratePlans
- **目的**：
    - 基于输入参数自动生成建筑体块方案
- **输入**：
    - 各地块设置后的参数，从UrbanDesign_SiteParameterExtra组件中获取
    - 方案所在城市对应的ID
- **输出**：
    - 包含设计方案所有信息的对象。该对象将用于“多维评估”模块
    - 各地块的原始边界曲线（未分割）
    - 各地块的容积率
    - 各地块的建筑密度
    - 地块分割得到的子地块的曲线
    - 地块分割得到的子地块的场地退线
    - 各建筑的基底轮廓的曲线
    - 各建筑的屋顶轮廓的曲线
    - 各建筑的层数
    - 各建筑的所有体块（brep）
    - 各建筑的各体块的建筑功能，与上述的“各建筑的所有体块”的顺序一一对应
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/UD_SiteGeneratePlans.png)
 

4. 公服覆盖
FacilityAnalysis_ConnectToNetwork
- **目的**：
    - 把各地块与其邻近的道路中心线相连，以使各地块融入到道路网中，方便后续的网络计算
- **输入**：
    - 清洗后的道路网
    - 地块面
- **输出**：
    - 路网模型，将用于FacilityAnalysis_CoverageArea组件中
    - 各地块与邻近道路的连线
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/FL_ConnectToNetwork.png)
 

FacilityAnalysis_CoverageArea
- **目的**：
    - 基于给定的计算半径，道路网中的最短路径距离，计算同一类所有设施的覆盖面积
- **输入**：
    - 路网模型，从FacilityAnalysis_ConnectToNetwork组件中获取
    - 公服设施所处的地块面
    - 公服设施的服务半径。该半径基于道路网最短路径进行定义
- **输出**：
    - 位于设施覆盖范围内的地块
    - 被设施覆盖的地块的中心点
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/FL_CoverageArea.png)
 

5. 多维评估
SustainabilityAnalysis_Energy
- **目的**：
    - 计算自生成设计方案中各个建筑的能源消耗量
- **输入**：
    - 包含设计方案所有信息的参数，从UrbanDesign_SiteGeneratePlans组件中获取
- **输出**：
    - 各建筑的能源消耗量
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_Energy.png)
 

SustainabilityAnalysis_EnergyCarbonEmissions
- **目的**：
    - 计算生产给定的能源消耗量所产生的碳排放
- **输入**：
    - 能源消耗量（单位：千瓦时/年）
- **输出**：
    - 生产给定的能源消耗量所产生的碳排放（单位：吨二氧化碳/年）
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_E_CarbonEmissions.png)
 

SustainabilityAnalysis_Water
- **目的**：
    - 计算自生成设计方案中各个建筑的水资源消耗量
- **输入**：
    - 包含设计方案所有信息的参数，从UrbanDesign_SiteGeneratePlans组件中获取
- **输出**：
    - 各建筑的水资源消耗量
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_Water.png)
 

SustainabilityAnalysis_Waste
- **目的**：
    - 计算自生成设计方案中各个建筑的垃圾产生量
- **输入**：
    - 包含设计方案所有信息的参数，从UrbanDesign_SiteGeneratePlans组件中获取
- **输出**：
    - 各建筑的垃圾产生量
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_Garbage.png)
 

SustainabilityAnalysis_WasteCarbonEmissions
- **目的**：
    - 计算给定的生活垃圾产生量和垃圾处理方式所产生的碳排放
- **输入**：
    - 需要进行垃圾处理的生活垃圾产生量（单位：吨/年）
    - 垃圾处理方式（0-垃圾填埋，1-垃圾焚烧，2-垃圾堆肥）
- **输出**：
    - 处理给定的生活垃圾产生量所产生的碳排放（单位：吨二氧化碳/年）
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_G_CarbonEmissions.png)
 

SustainabilityAnalysis_EnergyCustom
- **目的**：
    - 根据用户输入的建筑体块及其功能，计算各建筑的能源消耗量
- **输入**：
    - 建筑体块（brep）
    - 各建筑体块的功能
- **输出**：
    - 各建筑体块的能源消耗量
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_EnergyCustom.png)
 

SustainabilityAnalysis_WaterCustom
- **目的**：
    - 根据用户输入的建筑体块及其功能，计算各建筑的水资源消耗量
- **输入**：
    - 建筑体块（brep）
    - 各建筑体块的功能
- **输出**：
    - 各建筑体块的水资源消耗量
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_WaterCustom.png)
 

SustainabilityAnalysis_WasteCustom
- **目的**：
    - 根据用户输入的建筑体块及其功能，计算各建筑的垃圾产生量
- **输入**：
    - 建筑体块（brep）
    - 各建筑体块的功能
- **输出**：
    - 各建筑体块的垃圾产生量
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_GarbageCustom.png)
 

SustainabilityAnalysis_Population
- **目的**：
    - 估算各居住建筑的居住人口
- **输入**：
    - 建筑体块（brep）
- **输出**：
    - 各建筑体块的估算居住人口
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/RD_Population.png)

6. 视线分析
VisibilityAnalysis_ExposureRate2D
- **目的**：
    - 通过分析道路节点与底层商业的关系，计算底层商业在二维层面上的曝光率。计算结果可为商业选址提供空间数据支持
- **输入**：
    - 建筑体块（brep）
    - 预设视点
    - 是否标准化
    - 视域半径
    - 细分程度（数值越高，计算结果越准确，但计算时间越长）
- **输出**：
    - 建筑体块基底轮廓线
    - 基底轮廓线对应的曝光率
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_ExposureRate2D.png)
 

VisibilityAnalysis_GenerateMeshBuilding
- **目的**：
    - 根据细分程度，把建筑的Rhino Brep面转换成DMesh面，以提高计算效率
- **输入**：
    - 建筑的Rhino Brep面
    - 细分程度（默认值：-1；该数值越高，计算结果越准确，但计算时间越长）
- **输出**：
    - GenerateMesh类对象
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_GenerateMesh.png)
 

VisibilityAnalysis_GenerateMesh
- **目的**：
    - 根据细分程度，把建筑的Rhino Mesh面转换成DMesh面，以提高计算效率
- **输入**：
    - 建筑的Rhino Mesh面
- **输出**：
    - GenerateMesh类对象
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_GenerateMesh_Mesh.png)

VisibilityAnalysis_ExposureRate3DBuildings
- **目的**：
    - 通过分析视点与建筑的关系，计算建筑在三维层面上的曝光率。计算结果可为商业选址提供空间数据支持
- **输入**：
    - 预设视点
    - GenerateMesh类对象
    - 各点的视域半径（默认值：300）
- **输出**：
    - 各建筑被染色的侧边Mesh面
    - 各建筑无染色的顶部和底部Mesh面
    - 各Mesh面的被观测次数
    - 各视点的曝光率
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_ExposureRate3D.png)

VisibilityAnalysis_ExposureRate3DMesh
- **目的**：
    - 通过分析视点与Mesh面的关系，计算各Mesh面在三维层面上的曝光率。计算结果可为商业选址提供空间数据支持
- **输入**：
    - 预设视点
    - GenerateMesh类对象
    - 各点的视域半径（默认值：300）
- **输出**：
    - 染色的Mesh面
    - 各Mesh面的被观测次数
    - 各视点的曝光率
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_ExposureRate3D_Mesh.png)

VisibilityAnalysis_VisualCalc
- **目的**：
    - 在三维层面上，通过对道路网进行插点，计算路网的可视性
- **输入**：
    - 预设路网
    - GenerateMesh类对象
    - 路网细分程度（单位：米，默认值：500）
    - 各点的视域半径（默认值：300）
    - 是否输出Mesh面
- **输出**：
    - 清洗后的道路网，将用于VisibilityAnalysis_VisualSyntaxComputing组件中
    - 道路上的视点
    - 各道路的可视性属性
    - 染色的Mesh面（取决于是否选择输出Mesh面）
- **示例**：
 
 ![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_VisualCalc.png)

VisibilityAnalysis_VisualSyntaxComputing
- **目的**：
    - 基于输入的道路网和三维层面上其对应的可视性属性进行可视网络分析
- **输入**：
    - 清洗后的道路网，从VisibilityAnalysis_VisualCalc组件中获取
    - 各道路对应的可视性属性
    - 计算半径（默认值：-1，即计算全局路网）
- **输出**：
    - Visual total depth
    - Visual mean depth
    - Visual integration
    - Visual choice
    - Normalized visual integration
    - Normalized visual choice
- **示例**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/SA_VisualSyntaxCompute.png)

### 6. 水管网计算（Coming Soon）
<details>
<summary>水管网计算具体参数</summary>

> Water_InpFileToGeometry
- **目的**：
- **输入**：
- **输出**：
- **样例展示**：

> Water_CalculateSiteDemand
- **目的**：
- **输入**：
- **输出**：
- **样例展示**：

> Water_NetworkOptimization
- **目的**：
- **输入**：
- **输出**：
- **样例展示**：

</details>


## **许可证**
### ***GNU General Public License v.3***
*Copyright (C) 2020  Tao Yang, Weizhen Luo, Xuhui Lin, Chengru Deng*

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
