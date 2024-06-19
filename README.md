# ECharts Gantt Chart Example
This project provides an example of creating a Gantt chart using ECharts. You can modify the status and color settings, as well as the data for the Gantt chart via specific textareas in the HTML file.

## Setup
Include the following CDN links in your HTML file:

   ```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/echarts/5.1.2/echarts.min.js"></script>
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
<script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
   ```

## Customization
### Status and Color Settings
You can modify the status and color settings in the textarea with id="status_color_dict". Here is an example format:
   ```json
{
    "Green": "#2DB884",
    "Yellow": "#F8E571",
    "Dark Blue": "#3B579A",
    "Red": "#D04551",
    "Pink": "#F1A7B8"
}
   ```
### Gantt Chart Data
You can modify the Gantt chart data in the textarea with id="data". 
 * The "Start_Time" defines the starting value of the X-axis.
 * The "End_Time" defines the ending value of the X-axis.
 *  The keys in the "data" object represent the values on the Y-axis.
   
Here is an example format:
   ```json
{
    "Start_Time": "2023-01-05T00:00:00.000",
    "End_Time": "2023-01-05T10:00:00.000",
    "data": {
        "A": {
            "0": {
                "STime": "2023-01-04 22:40:20",
                "ETime": "2023-01-05 01:04:03",
                "Comment": "Green stuff",
                "Status": "Green"
            },
            "1": {
                "STime": "2023-01-05 01:04:03",
                "ETime": "2023-01-05 01:46:45",
                "Comment": "Dark Blue stuff",
                "Status": "Dark Blue"
            }
        },
        "B": {
            "0": {
                "STime": "2023-01-04 21:40:20",
                "ETime": "2023-01-05 02:04:03",
                "Comment": "Yellow stuff",
                "Status": "Yellow"
            },
            "1": {
                "STime": "2023-01-05 02:04:03",
                "ETime": "2023-01-05 02:10:45",
                "Comment": "Pink stuff",
                "Status": "Pink"
            },
            "2": {
                "STime": "2023-01-05 02:10:45",
                "ETime": "2023-01-05 08:00:00",
                "Comment": "Red stuff",
                "Status": "Red"
            }
        }
    }
}

   ```
