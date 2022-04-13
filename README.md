# comp5349-assignment1
## How to run the code
This assignment was written and run on colab.

For data import, I use colab to load google drive and read the dataset (.csv file) which is needed for this assignment from google drive.For each person the location where the dataset is stored in google drive is different. The code I use is as follows.

```
   input_path = 'file:///content/drive/MyDrive/comp5349/' #Location of .csv in google drive
   Anti_assignment_CIC_g3_rdd = spark.read.csv(input_path+"Anti_assignment_CIC_g3_utf8.csv",header=True).rdd
   Governing_Law_rdd = spark.read.csv(input_path+"Governing_Law.csv",header=True).rdd
```      

The input_path here is the path of the dataset (.csv) in google drive. In order to read the dataset successfully with this code, **please modify the input_path and replace it with the path where the dataset is located in your own google drive or put the dataset (.csv) into the path shown in input_path.**
Once the dataset has been successfully read, run the code for Method 1 in order, then the code for Method 2 in order. Because method 2 will use the functions written in method 1
