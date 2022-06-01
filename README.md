# AutoIFS
**Automated Important Features Selection for Machine Learning Models**

The model releases the following material after implementation:

1. EncodedData.csv
2. FeaturesData.csv
3. TargetData.csv
4. MainDataFrame.csv
5. AutoDP_DataDistribution.png
6. AutoDP_DataDistribution.tif
7. ImportantFeatures.csv
8. AutoIFS.png
9. AutoIFS.tif

**Note:** If you have a **Big Data**, you can use the following code in the **"Data Ingestion"** section after loading data.

<!-- Data Size Reduction If it needs -->
print("The Data Former Size:", df.size)
print("")

N = 3000

if df.size <= N:
    df = df.iloc[:, :]
else:
    df = df.iloc[0: N, :] 
    
print("The Data After Size:", df.size)
print("")
