# PATIENT_HEALTH_ANALYSIS
<p>In this dashboard, we analyse the historical monthly trend of waiting lists in inpatient or outpatient categories, where Inpatient means a patient who stays in a hospital while under treatment and Outpatient means a patient who receives medical treatment without being admitted to a hospital. A comprehensive overview of the patient's medical history, including past illnesses, surgeries, allergies, chronic conditions, etc., is presented on the dashboard. Detailed specialty level and age profile analysis. Use the folder connector and use multiple Excel files to collate them together and then import them.

  Combine both inpatient and outpatient data sets together to get a single set of data that will be used for visualisation purposes. Append tables, append both sets of data together, and rename it ALL DATA.

  <p><h3>DATA MODEL</h3></p>
<img src=https://github.com/AloraKesharwani/Hospital-_-Patient-_-Details/assets/155231669/47722b03-b0c7-45ec-8141-8aed77dbcdcc>

</p>
There are three tables Inpatient, outpatient and all data which are created. Since I have already appended are inpatient and outpatient data in all data. Avoiding confusion both the table was hiding. Created additional mapping table which maps all the specialties to a certain specialty group in a csv file. Modeled data by creating a relationship between mapping specialty and all data.
Simply means that the filter context is flowing from mapping table to my all data.




<p><h3>SUMMARY </h3></p>
<img src=https://github.com/AloraKesharwani/Patient_Health_Analysis/assets/155231669/5b2e2192-059b-4d81-bda1-57790f56b015>
<p>
 
  <b>TOP LEFT SECTION:</b> 
  </p>
  
  In top left section, there are two numbers that will show the current month wait list versus the same month previous year wait list. For this, we can use a card visual, but for the numbers, we need the total wait list column. We will use DAX to make a more dynamic card and create a new measure called " Latest Month Wait List." This will display the current month's wait list.

Similarly, create a new measure for the same month previous year named "Previous Year Latest Month Wait List, now displaying the number or count of waiting lists for the previous year of the same month.

In Top, also create a few filters for the overall dashboard functioning, which will be the month, casetype, specialty, and archive date column.
Indication: Create explicit titles that will show whether the average is selected or the median is selected, and create a new measure named Dynamic Title (Key Indicator Wait List).
</p>
<p>
  <b>MIDDLE SECTION:</b> 
  
 In this section, we use three different charts: the donut chart, the stacked column chart, and the multi-row card. Donut chart showing a bifurcation between outpatient, inpatient, and day-case waiting lists a stacked column chart displaying the relationship between the time brand and age profile, and a grid that showcases the top specialties. All this chart showcases average wait list values. There are a couple of outliers that only have averages in the dashboard, which will not be sufficient, so we would like to add the median waiting list as well, but in order to add two metrics to the same chart, we created some kind of toggle mechanism using which users can easily switch between any metric they want. There are many ways to do this, but stick to a simple method that will be easier to grasp.

Before we create that toggle button, we need to create a blank table that will host the value of the matrix that we are trying to toggle, which is Average and Median. This table is named the calculation method for the slicer.

Create two measures, which will be average waiting and median waiting list, in the average waiting list, which contains the average of the total column, and the median waiting list, which contains the median of the total weight list column. Create one more measure, which will enable us to interact with this button and switch between these two metrics. Let’s name this as average/median wait list.
</p>
<p>
  <b>BOTTOM SECTION: </b> 
  
</p>The line chart will show the total wait list in case type. In this chart, we use day case and inpatient data. Create a same-line chart by using outpatient data. Monthly trend analysis on the basis of inpatient, daycase, and outpatient will showcase the total wait list for a particular category.
</p>
<p>
  <p><h3>DETAILED </h3></p>
  
<img src=https://github.com/AloraKesharwani/Patient_Health_Analysis/assets/155231669/72fbaabf-e706-46a4-80fe-ebae270d9241>
</p>

  In this dashboard, add a slicer named archive data, casetype, speciality, age profile, or timeband. Use a grid or table instead of this simple table, add some value to the data, and use a matrix view. This will give us an option to summarise the data and may create some other type of transformation within this view, which will be beneficial for the end user for granular-level analysis.

</p>
<p>
   <p><h3>DRILLDOWN </h3></p>

   <img src=https://github.com/AloraKesharwani/Patient_Health_Analysis/assets/155231669/72fbaabf-e706-46a4-80fe-ebae270d9241>
</p>

   

Creating a pop-up window of some sort that will show a split of specialties for that particular month, specifically using the speciality group, will use the speciality column now and add a new pop-up window that will show a different kind of view without wasting any of the real estate in this dashboard. Add one more page named DrillDown, add a chart using the specialty mapping, and use a card to see the total number of waitlists for that particular month in this kind of view. When users hover on a line chart and it's going to show an entire drilldown page with that particular view and move the cursor, the views are also getting filtered accordingly.  

</p>

<p>Jan 2024 <p/>
