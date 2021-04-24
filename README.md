# UrbanXTools


##  **目录**
  * [**更新**](#更新)
  * [**介绍**](#介绍)
  * [**安装步骤**](#安装步骤)
  * [**演示**](#演示)
  * [**工具内容**](#工具内容)
  * [**许可证**](#许可证)

## **更新**
### [UrbanXTools_v2.0.0](https://github.com/CAUPDxUrbanXLab/UrbanXTools/releases/tag/v2.0.0_V6.14)
#### **1. NA_Computing**
 - **优化底层算法**
 - **新增计算指标**
 - **将路网清洗（合并、去重、打断等）流程内置。**
   
   **现有如下计算指标：**
 - *Metric choice*
 - *Metric integration*
 - *Metric mean depth*
 - *Metric total depth*
 
 - *Angular choice*
 - *Angular integration*
 - *Angular mean depth*
 - *Angular total depth*
 
 - *Normalized angular choice(NACH)*
 - *Normalized angular integration(NAIN)*
#### **2. NA_GeneratingSites**
 - **新增根据不同等级路网生成地块的工具。**
#### **3. NA_ClearRoadsData**
 - **更名为NA_RoadsSplitter**
 - **且使用NA_Computing前不再强制需要使用此工具。**
 - **此工具在寻找曲线交点时，使用IntervalTree的数据结构和相应算法，替代暴力算法，加快速度。** 
#### **4. SA_GenerateMesh**
 - **几何数据转换**
#### **5. SA_Exposure3D**
 - **三维视线分析**

## **介绍**
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/intro.png)
### 1. 主要功能
- 基于城市规划设计逻辑和计算机算法，快速生成符合上位规划管控指标的城市设计方案草模；
- 基于多专业协同理念和可持续发展目标，即时对城市设计方案进行评估；
- 依托参数化设计方法，建立控规详规与城市设计方案快速评估、反馈、修改的机制，提高设计效率与方案质量。
### 2. 目标
- 高质量
- 可持续城市发展
### 3. 研发人员
- 杨滔、罗维祯、林旭辉、邓成汝、董雨菲
### 4. 合作单位
- 中国城市规划设计研究院——城市设计分院
### 5. 注意事项
- 推荐使用Rhino version 6.30 ， 如使用Rhino版本低于6.30， 请于release下载v6.12插件；
- 模型单位必须使用米（model unit: meter），如使用毫米则无法进行方案自动生成；
- 如方案距离工作视图原点较远时，由于Rhinocommon几何运算精度限制，几何布尔运算有一定概率出现问题，因此请将路网地块等几何数据移动至原点（0，0，0）附近；
- 如有运行问题或功能需求，可在github issue里提出，开发者会尽力解决。

## **安装步骤**
- 下载链接：
	- 蓝奏云盘
		- 链接：https://wwe.lanzous.com/b01tqy68f
		- 密码:h5d8
	- 百度网盘
		- 链接：https://pan.baidu.com/s/1Bkl0HBBNNevcUSm3aFa4nA 
		- 密码：koff
	- Github下载
		- 链接：https://github.com/CAUPDxUrbanXLab/UrbanXTools/releases
### 1. 进入Release界面，选择合适版本，下载zip文件，解压并取出

- 点击进入Release界面

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_000.png)

- 进入Release界面
	- 完全版：推荐选择 UrbanXTools_v2.0.0（已经包含以下多种版本）
	
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/releaseVersion.png)

- 取出文件夹：UrbanXTools_v.2.0.0

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_002.png)

### 2. 打开Rhino，打开Grasshopper，进入Component File

- 打开Rhino，打开Grasshopper，点击 File --> Special Folders --> Components Folder 

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_003.png)

- 将文件夹：UrbanXTools_v.2.0.0 置入
- 如果文件夹中存在 UrbanXTools_v.1.0.0，请将该文件夹全部删除，置入UrbanXTools_v.2.0.0

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_003_1.png)

### 3. 检查文件夹内容完整性，重启Rhino

- 确保文件夹里，有如下文件

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_004.png)

### 4. 顺利置入

