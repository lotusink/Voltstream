[English](./README.md) | [简体中文](./README.ch-zh.md)

# **Simulated Data Lake**

This section represents the simulated local data lake storage space. Due to the repository file size limitations, only 50 records are provided for both the static data files and the simulated streaming source files, along with the baseline model placeholder file and the optimal model parameter configuration.

The structured data includes:

| Data Name | Static Data                                                                                                                                                               | Streaming Source File                                          |
|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|
| Meteorological Data | [weather](Weather/Static/weather.csv)                                                                                                                                     | [weather_stream](Weather/Streaming/weather_stream.csv)         |
| Building Energy Consumption | [meters](EnergyConsumption/Static/meters.csv)                                                                                                                             | [meters_stream](EnergyConsumption/Streaming/MeterRead/meters_stream.csv) |
| Building Metadata | [building_information](BuildingMetadata/Static/building_information.csv) / [new_building_information_modify](BuildingMetadata/Static/new_building_information.csv) | -                                                              |

The model data includes:

| Baseline Model | Optimal Model |
|----------------|----------------|
| [placeholder](Model/Baseline/placeholder.txt) | [parameter](Model/Finetune/parameter.txt) |

---

**Structure Index:** [Introduction Page](../README.md) | [Simulated Data Lake](../SimulatedDataLake/README.md) | [Project Code](../Scripts/README.md)
