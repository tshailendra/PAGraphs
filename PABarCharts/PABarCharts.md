# PowerApps BarCharts

Provides a better graphs for Power App Canvas Apps using [PABarCharts.zip](https://github.com/)

## Deployment

Open [PowerApps](https://make.powerapps.com/)

From **Solutions** Node

-   Click Import
-   Browse the zip file downloaded from [Git](https://github.com)
-   Follow the steps to import the solution

## Development

-   Open your PowerApp
-   Ensure you enable "Components" in the App > Settings > Advanced Settings > Preview Features
    -   Insert Menu > Custom Import Components > Code
    -   Select **Bar Chart**
    -   Insert Bar Chart from code components
    -   set the Items property to a collection
    -   In the properties tab add fields
    -   Select the fields based on the Chart Type
    -   You can set a property as:
        -   **'PAGraphs.BarCharts.bcBorderType'.bcGraphRoundedShadow**
        -   **"graphroundedshadow"**

### Sample Chart

### Properties

Most properties have default values. However, you can change the values as per your requirement.

For PowerApps Bar Graph all properties are prefixed with "bc"

| Property                 | Description                                                                                                                                                                                     |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| bcAnimateDuration        | Animation Duration (in milli secs)                                                                                                                                                              |
| bcBackGroundColor        | To change the background color of the Graph. Refer Colors section below                                                                                                                         |
| bcBorderType             | Border of the Chart control. Valid values are:<ul><li>bcNone</li><li>bcGraphShadow</li><li>bcGraphNoShadow</li><li>bcGraphRoundedNoShadow</li><li>bcGraphRoundedShadow</li></ul>                |
| bcChartType              | Show the Graph in <ul><li>bcSimple (simple Bars)</li><li>bcStacked (Stacked Bar)</li></ul>. Refer Stacked View section for details                                                              |
| bcColors                 | Override the default colors. Based on the data provide custom colors as comma separated values. Refer Colors section for details                                                                |
| bchAxisMinValue          | Change the Horizontal Axis Min Value (default 0)                                                                                                                                                |
| bchAxisTextBold          | Display Horizontal Axis Text in Bold (true or false)                                                                                                                                            |
| bchAxisTextColor         | Change the Horizontal Axis Text color                                                                                                                                                           |
| bchAxisTextDateFormat    | Currently this feature is disabled                                                                                                                                                              |
| bchAxisTextFontName      | Set the Font Name of Horizontal Axis Text                                                                                                                                                       |
| bchAxisTextFontSize      | Set the Font Size of Horizontal Axis Text                                                                                                                                                       |
| bchAxisTextFormat        | Change the Horizontal Axis Text format. Valid values are: <ul><li>bcNone</li><li>bcDecimal</li><li>bcCurrency</li><li>bcShort (Shows 1M instead of 1,000,000)</li></ul>                         |
| bchAxisTextItalic        | Display Horizontal Axis Text to Italic (default false)                                                                                                                                          |
| bchAxisTitle             | Horizontal Axis Title                                                                                                                                                                           |
| bchAxisTitleTextBold     | Set the Horizontal Axis Title to Bold (default true)                                                                                                                                            |
| bchAxisTitleTextColor    | Change the Horizontal Axis Title color                                                                                                                                                          |
| bchAxisTitleTextFontName | Set the Font Name of Horizontal Axis Title                                                                                                                                                      |
| bchAxisTitleTextFontSize | Set the Font Size of Horizontal Axis Title                                                                                                                                                      |
| bchAxisTitleTextItalic   | Display Horizontal Axis Title to Italic (default false)                                                                                                                                         |
| bcLegend                 | Show the Legend by setting one of the values: <ul><li>bcNone (to remove Legend) </li><li>bcLabeled</li><li>bcRight</li><li>bcBottom</li><li>bcTop</li></ul>                                     |
| bcLegendTextBold         | Set the Legend Text to Bold (default false)                                                                                                                                                     |
| bcLegendTextColor        | Change the Legend Text color                                                                                                                                                                    |
| bcLegendTextFontName     | Set the Font Name of Legend Text                                                                                                                                                                |
| bcLegendTextFontSize     | Set the Font Size of Legend Text                                                                                                                                                                |
| bcLegendTextItalic       | Display Legend Text to Italic (default false)                                                                                                                                                   |
| bcLegendWidth            | Increase (positive value) or decrease (negative value) the Legend Width                                                                                                                         |
| bcOrientation            | Orientation of Graph <ul><li>Vertical - bcVertical</li><li>Horizontal - bcHorizontal</li></ul>                                                                                                  |
| bcRightYAxis             | Show Y Axis to right side of graph                                                                                                                                                              |
| bcStackedMultiSeries     | Show Graph in multi series instead of stacked. Refer Stacked View section below                                                                                                                 |
| bcStackFullWidth         | Show Stacked Graph 100% width of the available chart width                                                                                                                                      |
| bcSubTitle               | Set Sub Title of the Graph                                                                                                                                                                      |
| bcSubTitleTextColor      | Change the Sub Title Text color                                                                                                                                                                 |
| bcSubTitleTextFontName   | Set the Font Name of Sub Title Text                                                                                                                                                             |
| bcSubTitleTextFontSize   | Set the Font Size of Sub Title Text                                                                                                                                                             |
| bcSubTitleTextFontStyle  | Set the Sub Title Text to either: <ul><li>bcNormal</li><li>bcOblique</li><li>bcItalic</li></ul>                                                                                                 |
| bcSubTitleTextFontWeight | Set the Sub Title Text to either: <ul><li>bcNormal</li><li>bcLight</li><li>bcLighter</li><li>bcBold</li><li>bcBolder</li></ul>                                                                  |
| bcTitle                  | Set Title of the Graph                                                                                                                                                                          |
| bcTitleTextColor         | Change the Title Text color                                                                                                                                                                     |
| bcTitleTextFontName      | Set the Font Name of Title Text                                                                                                                                                                 |
| bcTitleTextFontSize      | Set the Font Size of Title Text                                                                                                                                                                 |
| bcTitleTextFontStyle     | Set the Title Text to either: <ul><li>bcNormal</li><li>bcOblique</li><li>bcItalic</li></ul>                                                                                                     |
| bcTitleTextFontWeight    | Set the Title Text to either: <ul><li>bcNormal</li><li>bcLight</li><li>bcLighter</li><li>bcBold</li><li>bcBolder</li></ul>                                                                      |
| bcTransposeData          | Transpose the provide data                                                                                                                                                                      |
| bcvAxisTextBold          | Set the Vertical Axis Text to Bold (default false)                                                                                                                                              |
| bcvAxisTextColor         | Change the Vertical Axis Text color                                                                                                                                                             |
| bcvAxisTextDateFormat    | Currently this feature is disabled                                                                                                                                                              |
| bcvAxisTextFontName      | Set the Font Name of Vertical Axis Text                                                                                                                                                         |
| bcvAxisTextFontSize      | Set the Font Size of Vertical Axis Text                                                                                                                                                         |
| bcvAxisTextFormat        | Change the Vertical Axis Text format. Valid values are:<ul><li>bcNone</li><li>bcDecimal</li><li>bcCurrency</li><li>bcShort (Shows 1M instead of 1,000,000)</li></ul>                            |
| bcvAxisTextItalic        | Display Vertical Axis Text to Italic (default false)                                                                                                                                            |
| bcvAxisTitle             | Vertical Axis Title                                                                                                                                                                             |
| bcvAxisTitleTextBold     | Set the Vertical Axis Title to Bold (default true)                                                                                                                                              |
| bcvAxisTitleTextColor    | Change the Vertical Axis Title color                                                                                                                                                            |
| bcvAxisTitleTextFontName | Set the Font Name of Vertical Axis Title                                                                                                                                                        |
| bcvAxisTitleTextFontSize | Set the Font Size of Vertical Axis Title                                                                                                                                                        |
| bcvAxisTitleTextItalic   | Display Vertical Axis Title to Italic (default false)                                                                                                                                           |
| bcEnableConsoleLog       | Set to true to enable log in Console                                                                                                                                                            |
| bcEnableGraphClick       | Set to true to enable Click event within graph. On click the graph returns values which can be accessed through the below properties: <ul><li>bcSelectedData1</li><li>bcSelectedData2</li></ul> |
| bcSelectedData1          | Get X axis value (on click)                                                                                                                                                                     |
| bcSelectedData2          | Get Y axis value (on click)                                                                                                                                                                     |
| bcDataCollection         | Set the data collection to display graph                                                                                                                                                        |

### **Colors**

You can provide colors in either formats:<ul><li><b>#ff0000, #00ff00, #0000ff</b></li><li><b>red, green, blue</b></li></ul>

### **Stacked View**

To show the graph is Stacked View

-   Write MORE Tests
-   Add Night Mode