- 如顺利置入，界面如下

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%AE%89%E8%A3%85%E6%B5%81%E7%A8%8B_005.png)




## **演示**
### 1. 空间结构交互性评估
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E7%A9%BA%E9%97%B4%E7%BB%93%E6%9E%84%E8%AE%A1%E7%AE%97%E6%BC%94%E7%A4%BA.gif)

[案例: NetworkAnalysis](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/1_NetworkAnalysis)

### 2. 公共服务设施覆盖分析
![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E5%85%AC%E6%9C%8D%E8%A6%86%E7%9B%96%E6%BC%94%E7%A4%BA.gif)

[案例: FacilityLocation](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/2_FacilityLocation)

### 3. 城市设计方案自动生成
- 住宅行列式+点式

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90%E6%BC%94%E7%A4%BA_%E4%BD%8F%E5%AE%85%E8%A1%8C%E5%88%97%E5%BC%8F%2B%E7%82%B9%E5%BC%8F.gif)

- 商业+仓储+工厂

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90%E6%BC%94%E7%A4%BA_%E5%95%86%E4%B8%9A%2B%E4%BB%93%E5%82%A8%2B%E5%B7%A5%E5%8E%82.gif)

[案例: UrbanDesign SingleSite](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/3_UrbanDesign)

[案例: UrbanDesign_MultiSitesSites](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/3_UrbanDesign)

### 4. 城市设计方案资源荷载计算

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E8%B5%84%E6%BA%90%E8%8D%B7%E8%BD%BD.gif)

[案例: Resources Demand](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/4_ResourcesDemand)

### 5. 城市设计方案曝光度分析2D

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%87.png)

[案例: ExposureRates2D](https://github.com/CAUPDxUrbanXLab/UrbanXTools/tree/main/Samples/5_SpatialAnalysis)

### 6. 城市设计方案曝光度分析3D

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/%E6%9B%9D%E5%85%89%E7%8E%873D.png)

[案例: ExposureRates3D](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/Samples/5_SpatialAnalysis)


## **工具内容**

### 1. 空间结构分析

> Network_ClearRoadsData

- **目的**：
    - 清洗和分割所有道路曲线，处理情况包括：重叠、形状相同和无效曲线。
- **输入**：
    - 待清洗、分割的道路曲线
- **输出**：
    - 清洗并分割完成的道路曲线
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Network_ClearRoadsData.png)

> Network_ClearSitesData

- **目的**：
    - 清洗所有地块曲线，处理情况包括：重叠、形状相同、非平面、非闭合地块曲线。
- **输入**：
    - 待清洗的地块曲线
- **输出**：
    - 清洗完成的道路曲线
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Network_ClearSitesData.png)

> Network_Computing

- **目的**：
    - 计算道路网络性质，包括按米制、按角度制的空间句法，可选择不同半径进行计算
    - 介数中心性(betweenness): 在一定范围内，找出网络中任意两点的最短经，并计算每段道路被经过的次数
    - 紧密中心性(closeness): 在一定范围内，从该点到沿最短路径的指定目标点所需的平均距离
- **输入**：
    - 需要计算的路网曲线
    - 计算半径
    - 是否需要标准化
- **输出**：
    - 米制 介数中心性
    - 米制 紧密中心性
    - 角度制 介数中心性
    - 角度制 紧密中心性
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Network_Computing.png)

> Network_SiteAccessibility

- **目的**：
    - 计算地块可达性
- **输入**：
    - 地块周边路网曲线
    - 周边路网曲线对应数值
    - 需要计算的地块曲线
- **输出**：
    - 由地块曲线围合而成的地块平面
    - 地块可达性得分
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Network_SiteAccessibility.png)

> Network_RoadDensity

- **目的**：
    - 基于特定边界，计算路网密度
- **输入**：
    - 输入需要计算的路网曲线
    - 输入对应路网的边界线
- **输出**：
    - 输出道路网密度（数据）
    - 输出道路网密度（单位：km/km²）
    - 输出边界内容道路曲线
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Network_RoadDensity.png)

### 2. 设施计算

> Facility_ToNetwork

