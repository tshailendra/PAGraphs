# PowerApps LineCharts

Provides a better graphs for Power App Canvas Apps using [PALineCharts](./Solution/PALineCharts.zip)

## Deployment

-   Open [PowerApps](https://make.powerapps.com/)

-   From **Solutions** Node

    -   Click Import
    -   Browse the zip file downloaded from [PALineCharts](./Solution/PALineCharts.zip)
    -   Follow the steps to import the solution

    ![Deployment](./images/lcSolutionsImport.png?raw=true)

## Development

-   Open your PowerApp
-   Ensure you enable "Components" in the App > Settings > Advanced Settings > Preview Features
-   Insert Menu > Custom Import Components > Code
    ![LineChart](./images/lcImportComponent.png?raw=true)

-   Select **LineCharts**
-   Insert BarCharts from code components
-   Set the Items property to a collection
-   In the properties tab add fields
-   Select the fields based on the Chart Type
-   You can set a property as:
    -   **'PAGraphs.LineCharts.lcBorderType'.lcGraphRoundedShadow**
    -   **"graphroundedshadow"**

![Properties](./images/LineChartProperties.png?raw=true)

### Sample Chart

-   Chart displayed based on transpose data (refer BarChart for transpose)
-   Set lcBackGroundColor to "#0079BB"
-   Set lcLegend as "bottom"
-   Set lcPointShape as "diamond"
-   Set lcPointSize to 10

![Line Charts](./images/lcSample.png?raw=true)

-   Set lcLegend as "labeled"

![Line Charts ToolTip](./images/lcSampleToolTip.png?raw=true)

### Properties

Most properties have default values. However, you can change the values as per your requirement.

For PowerApps Bar Graph all properties are prefixed with "bc"

| Property                 | Description                                                                                                                                                                                     |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| lcAnimateDuration        | Animation Duration (in milli secs)                                                                                                                                                              |
| lcBackGroundColor        | To change the background color of the Graph. Refer Colors section below                                                                                                                         |
| lcBorderType             | Border of the Chart control. Valid values are:<ul><li>lcNone</li><li>lcGraphShadow</li><li>lcGraphNoShadow</li><li>lcGraphRoundedNoShadow</li><li>lcGraphRoundedShadow</li></ul>                |
| lcColors                 | Override the default colors. Based on the data provide custom colors as comma separated values. Refer Colors section for details                                                                |
| lchAxisMinValue          | Change the Horizontal Axis Min Value (default 0)                                                                                                                                                |
| lchAxisTextBold          | Display Horizontal Axis Text in Bold (true or false)                                                                                                                                            |
| lchAxisTextColor         | Change the Horizontal Axis Text color                                                                                                                                                           |
| lchAxisTextFontName      | Set the Font Name of Horizontal Axis Text                                                                                                                                                       |
| lchAxisTextFontSize      | Set the Font Size of Horizontal Axis Text                                                                                                                                                       |
| lchAxisTextFormat        | Change the Horizontal Axis Text format. Valid values are: <br><br><ul><li>lcNone</li><li>lcDecimal</li><li>lcCurrency</li><li>lcShort (Shows 1M instead of 1,000,000)</li></ul>                 |
| lchAxisTextItalic        | Display Horizontal Axis Text to Italic (default false)                                                                                                                                          |
| lchAxisTitle             | Horizontal Axis Title                                                                                                                                                                           |
| lchAxisTitleTextBold     | Set the Horizontal Axis Title to Bold (default true)                                                                                                                                            |
| lchAxisTitleTextColor    | Change the Horizontal Axis Title color                                                                                                                                                          |
| lchAxisTitleTextFontName | Set the Font Name of Horizontal Axis Title                                                                                                                                                      |
| lchAxisTitleTextFontSize | Set the Font Size of Horizontal Axis Title                                                                                                                                                      |
| lchAxisTitleTextItalic   | Display Horizontal Axis Title to Italic (default false)                                                                                                                                         |
| lcLegend                 | Show the Legend by setting one of the values: <ul><li>lcNone (to remove Legend) </li><li>lcLabeled</li><li>lcRight</li><li>lcBottom</li><li>lcTop</li></ul>                                     |
| lcLegendTextBold         | Set the Legend Text to Bold (default false)                                                                                                                                                     |
| lcLegendTextColor        | Change the Legend Text color                                                                                                                                                                    |
| lcLegendTextFontName     | Set the Font Name of Legend Text                                                                                                                                                                |
| lcLegendTextFontSize     | Set the Font Size of Legend Text                                                                                                                                                                |
| lcLegendTextItalic       | Display Legend Text to Italic (default false)                                                                                                                                                   |
| lcLegendWidth            | Increase (positive value) or decrease (negative value) the Legend Width                                                                                                                         |
| lcLineType               | Display Line in straight line or curve. <ul><li>lgNone - Straight line</li><li>lgCurve - for curved lines</li></ul>                                                                             |
| lcOrientation            | Orientation of Graph <ul><li>Vertical - bcVertical</li><li>Horizontal - bcHorizontal</li></ul>                                                                                                  |
| lcPointShape             | Display the following shape at the plotted points. <ul><li>lcPointShape</li><li>lcCircle</li><li>lcTriangle</li><li>lcSquare</li><li>lcDiamond</li><li>lcStar</li><li>lcPolygon</li></ul>       |
| lcPointSize              | Size of the shape defined in lgPointShape                                                                                                                                                       |
| lcSubTitle               | Set Sub Title of the Graph                                                                                                                                                                      |
| lcSubTitleTextColor      | Change the Sub Title Text color                                                                                                                                                                 |
| lcSubTitleTextFontName   | Set the Font Name of Sub Title Text                                                                                                                                                             |
| lcSubTitleTextFontSize   | Set the Font Size of Sub Title Text                                                                                                                                                             |
| lcSubTitleTextFontStyle  | Set the Sub Title Text to either: <ul><li>lcNormal</li><li>lcOblique</li><li>lcItalic</li></ul>                                                                                                 |
| lcSubTitleTextFontWeight | Set the Sub Title Text to either: <ul><li>lcNormal</li><li>lcLight</li><li>lcLighter</li><li>lcBold</li><li>lcBolder</li></ul>                                                                  |
| lcTitle                  | Set Title of the Graph                                                                                                                                                                          |
| lcTitleTextColor         | Change the Title Text color                                                                                                                                                                     |
| lcTitleTextFontName      | Set the Font Name of Title Text                                                                                                                                                                 |
| lcTitleTextFontSize      | Set the Font Size of Title Text                                                                                                                                                                 |
| lcTitleTextFontStyle     | Set the Title Text to either: <ul><li>lcNormal</li><li>lcOblique</li><li>lcItalic</li></ul>                                                                                                     |
| lcTitleTextFontWeight    | Set the Title Text to either: <ul><li>lcNormal</li><li>lcLight</li><li>lcLighter</li><li>lcBold</li><li>lcBolder</li></ul>                                                                      |
| lcTransposeData          | Transpose the provide data                                                                                                                                                                      |
| lcvAxisTextBold          | Set the Vertical Axis Text to Bold (default false)                                                                                                                                              |
| lcvAxisTextColor         | Change the Vertical Axis Text color                                                                                                                                                             |
| lcvAxisTextFontName      | Set the Font Name of Vertical Axis Text                                                                                                                                                         |
| lcvAxisTextFontSize      | Set the Font Size of Vertical Axis Text                                                                                                                                                         |
| lcvAxisTextFormat        | Change the Vertical Axis Text format. Valid values are: <br><br><ul><li>lcNone</li><li>lcDecimal</li><li>lcCurrency</li><li>lcShort (Shows 1M instead of 1,000,000)</li></ul>                   |
| lcvAxisTextItalic        | Display Vertical Axis Text to Italic (default false)                                                                                                                                            |
| lcvAxisTitle             | Vertical Axis Title                                                                                                                                                                             |
| lcvAxisTitleTextBold     | Set the Vertical Axis Title to Bold (default true)                                                                                                                                              |
| lcvAxisTitleTextColor    | Change the Vertical Axis Title color                                                                                                                                                            |
| lcvAxisTitleTextFontName | Set the Font Name of Vertical Axis Title                                                                                                                                                        |
| lcvAxisTitleTextFontSize | Set the Font Size of Vertical Axis Title                                                                                                                                                        |
| lcvAxisTitleTextItalic   | Display Vertical Axis Title to Italic (default false)                                                                                                                                           |
| lcEnableConsoleLog       | Set to true to enable log in Console                                                                                                                                                            |
| lcEnableGraphClick       | Set to true to enable Click event within graph. On click the graph returns values which can be accessed through the below properties: <ul><li>lcSelectedData1</li><li>lcSelectedData2</li></ul> |
| lcSelectedData1          | Get X axis value (on click)                                                                                                                                                                     |
| lcSelectedData2          | Get Y axis value (on click)                                                                                                                                                                     |
| lcDataCollection         | Set the data collection to display graph                                                                                                                                                        |

### **Colors**

You can provide colors in either formats:<ul><li><b>#ff0000, #00ff00, #0000ff</b></li><li><b>red, green, blue</b></li></ul>
