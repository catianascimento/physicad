# Dengue and Mobility Data Analysis Project

We provide dengue case data aggregated both temporally (weekly) and spatially (by traffic zones).

This project uses Python notebooks to process dengue and mobility data, generate networks, and make comparisons between the networks based on different metrics. Below is a description of each notebook in the project:

> 📁 **Notebooks are organized in two folders located at the root of the repository**:
> - `github_physicad_20142024`: contains the notebooks used to compute results for all years cited in the paper.
> - `github_physicad_2015`: contains the notebooks focused specifically on data from the year 2015.

## 01-denguedataprocessing.ipynb  
This notebook aims to process daily dengue case data and generate weekly data. It also generates histograms for both daily and weekly data and performs some exploratory analyses. Additionally, the **mutual information** between the time series of dengue cases is calculated, and a similarity matrix based on this metric is generated and saved to a file.

### Features:
- Generate weekly data from daily data.
- Create daily and weekly histograms.
- Calculate mutual information between time series of dengue cases.
- Generate a similarity matrix based on mutual information.

## 02-firstcomparisons.ipynb  
This notebook performs some comparative analyses between **mobility x distance** and **mutual information x distance**. Statistical analyses are conducted, including the calculation of a **linear regression**, to explore the relationships between these variables.

### Features:
- Analysis between mobility and distance.
- Analysis between mutual information and distance.
- Linear regression calculation and interpretation.

## 03-denguenetworks.ipynb  
In this notebook, dengue networks are generated using thresholds applied to the similarity matrices obtained from the **mutual information** calculated between the weekly dengue case time series in each traffic zone.

### Features:
- Generate networks based on thresholds applied to similarity matrices.
- Construct dengue networks using mutual information.

## 04-mobnetworks.ipynb  
This notebook contains the necessary code to generate mobility networks. The networks are constructed by applying thresholds to the flow matrix between the traffic zones.

### Features:
- Generate mobility networks based on flow matrices.
- Construct mobility networks using thresholds applied to the matrices.

## 05-comparingnetworks.ipynb  
In the final notebook, we compare dengue networks with mobility networks. Different comparison metrics, such as the **Frobenius norm**, are used to assess the differences and similarities between the networks generated in the previous notebooks.

### Features:
- Compare dengue networks with mobility networks.
- Calculate comparison metrics like the **Frobenius norm**.

---

This project provides a comprehensive analysis of dengue and mobility networks, using mutual information metrics and other statistical techniques to explore the relationships between these variables in traffic zones. All notebooks are executable in Python with the appropriate libraries installed.
