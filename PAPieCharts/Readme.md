# PowerApps PieCharts

Provides a better graphs for Power App Canvas Apps using [PAPieCharts](./Solution/PAPieCharts.zip)

## Deployment

Open [PowerApps](https://make.powerapps.com/)

From **Solutions** Node

-   Click Import
-   Browse the zip file downloaded from [PAPieCharts](./Solution/PAPieCharts.zip)
-   Follow the steps to import the solution

![Deployment](./images/pcSolutionsImport.png?raw=true)

## Development

-   Open your PowerApp
-   Ensure you enable "Components" in the App > Settings > Advanced Settings > Preview Features
-   Insert Menu > Custom Import Components > Code

    ![PieChart](./images/pcImportComponent.png?raw=true)

-   Select **PieChart**
-   Insert PieCharts from code components
-   Set the Items property to a collection
-   In the properties tab add fields
-   Select the fields based on the Chart Type
-   You can set a property as:
    -   **'PAGraphs.PieCharts.pcBorderType'.pcGraphRoundedShadow**
    -   **"graphroundedshadow"**

![Properties](./images/PieChartProperties.png?raw=true)

### Sample Charts

-   Donut Charts
-   Set pcLegend as "labeled"
-   Set pcSliceText as "value"

![Donut Charts](./images/pcDonutChart.png?raw=true)

-   3D Charts
-   Set pcIs3D to "true"

![3D Charts](./images/pc3DPieChart.png?raw=true)

### Properties

Most properties have default values. However, you can change the values as per your requirement.

For PowerApps Bar Graph all properties are prefixed with "pc"

| Property                 | Description                                                                                                                                                                      |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| pcBackGroundColor        | To change the background color of the Chart. Refer Colors section below                                                                                                          |
| pcBorderType             | Border of the Chart control. Valid values are:<ul><li>pcNone</li><li>pcChartShadow</li><li>pcChartNoShadow</li><li>pcChartRoundedNoShadow</li><li>pcChartRoundedShadow</li></ul> |
| pcChartHole              | Set a value to show donut Chart                                                                                                                                                  |
| pcColors                 | Override the default colors. Based on the data, provide custom colors as comma separated values. Refer Colors section for details                                                |
| pcIs3D                   | Set to true for 3D Pie Chart                                                                                                                                                     |
| pcLegend                 | Show the Legend by setting one of the values: <ul><li>pcNone (to remove Legend) </li><li>pcLabeled</li><li>pcLeft</li><li>pcRight</li><li>pcBottom</li><li>pcTop</li></ul>       |
| pcLegendTextBold         | Set the Legend Text to Bold (default false)                                                                                                                                      |
| pcLegendTextColor        | Change the Legend Text color                                                                                                                                                     |
| pcLegendTextFontName     | Set the Font Name of Legend Text                                                                                                                                                 |
| pcLegendTextFontSize     | Set the Font Size of Legend Text                                                                                                                                                 |
| pcLegendTextItalic       | Display Legend Text to Italic (default false)                                                                                                                                    |
| pcLegendWidth            | Increase (positive value) or decrease (negative value) the Legend Width                                                                                                          |
| pcSliceText              | Set the Slice Title of the Chart                                                                                                                                                 |
| pcSliceTitleTextBold     | Set the Slice Title to Bold (default true)                                                                                                                                       |
| pcSliceTitleTextColor    | Change the Slice Title color                                                                                                                                                     |
| pcSliceTitleTextFontName | Set the Font Name of Slice Title                                                                                                                                                 |
| pcSliceTitleTextFontSize | Set the Font Size of Slice Title                                                                                                                                                 |
| pcSliceTitleTextItalic   | Display Slice Title to Italic (default false)                                                                                                                                    |
| pcSubTitle               | Set Sub Title of the Chart                                                                                                                                                       |
| pcSubTitleTextColor      | Change the Sub Title Text color                                                                                                                                                  |
| pcSubTitleTextFontName   | Set the Font Name of Sub Title Text                                                                                                                                              |
| pcSubTitleTextFontSize   | Set the Font Size of Sub Title Text                                                                                                                                              |
| pcSubTitleTextFontStyle  | Set the Sub Title Text to either: <ul><li>pcNormal</li><li>pcOblique</li><li>pcItalic</li></ul>                                                                                  |
| pcSubTitleTextFontWeight | Set the Sub Title Text to either: <ul><li>pcNormal</li><li>pcLight</li><li>pcLighter</li><li>pcBold</li><li>pcBolder</li></ul>                                                   |
| pcTitle                  | Set Title of the Chart                                                                                                                                                           |
| pcTitleTextColor         | Change the Title Text color                                                                                                                                                      |
| pcTitleTextFontName      | Set the Font Name of Title Text                                                                                                                                                  |
| pcTitleTextFontSize      | Set the Font Size of Title Text                                                                                                                                                  |
| pcTitleTextFontStyle     | Set the Title Text to either: <ul><li>pcNormal</li><li>pcOblique</li><li>pcItalic</li></ul>                                                                                      |
| pcTitleTextFontWeight    | Set the Title Text to either: <ul><li>pcNormal</li><li>pcLight</li><li>pcLighter</li><li>pcBold</li><li>pcBolder</li></ul>                                                       |
| pcEnableConsoleLog       | Set to true to enable log in Console                                                                                                                                             |
| pcEnableGraphClick       | Set to true to enable Click event within Chart. On click the Chart returns values which can be accessed through the below properties: <ul><li>pcSelectedData</li></ul>           |
| pcSelectedData           | Get Slice value (on click)                                                                                                                                                       |
| pcDataCollection         | Set the data collection to display Chart                                                                                                                                         |

### **Colors**

You can provide colors in either formats:<ul><li><b>#ff0000, #00ff00, #0000ff</b></li><li><b>red, green, blue</b></li></ul>
