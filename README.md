# London Bike Sharing Dashboard

<div align="center">
    <img src="https://www.verdict.co.uk/wp-content/uploads/2018/05/santander_bikes.jpg" width="500px">
</div>

## Introduction:
**London Bike Sharing** service is a prevalent choice among commuters and tourists in London. This project leverages the London Bike Sharing Dataset from Kaggle to analyze usage patterns across different seasons, weather conditions, and holidays to forecast demand and improve service efficiency.

## Project Objective 🎯:
This project aims to understand and visualize the dynamics of bike-sharing usage in London to enhance operational decisions and customer satisfaction through data-driven insights.

### Key Performance Indicators include 🔑:
| Objective                            | Description                                                    |
|--------------------------------------|----------------------------------------------------------------|
| **Total Bike Rides**                 | Track the total number of bike rentals.                        |
| **Ride Frequency by Weather**        | Analyze how weather conditions affect bike usage.              |
| **Effect of Holidays on Bike Usage** | Evaluate changes in bike rental patterns during holidays.      |
| **Seasonal Usage Patterns**          | Understand how different seasons impact bike sharing.          |
| **Hourly Usage Trends**              | Identify peak usage hours to optimize bike availability.       |

## Dashboard 🎛:

![London Bike Sharing Dashboard](https://github.com/sanidhya-mitra/Pedal-Pulse-London/blob/main/Pedal%20Pulse%20London%20Dashboard.gif)

## Data Source 📁:

This project utilizes the London Bike Sharing dataset from Kaggle, which includes comprehensive data such as hourly bike rental numbers, weather conditions, and seasonal information spanning from January 2015 to December 2016. 

For access to the dataset and the Tableau workbook used in this analysis, please use the following links:

<p align="center">
    <a href="https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset?resource=download">
        <img src="https://www.svgrepo.com/show/349422/kaggle.svg" width="60px" alt="Kaggle Dataset"><br>
        Access
    </a>
</p>

## Tools and Skills Used 🛠️:

<div align="center">
    <table>
        <tr>
            <td align="center"><img alt="Tableau" width="35px" src="https://cdn.worldvectorlogo.com/logos/tableau-software.svg"/><br>Tableau</td>
            <td align="center"><img alt="Python" width="35px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg"/><br>Python</td>
            <td align="center"><img alt="Pandas" width="35px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original-wordmark.svg"/><br>Pandas</td>
        </tr>
    </table>
</div>

## Technical Workflow 🖥️:

1. **Data Acquisition**: Programmatic download of data using Kaggle API.
2. **Data Preprocessing and Analysis**: Data manipulation using Python and Pandas.
3. **Visualization**: Dynamic visualizations created in Tableau.

## Challenges Faced 😵:

### Challenge 1: Authenticating Kaggle API
**Issue**: After importing the Kaggle library, I encountered an `OSError` because the `kaggle.json` file was somehow initially missing, causing authentication to fail.<br><br>
**Resolution**: Generated a new API token by accessing my Kaggle account settings and downloading the `kaggle.json` file. Ensured the file was correctly saved in the specified `.kaggle` directory under my user profile, followed by setting the appropriate file permissions for security.

### Challenge 2: Adjusting Time Display in Tableau
**Issue**: After the "time" field was dragged into the Rows shelf, by default, Tableau displayed the "time" field from the dataset in a 24-hour format, starting at 0 and ending at 23. This was technically correct but not aligned with typical user expectations, who prefer hours numbered from 1 to 24.

**Resolution**: After exploring several Tableau community forums for guidance, I constructed a calculated field to adjust the hour display. The solution involved using the formula `IF [Hour] = 0 THEN 24 ELSE [Hour] END`, effectively mapping the '0' hour to '24' for better readability and to meet user preferences. This adjustment improved the clarity and usability of the hourly data in the dashboard.

## Techincal Breakthrough🏆: Advanced Tooltips in Tableau
**Overview**: Successfully implemented advanced dynamic tooltips in Tableau for the first time.

**Details**: Following a [video tutorial](https://www.youtube.com/watch?v=P1V3SPiiPM8), I learned Tableau's 'Viz in Tooltip' feature, embedding extra visual elements directly within tooltips. This enhancement allowed for displaying detailed data like weather conditions and hourly distributions on hover, significantly improving the dashboard's interactivity and user experience without overcrowding the main view.


## Data Insights and Visualizations 📊:

- **Interactive Time Series Analysis**: Visualizing bike usage over time.
- **Weather Impact Study**: Heatmap correlating temperature, wind speed, and bike rentals.

## Conclusion and Insights 💡:

The dashboard reveals key insights into factors affecting bike rental volumes, enabling strategic improvements for operational efficiency and customer satisfaction.<br><br>

View the live Tableau Dashboard here:

<p align="center">
    <a href="https://public.tableau.com/app/profile/sanidhya.mitra4662/viz/LondonBikeRideAnalytics/Dashboard1">
        <img src="https://www.svgrepo.com/show/324142/dashboard-graph-analytics-report.svg" width="65px" alt="Access Dataset"><br>
        View
    </a>
</p> <br>

Or download my London Bike-Share Analytics Workbook:
<p align="center">
    <a href="https://github.com/sanidhya-mitra/Pedal-Pulse-London/blob/main/London%20Bike%20Ride%20Analytics.twbx">
        <img src="https://analyticscanvas.com/wp-content/uploads/2016/02/twbx.png" width="60px" alt="Tableau Workbook"><br>
        Download
    </a>
</p>

---

<div align="center">
Thank you for taking the time to explore the Pedal Pulse London project! Your interest and feedback are invaluable to me. I greatly appreciate your interest.
Feel free to reach out for any questions or suggestions about this project. I'm open to discussions and eager to assist. <br>
    🌐 Connect with me on <a href="https://www.linkedin.com/in/sanidhya-mitra">LinkedIn | Sanidhya Mitra</a> <br>
Don't forget to follow and star ⭐ the repository if you find it valuable.
</div>