- **目的**：
    - 计算地块几何中心，连接到周边最近路段，并将新路段添加到已有道路网络
- **输入**：
	- 清洗处理后的路网
	- 全部需计算地块
- **输出**：
  - 新建路网图结构数据，用于路网密度计算
  - 新建路网线段几何数据
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Facility_ToNetwork.png)

> Facility_CoverageArea

- **目的**：
    - 按照路网距离计算设施覆盖范围
- **输入**：
  - 路网图结构数据，连接Facility_ToNetwork的RoadsNetwork输出端
  - 公服设施地块，覆盖范围计算起点
  - 公服设施覆盖半径，按照真实路网距离进行计算
- **输出**：
  - 覆盖范围内的地块
  - 覆盖范围内地块的几何中点
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Facility_CoverageArea.png)

### 3. 自动生成

> Urban_DesignCalculator
- **目的**：
    - 计算在特定场地内，可容纳的建筑数量和楼层，以实现给定 FAR 和密度的目标
- **输入**：
    - 输入场地曲线
    - 输入建筑原型的平面线稿
    - 输入每一种建筑类型的层数范围
    - 输入目标容积率FAR
    - 输入目标建筑密度
- **输出**：
    - 可容纳的建筑数量
    - 可容纳的建筑楼层数
    - 现有地块FAR容积率
    - 现有地块建筑密度
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Urban_DesignCalculator.png)


> Urban_DynamicSplit
- **目的**：
    - 使用Binary Partition Tree算法，基于容积率，对地块进行精确划分。
- **输入**：
    - 输入准备切分的场地曲线
    - 输入场地对应的目标面积或比例
    - 输入场地对应的优先等级
    - 输入场地边界框的可达性得分
    - 输入场地边界框的角度
    - 在动态切分时，是否改变角度
- **输出**：
    - 输出子地块边线
    - 输出子地块边界框
    - 输出子地块边界性得分
    - 输出子地块角度
    - 输出子地块ID
    - 输出Binary Partition Tree的可视化结果
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Urban_DynamicSplit.png)


> Urban_ResidentialLimitation
- **目的**：
    - 输入场地、及所在城市，计算该场地可达到的最大容积率及建筑密度
- **输入**：
    - 输入准备进行计算的场地曲线
    - 输入城市序号，获得气象信息
    - 输入该场地能容纳的最大限高
    - 输入住宅层数高度，默认为3米
    - 输入住宅朝向角度，默认为0度
    - 输入住宅深度，默认为26米
- **输出**：
    - 输出场地可容纳的最大容积率
    - 输出场地可容纳的最大建筑密度
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Urban_ResidentialLimitations.png)


> Urban_SiteParameter
- **目的**：
    - 基于道路、道路可达性得分及场地数据，形成自生成参数
- **输入**：
    - 输入道路曲线
    - 输入道路可达性得分
    - 输入场地曲线
- **输出**：
    - 输出 Urban_SiteParameter 类
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Urban_SiteParameter.png)


> Urban_SiteParameterExtra
- **目的**：
    - 调整地块参数（容积率、建筑密度等），设计参数调整功能
- **输入**：
    - 输入 Urban_SiteParameter 类
    - 输入场地对应的用地属性（R:0, C:1, GIC:2, M:3, W:4）
    - 输入场地对应的容积率FAR
    - 输入场地对应的建筑密度
    - 输入场地对应的混合度
    - 输入场地对应的建筑风格（住宅：风格0_行列式，风格1_点式|| 非住宅：风格0_点式，风格1_围合式，风格2_混合式 ）
    - 输入场地对应的朝向角度
- **输出**：
    - 输出 Urban_SiteParameter 类
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Urban_SiteParameterEtra.png)


> Urban_SiteGeneratePlans
- **目的**：
    - 基于输入参数，建筑体块方案自动生成，得到生成结果
- **输入**：
    - 输入 Urban_SiteParameter 类
    - 输入所在城市序号
