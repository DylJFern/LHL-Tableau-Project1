# Data Visualization and Dashboards with Tableau

## Project/Goals
The objective of this project was turn data into easily consumable visual insights using Tableau by creating an impactful dashboard communicated with correct visualizations to help stakeholders make decisions (based on business questions).

## <br>Process
1. Select and connect to a dataset.
2. Examine different datatypes and available fields.
3. Build visualizations to learn more about the dataset.
    - incorporate the main categorical features: effect, when and wildlife.
4. Find any patterns, trends and outliers within the data.
5. Create a 'story' to annotate any keypoints, findings, or assumptions made.
6. Create a 'dashboard' to answer questions about the data.

## <br>Results
Option 2: 2015 FAA Wildlife Strikes

### Visualizations Used
- Map chart: to see how the number of strikes vary based on state.

- Forecast line chart: to observe the number of strikes over the years and predict the current year data to determine how accurate the model is when compared to actual reported data.

- Treemap chart: to determine the relative sizes by number of strikes of each species within each category.

- Stacked bar chart: to show a how the number of strikes over the years changes depending on the time of day and unlike a scatterplot variation of this visualization, we can see a cumulative sum depending on the selection of time of day (whereas a scatterplot would only show individual values).

- Highlight table: to depict the effect the damage has on the impact of the flight based on the number of strikes, as text with important numbers enhanced by colour variation.

- Horizontal bar: to provide information on the number of strikes at each phase of flight with corresponding associated costs of each phase.

### <br>Exploratory Data Analysis Process
-  Data for the year 2015 was found to be incomplete and was removed for all visualizations.

![PPT-NullView1](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/4bba386d-34c8-466d-9755-7564e8cb872e)

- The visualizations and dataset depicted outliers, for example the overall trend of the data showed that the number of strikes increased with each passing year. However, for specific times of day like "dusk", outliers could be considered present for years 2008 and 2009 where the data did not follow the same trend. Data containing outliers was left unmodified.

![PPT-OutlierView2](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/5277e405-4e63-40e6-96f0-50b332bab780)

- The visualizations containing null data was 'excluded' from view or filtered out with sets and other sheet settings (e.g. filter applied across all worksheets).

- The visualizations containing blank field(s) were adjusted using a calculated field.

![PPT-NullView3(3)](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/fe891181-3eb8-4169-b2c2-2cbbae50fd16)

### <br>Questions To Be Answered

Using the [dashboard](https://github.com/DylJFern/LHL-Tableau-Project1/blob/master/images/2015%20FAA%20Wildlife%20Strikes%20Dashboard.png), the following questions can be answered.

#### Where do wildlife strikes most frequently occur?
The highest number of strikes is 2,827, 2,126 and 2,116 which occur in California, Texas and Florida, respectively.

![PPT-ImgMap](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/5207a58f-3807-47a0-8fd6-49d5b64a49a6)

#### What is the trend of wildlife strikes over the years? How accurate is the model at predicting future results?

The number of strikes for each year of collision depicts exponential growth. The filtered model predicts that approximately 12,000 wildlife strikes will occur in the year 2022. However, the actual reported number of strikes is 17,190 for the year 2022 based on a [1990-2022 FAA Wildlife Strike Report](https://www.faa.gov/airports/airport_safety/wildlife/wildlife_strikes_civil_aircraft_united_states_1990_2022). Therefore, the model is not accurate in predicting future results.

![PPT-ImgForecast(1)](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/b338a8c9-12c0-4cc1-b620-f421b2cbbe14)

#### Are there particular wildlife categories more commonly involved? Of the categories, which wildlife species are most frequently involved?

Birds account for majority of the wildlife strikes. More specifically, perching birds (e.g. crows, mockingbirds and sparrows) are the most prone to incidents. They make up 10,779 of the total 26,180 strikes costing $7,887,249, whereas ducks, geese, swans, waterfowl make up only 1,593 of the total number of strikes yet cause the most damage (have the highest cost of $134,059,243).

#### What is the impact of strikes on flight operations? How does the effect of strikes vary with the phase of flight?
Overall, there is little to no impact of strikes on flight operations as most of the strikes occur during "approach", "landing roll" and "take-off run" phases of flight which are at low altitude and speed. This large number of wildlife strikes can be attributed to the fact that bird populations (and other flightless animals) tend to congregate near airports due to availability of food sources (e.g. insects, vegetation, or waste). On the other hand, the reduced severity of damage at lower altitudes and speeds is primarily due to the decrease in kinetic energy, impact force, momentum, and stress on aircraft components.

![PPT-ImgHighlightedTable(1)](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/da2d6257-f7dd-457c-8eaa-922f1343ebdf)

![PPT-ImgHorizontalBar(1)](https://github.com/DylJFern/LHL-Tableau-Project1/assets/128000630/daa52f6d-e11a-4dc2-8bd4-6a863935f84f)

#### How does the cost associated with the different phases of flight vary? What are possible causes?
Conversely, the total cost is highest for the "climb" phase compared to the others because the aircraft in this stage will be gaining altitude and accelerating, the engines will be consuming more power but will also be more suspectible to damage from wildlife strikes (and since the cost of engines are generally the most expensive, this will drive up the costs significantly), and the bird size and mass will (typcially) increase (at these higher altitudes) resulting in a larger impact collision between both objects when travelling at greater speeds.

## <br>Challenges 
- The dataset did not include other useful/relevant data, for example it could have included the number of flights such that any correlation between the number of strikes and the number of flights or the types of aircraft.
- Developing a user-friendly dashboard that balances analysis with a clear flow of information whilst considering varying desktop sizes, whether or not the user is colourblind, and so on.
- Ensuring data quality (methods of dealing with null, outliers and inconsistencies)

## Future Goals
- Examining different visualizations based on a different set of questions.
- Expore other data and make additional comparisons between the current dataset (we are using) and the existing reported data documentation by FAA.
