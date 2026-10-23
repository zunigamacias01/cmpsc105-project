# Summary of Exploratory Data Analysis for CMPSC 105 Project

## About the Dataset
This dataset is about NYC service requests. It shows how often people in the area complain about various issues, including noise, heat and hot water, and street conditions.

The dataset includes the following information:
- Created date
- Closed date
- Agency name
- Problem category and details
- Location type
- Address
- Latitude and longitude
- Complaint-specific information, such as "Road Ramp" and "Park Facility Name"

Top 10 complaint categories:
1. Heat/Hot Water
2. Illegal Parking
3. Noise - Residential
4. Snow/Ice
5. Blocked Driveway
6. Unsanitary Condition
7. Plumbing
8. Water System
9. Paint/Plaster
10. Door/Window

We chose January for our analysis because it includes winter-related problems, such as snow and ice, which may help us understand seasonal issues. We expect to see a variety of problems and longer resolution times compared to other months due to weather conditions.

## Method Used to Clean the Data
We started by removing 33 columns and filtering the dataset to include only illegal parking complaints. Next, we checked for missing values and invalid data, but we did not find any such cases among the records we examined, including complaints that had not been closed. We removed two rows with unspecified boroughs.

For data types, we converted the created and closed dates from text to date-time values so we could calculate the time spent resolving each issue. We also converted ZIP codes from decimals to whole numbers.

## Dataset Quirks
We chose illegal parking for our investigation because NYC is known for its large population and heavy traffic.

We intend to focus on differences in the time it takes to close a complaint across boroughs. By comparing resolution times for illegal parking complaints, we want to understand differences in response efficiency across boroughs and suggest how the city council and mayor could allocate money and resources.

## Descriptive Statistics for Illegal Parking (in hours)
- Number of complaints: 48,715
- Mean resolution time: 2.41 hours
- Median resolution time: 1.42 hours
- Standard deviation: 2.88 hours
- Minimum resolution time: 0.0 hours
- Maximum resolution time: 56.33 hours

## Plotted Dataset
The plots are available in the Jupyter Notebook.