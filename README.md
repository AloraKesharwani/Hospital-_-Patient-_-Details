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
</p>
<p>
  <b>MIDDLE SECTION:</b> 
  
 In this section, we use three different charts: the donut chart, the stacked column chart, and the multi-row card. Donut chart showing a bifurcation between outpatient, inpatient, and day-case waiting lists a stacked column chart displaying the relationship between the time brand and age profile, and a grid that showcases the top specialties. All this chart showcases average wait list values. There are a couple of outliers that only have averages in the dashboard, which will not be sufficient, so we would like to add the median waiting list as well, but in order to add two metrics to the same chart, we created some kind of toggle mechanism using which users can easily switch between any metric they want. There are many ways to do this, but stick to a simple method that will be easier to grasp.

Before we create that toggle button, we need to create a blank table that will host the value of the matrix that we are trying to toggle, which is Average and Median. This table is named the calculation method for the slicer.

Create two measures, which will be average waiting and median waiting list, in the average waiting list, which contains the average of the total column, and the median waiting list, which contains the median of the total weight list column. Create one more measure, which will enable us to interact with this button and switch between these two metrics. Let’s name this as average/median wait list.
</p>
<p>
  <b>3. PROFIT BY SUB- CATEGORY AND REGIONS:</b> 
  
</p>The profit by subcategories and region provides a variety of filters. The users can also filter the visualisations in the dashboard by region and sub-categories. The dashboard is dynamic, and the filter will be applied to all the visualisations available in the matrix chart.These matrix charts can help the business optimise its profit by region and subcategories.The profit matrix chart is a valuable visualisation that can provide an overall view of the subcategories of each region.
</p>
<p>
  <b>4. PROFIT BY CATEGORY:</b> 
  
The profit by category chart gives managers the ability to have a wide range of information in just one chart, by drilling up they can have information about the overall profit of each product category and by drilling down they can find the most valuable products and the slow-mover ones. This can help production to put their resources into producing profitable goods and perhaps stop the production of goods with little to no profit
</p>
<p>
  <b>5. PROFIT BY STATES:</b> 
  
  Determining the top-performing state by analysing various metrics. By evaluating metrics such as total sales, customer acquisition, and profitability by state, businesses can identify the region contributing the most to overall success. This analysis guides strategic decisions, allowing businesses to focus resources, marketing efforts, and customer engagement strategies on the top-performing state for sustained growth and market dominance. Identifying and targeting top customers based on higher spending for special discounts and coupons is a strategic approach to cultivating preferred customer relationships.
</p>

<p>Jan 2024 <p/>
