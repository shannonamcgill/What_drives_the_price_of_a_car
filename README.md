# Business Understanding
The business objectives for this project are to mine the used car dataset and determine the features that have the highest correlation in purchasing a car. 

# Data Understanding
There are 4 major steps engineers and scientist should complete during the data understanding phase. 
   <ol>
    <li>Collect Initial Data and creating an Initial Data Collection Report</li>
    <li>Describe Data and creating a Data Description Report</li>
    <li>Explore Data and creating a Data Exploration Report</li>
    <li>Verify Data Quality and creating a Data Quality Report</li>
    <ol>

##Initial Data Collection Report

   For this project we will be looking at a used car dataset found in the on the Kagal website. 
   
   ##Data Description Description Report
   This dataset contains 18 columns and has 426,880 rows of data with 32,895 of these rows missing their price. 
   id, region, price, year, manufacturer, model, condition, cylinders, fuel, odometer, title_status, transmission, VIN, drive, size, type, paint_color and, state.
   
   The following shows a list of each of the columns and the number of missing values for each of them. 
   
   id                   0
   region               0
   price                0
   year              1205
   manufacturer     17646
   model             5277
   condition       174104
   cylinders       177678
   fuel              3013
   odometer          4400
   title_status      8242
   transmission      2556
   VIN             161042
   drive           130567
   size            306361
   type             92858
   paint_color     130203
   state                0

##Data Quality Report

<p>
    Exploring the data there are several key takeaways. 
    <ol> 
        <li> There are a total of 426K rows in this dataset </li>
        <li> The size feature only contains 120519 populated values. This might make the feature more noisy than              valuable.</li>
        <li> The ID and VIN columns are unique identifiers and not something that would correlate with the price of              the vehicle. Unless used as the dataset's index, these should be removed from our data. </li>
        <li>Most of our features are text values and must be transformed into numerical representations to 
            determine their correlation to the vehicle’s price.</li>
        <li>There were 32895 records with a price tag of 0.00 This should be dropped from our dataset. I also 
            decided to reduce the dataset down sales prices below 60K </li>
        <li>The cylinders feature is a numerical category and should be cleaned up to remove the text values of    
             cylinders and replace the other value with and empty value. </li>
        <li> The condition column can be updated with numberical representations using Ordinal Encoder.</li>
        <li> The model column will be dropped because it contains 28265 different values </li>
     </ol>
</p>    



