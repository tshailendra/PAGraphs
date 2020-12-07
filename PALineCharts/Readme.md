# PowerApps LineCharts

Provides a better graphs for Power App Canvas Apps using [PALineCharts.zip](https://github.com/)

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
    -   Select **LineChart**
    -   Insert Bar Chart from code components
    -   set the Items property to a collection
    -   In the properties tab add fields
    -   Select the fields based on the Chart Type
    -

### Sample Chart

**to do**

### Properties

Most properties have default values. However, you can change the values as per your requirement.

For PowerApps Bar Graph all properties are prefixed with "bc"

| Property                 | Description                                                                                                                                                                                     |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| lgAnimateDuration        | Animation Duration (in milli secs)                                                                                                                                                              |
| lgBackGroundColor        | To change the background color of the Graph. Refer Colors section below                                                                                                                         |
| lgBorderType             | Border of the Chart control. Valid values are:<ul><li>bcNone</li><li>bcGraphShadow</li><li>bcGraphNoShadow</li><li>bcGraphRoundedNoShadow</li><li>bcGraphRoundedShadow</li></ul>                |
| lgColors                 | Override the default colors. Based on the data provide custom colors as comma separated values. Refer Colors section for details                                                                |
| lghAxisMinValue          | Change the Horizontal Axis Min Value (default 0)                                                                                                                                                |
| lghAxisTextBold          | Display Horizontal Axis Text in Bold (true or false)                                                                                                                                            |
| lghAxisTextColor         | Change the Horizontal Axis Text color                                                                                                                                                           |
| lghAxisTextFontName      | Set the Font Name of Horizontal Axis Text                                                                                                                                                       |
| lghAxisTextFontSize      | Set the Font Size of Horizontal Axis Text                                                                                                                                                       |
| lghAxisTextFormat        | Change the Horizontal Axis Text format. Valid values are: <br><br><ul><li>bcNone</li><li>bcDecimal</li><li>bcCurrency</li><li>bcShort (Shows 1M instead of 1,000,000)</li></ul>                 |
| lghAxisTextItalic        | Display Horizontal Axis Text to Italic (default false)                                                                                                                                          |
| lghAxisTitle             | Horizontal Axis Title                                                                                                                                                                           |
| lghAxisTitleTextBold     | Set the Horizontal Axis Title to Bold (default true)                                                                                                                                            |
| lghAxisTitleTextColor    | Change the Horizontal Axis Title color                                                                                                                                                          |
| lghAxisTitleTextFontName | Set the Font Name of Horizontal Axis Title                                                                                                                                                      |
| lghAxisTitleTextFontSize | Set the Font Size of Horizontal Axis Title                                                                                                                                                      |
| lghAxisTitleTextItalic   | Display Horizontal Axis Title to Italic (default false)                                                                                                                                         |
| lgLegend                 | Show the Legend by setting one of the values: <ul><li>bcNone (to remove Legend) </li><li>bcLabeled</li><li>bcRight</li><li>bcBottom</li><li>bcTop</li></ul>                                     |
| lgLegendTextBold         | Set the Legend Text to Bold (default false)                                                                                                                                                     |
| lgLegendTextColor        | Change the Legend Text color                                                                                                                                                                    |
| lgLegendTextFontName     | Set the Font Name of Legend Text                                                                                                                                                                |
| lgLegendTextFontSize     | Set the Font Size of Legend Text                                                                                                                                                                |
| lgLegendTextItalic       | Display Legend Text to Italic (default false)                                                                                                                                                   |
| lgLegendWidth            | Increase (positive value) or decrease (negative value) the Legend Width                                                                                                                         |
| lgLineType               | Display Line in straight line or curve. <ul><li>lgNone - Straight line</li><li>lgCurve - for curved lines</li></ul>                                                                             |
| lgOrientation            | Orientation of Graph <ul><li>Vertical - bcVertical</li><li>Horizontal - bcHorizontal</li></ul>                                                                                                  |
| lgPointShape             | Display the following shape at the plotted points. <ul><li>lgPointShape</li><li>lgCircle</li><li>lgTriangle</li><li>lgSquare</li><li>lgDiamond</li><li>lgStar</li><li>lgPolygon</li></ul>       |
| lgPointSize              | Size of the shape defined in lgPointShape                                                                                                                                                       |
| lgSubTitle               | Set Sub Title of the Graph                                                                                                                                                                      |
| lgSubTitleTextColor      | Change the Sub Title Text color                                                                                                                                                                 |
| lgSubTitleTextFontName   | Set the Font Name of Sub Title Text                                                                                                                                                             |
| lgSubTitleTextFontSize   | Set the Font Size of Sub Title Text                                                                                                                                                             |
| lgSubTitleTextFontStyle  | Set the Sub Title Text to either: <ul><li>bcNormal</li><li>bcOblique</li><li>bcItalic</li></ul>                                                                                                 |
| lgSubTitleTextFontWeight | Set the Sub Title Text to either: <ul><li>bcNormal</li><li>bcLight</li><li>bcLighter</li><li>bcBold</li><li>bcBolder</li></ul>                                                                  |
| lgTitle                  | Set Title of the Graph                                                                                                                                                                          |
| lgTitleTextColor         | Change the Title Text color                                                                                                                                                                     |
| lgTitleTextFontName      | Set the Font Name of Title Text                                                                                                                                                                 |
| lgTitleTextFontSize      | Set the Font Size of Title Text                                                                                                                                                                 |
| lgTitleTextFontStyle     | Set the Title Text to either: <ul><li>bcNormal</li><li>bcOblique</li><li>bcItalic</li></ul>                                                                                                     |
| lgTitleTextFontWeight    | Set the Title Text to either: <ul><li>bcNormal</li><li>bcLight</li><li>bcLighter</li><li>bcBold</li><li>bcBolder</li></ul>                                                                      |
| lgTransposeData          | Transpose the provide data                                                                                                                                                                      |
| lgvAxisTextBold          | Set the Vertical Axis Text to Bold (default false)                                                                                                                                              |
| lgvAxisTextColor         | Change the Vertical Axis Text color                                                                                                                                                             |
| lgvAxisTextFontName      | Set the Font Name of Vertical Axis Text                                                                                                                                                         |
| lgvAxisTextFontSize      | Set the Font Size of Vertical Axis Text                                                                                                                                                         |
| lgvAxisTextFormat        | Change the Vertical Axis Text format. Valid values are: <br><br><ul><li>bcNone</li><li>bcDecimal</li><li>bcCurrency</li><li>bcShort (Shows 1M instead of 1,000,000)</li></ul>                   |
| lgvAxisTextItalic        | Display Vertical Axis Text to Italic (default false)                                                                                                                                            |
| lgvAxisTitle             | Vertical Axis Title                                                                                                                                                                             |
| lgvAxisTitleTextBold     | Set the Vertical Axis Title to Bold (default true)                                                                                                                                              |
| lgvAxisTitleTextColor    | Change the Vertical Axis Title color                                                                                                                                                            |
| lgvAxisTitleTextFontName | Set the Font Name of Vertical Axis Title                                                                                                                                                        |
| lgvAxisTitleTextFontSize | Set the Font Size of Vertical Axis Title                                                                                                                                                        |
| lgvAxisTitleTextItalic   | Display Vertical Axis Title to Italic (default false)                                                                                                                                           |
| lgEnableConsoleLog       | Set to true to enable log in Console                                                                                                                                                            |
| lgEnableGraphClick       | Set to true to enable Click event within graph. On click the graph returns values which can be accessed through the below properties: <ul><li>bcSelectedData1</li><li>bcSelectedData2</li></ul> |
| lgSelectedData1          | Get X axis value (on click)                                                                                                                                                                     |
| lgSelectedData2          | Get Y axis value (on click)                                                                                                                                                                     |
| lgDataCollection         | Set the data collection to display graph                                                                                                                                                        |

### **Colors**

You can provide colors in either formats:<ul><li><b>#ff0000, #00ff00, #0000ff</b></li><li><b>red, green, blue</b></li></ul>
