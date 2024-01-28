# PATIENT_HEALTH_ANALYSIS
<p>In this dashboard, we analyse the historical monthly trend of waiting lists in inpatient or outpatient categories, where Inpatient means a patient who stays in a hospital while under treatment and Outpatient means a patient who receives medical treatment without being admitted to a hospital. A comprehensive overview of the patient's medical history, including past illnesses, surgeries, allergies, chronic conditions, etc., is presented on the dashboard. Detailed specialty level and age profile analysis. Use the folder connector and use multiple Excel files to collate them together and then import them.

  Combine both inpatient and outpatient data sets together to get a single set of data that will be used for visualisation purposes. Append tables, append both sets of data together, and rename it ALL DATA.

  <p><h3>DATA MODEL</h3></p>
<img src=https://github.com/AloraKesharwani/Hospital-_-Patient-_-Details/assets/155231669/47722b03-b0c7-45ec-8141-8aed77dbcdcc>


There are three tables Inpatient, outpatient and all data which are created. Since I have already appended are inpatient and outpatient data in all data. Avoiding confusion both the table was hiding. Created additional mapping table which maps all the specialties to a certain specialty group in a csv file. Modeled data by creating a relationship between mapping specialty and all data.
Simply means that the filter context is flowing from mapping table to my all data.


<p><h3>SUMMARY </h3></p>
<img src=https://github.com/AloraKesharwani/Patient_Health_Analysis/assets/155231669/5b2e2192-059b-4d81-bda1-57790f56b015>
<p>
  <b>1. PROFIT BY YEAR AND QUATER:</b> 
  
 The profit chart shows the overall view of profit in each quarter and year.Sum up the profits for each quarter to get the total profit for each year.In 2018, profits seem to be increasing from Q1 to Q4, with Q4 being the most profitable quarter.In 2023, there is a slight dip in Q1, but profits increase again in Q2, Q3, and Q4.
Analyse each quarter individually to understand the factors contributing to fluctuations in profits.Identify whether profits are consistently growing, declining, or remaining stable.
</p>
<p>
  <b>2. PROFIT BY PRODUCTS:</b> 
  
  Compare profits for each product to identify which products are the most profitable and contribute significantly to overall store profits.Identify products that are often purchased together. This information can be used to create cross-selling strategies.Some products are in the growth phase, maturity, or decline phase, and adjust marketing and inventory strategies accordingly.
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