- **输出**：
    - 输出 Urban_SiteResult 类
    - 输出原始场地曲线（尚未切分）
    - 输出场地对应的容积率FAR
    - 输出场地对应的建筑密度
    - 输出场地对应的子地块曲线
    - 输出子地块的场地退线
    - 输出每个建筑对应的层数（curve）
    - 输出每个建筑对应的屋顶线 (curve)
    - 输出每个建筑对应的层数（int）
    - 输出每个建筑对应的体块 (brep)
    - 输出每个建筑对应的功能 (string)
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Urban_SiteGeneratePlan.png)


### 4. 资源指标计算
> Resources_Energy

- **目的**：
    - 计算自生成设计方案里，每个建筑的能源消耗量
- **输入**：
    - 输入Urban_SiteGeneratePlans 类
- **输出**：
    - 输出对应楼块的能源消耗量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Resources_Energy.png)


> Resources_Water
- **目的**：
    - 计算自生成设计方案里，每个建筑的水资源消耗量
- **输入**：
    - 输入Urban_SiteGeneratePlans 类
- **输出**：
    - 输出对应楼块的水资源消耗量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Resources_Water.png)


> Resources_Garbage
- **目的**：
    - 计算自生成设计方案里，每个建筑的固废产生量
- **输入**：
    - 输入Urban_SiteGeneratePlans 类
- **输出**：
    - 输出对应楼块的固废产生量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Resources_Garbage.png)


> Resources_EnergyCustom
- **目的**：
    - 根据建筑体块及功能，计算每个建筑的能源消耗量
- **输入**：
    - 输入建筑体块、及其对应的建筑功能
- **输出**：
    - 输出对应体块的能源消耗量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Resources_EnergyCustom.png)


> Resources_WaterCustom
- **目的**：
    - 根据建筑体块及功能，计算每个建筑的水资源消耗量
- **输入**：
    - 输入建筑体块、及其对应的建筑功能
- **输出**：
    - 输出对应体块的水资源消耗量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Resources_WaterCustom.png)

> Resources_GarbageCustom
- **目的**：
    - 根据建筑体块及功能，计算每个建筑的固废产生量
- **输入**：
    - 输入建筑体块、及其对应的建筑功能
- **输出**：
    - 输出对应体块的固废产生量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Resources_GarbageCustom.png)

> Resources_Population
- **目的**：
    - 根据建筑体块，计算每个建筑的可容纳人口量
- **输入**：
    - 输入建筑体块
- **输出**：
    - 输出对应体块的容纳人口量
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Spatial_Population.png)

### 5. 空间指标计算
> Spatial_Analysis_Exposure2D
- **目的**：
    - 根据道路节点，计算建筑底商的空间曝光率，为商业选址提供空间数据支持
- **输入**：
    - 输入建筑体块、预设置的可视节点、是否标准化、可视半径、细分程度（该数值越高，结果越准确，计算速度越慢）
- **输出**：
    - 输出建筑基底轮廓线、轮廓线对应曝光率
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Spatial_Analysis_ExposureRate2D.png)

> Spatial_Analysis_GenerateMesh
- **目的**：
    - 根据细分程度，将建筑Brep面转化为Mesh面，提高计算效率。
- **输入**：
    - 输入建筑体块、细分程度（默认值为-1）（该数值越高，结果越准确，计算速度越慢）
- **输出**：
    - 输出GenerateMesh Class（包含建筑Mesh面，建筑立面面积，建筑中心点）
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Spatial_Analysis_GenerateMesh.png)

> Spatial_Analysis_Exposure3D
- **目的**：
    - 根据可视点选择，计算建筑三维体块的空间曝光率，为商业选址提供空间数据支持
- **输入**：
    - 输入预设置的可视节点、GenerateMesh Class、横轴细分程度（默认为10）、纵轴细分程度（默认为40）、视角范围（默认为200）、视角高度（默认为45）（该数值越高，结果越准确，计算速度越慢）
- **输出**：
    - 输出建筑Mesh面（已染色），可视点对应的可视率
- **样例展示**：

![image](https://github.com/CAUPDxUrbanXLab/UrbanXTools/blob/main/images/logo_24px/Spatial_Analysis_ExposureRate3D.png)


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
