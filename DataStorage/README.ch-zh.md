[English](./README.md) | [简体中文](./README-ch.zh.md)

# **模拟数据湖**

本部分为模拟的本地数据湖存储空间，由于代码仓库文件大小的限制，我们仅提供了所有静态数据文件与模拟流式数据的源文件各 50 条，具体对应关系如下：

| 数据名称  | 静态数据                                                                                                                                                                     | 流数据源文件                                                         |
|-------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|
| 气象数据  | [weather](Weather/Static/weather.csv)                                                                                                                                    | [weather_stream](Weather/Streaming/weather_stream.csv)         |
| 建筑能耗  | [meters](EnergyConsumption/Static/meters.csv)                                                                                                                            | [meters_stream](EnergyConsumption/Streaming/meters_stream.csv) |
| 建筑元数据 | [building_information](BuildingMetadata/Static/building_information.csv)/ [new_building_information_modify](BuildingMetadata/Static/new_building_information_modify.csv) | -                                                              |
