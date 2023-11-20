<div style="text-align: center; line-height: 0; padding-top: 9px;">
  <img src="https://www.csd.auth.gr/wp-content/themes/csd/images/logo.png" alt="Auth Informatics Logo" style="width: 700px">
</div>

## The present repository contains two notebooks created during the implementation of my university thesis: "Development of a Residential Clustering System based on their Electricity Consumption Footprint."<br> Additionally, it includes one .csv file with the data used in the notebooks and one .pdf file that explains all the data attributes.

---

### <u>**Energy_data_Wrangling.ipynb**</u>

The purpose of this notebook is to transform the raw dataset 'Electric Energy Data.csv' into a clean and usable form by applying a series of steps, including:

1. **Load the data into a Pandas DataFrame and restructure it.**
2. **Remove unnecessary columns.**
3. **Handle missing values and eliminate duplicate rows.**
4. **Conduct an outlier analysis and address any erroneous records.**
5. **Split the dataset based on the 'Heating Source' attribute and apply techniques such as 'One-Hot Encoding,' 'Ordinal Encoding,' and 'MinMax Scaling' to both categorical and numerical attributes.**
6. **Visualize the data and store it in a MongoDB database.**

These transformations will enable us to later train various clustering algorithms for analysis.

---

### <u>**Cluster-analysis.ipynb**</u>

The aim of this notebook is to evaluate the accuracy and performance of three different clustering categories on the transformed dataset produced by the previous notebook. The main goals are to determine which algorithm exhibits the best performance.

#### Partition-Based Algorithms
- K-Means
- PAM/K-Medoids

#### Hierarchical Algorithms
- Single Linkage
- Complete Linkage
- Average Linkage
- Ward Linkage

#### Density-Based Algorithms
- DB-Scan
- OPTICS
