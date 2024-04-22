# Business Understanding
The business objectives for this project are to mine the used car dataset and determine the features that have the highest correlation in purchasing a car. 

# Data Understanding
There are 4 major steps engineers and scientist should complete during the data understanding phase. 
   <ol>
    <li>Collect Initial Data and creating an Initial Data Collection Report</li>
    <li>Describe Data and creating a Data Description Report</li>
    <li>Explore Data and creating a Data Exploration Report</li>
    <li>Verify Data Quality and creating a Data Quality Report</li>
   </ol>
   

## Initial Data Collection Report

   For this project we will be looking at a used car dataset found in the on the Kagal website. 
   
## Data Description Report
   <p>This dataset contains 18 columns and has 426,880 rows of data with 32,895 of these rows missing their price. 
   id, region, price, year, manufacturer, model, condition, cylinders, fuel, odometer, title_status, transmission, VIN, drive, size, type, paint_color and, state.</p>
   
   <p>The following shows a list of each of the columns and the number of missing values for each of them. </p>
   <p>
   <ul>
      <li>id:0</li>
      <li>price:0</li>
      <li>year:1205</li>
      <li>manufacturer:17646</li>
      <li>model:5277</li>
      <li>condition:174104</li>
      <li>cylinders:177678</li>
      <li>fuel:3013</li>
      <li>odometer:4400</li>
      <li>odometer:4400</li>
      <li>transmission:2556</li>
      <li>VIN:161042</li>
      <li>drive:130567</li>
      <li>size:306361</li>
      <li>type:92858</li>
      <li>paint_color:130203</li>
      <li>state:0</li>
   </ul>
   </p>
## Data Quality Report

<p>Exploring the data there are several key takeaways. 
<ol> 
        <li> There are a total of 426K rows in this dataset </li>
        <li> The size feature only contains 120519 populated values. This might make the feature more noisy than valuable.</li>
        <li> The ID and VIN columns are unique identifiers and not something that would correlate with the price of the vehicle. 
           Unless used as the dataset's index, these should be removed from our data. </li>
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

# Exploratory Data Analysis

![alt text](https://github.com/shannonamcgill/What_drives_the_price_of_a_car/blob/main/images/Salesmanufacturer.png)?raw=true)


# Model and Findings

<p>After having completed our analysis of historical car sales, our machine-learning models have predicted that the price of a vehicle can be determined with 75% accuracy when focusing on the odometer, color, model, status of the title, and overall vehicle condition. 
</p>

<p>
We believe we can fine-tune our algorithm to increase its accuracy, but we will need a few more weeks to conduct our development.</p>

<p> Our next steps will be to increase our model’s accuracy and identify the specific values within each category that drive up a vehicle’s price. 
</p>




