﻿
# Tachometer Capability Options

## Gauge Axis

## Gauge Axis - Default Settings
Figure 1 below shows the “Gauge Axis” Capability Options. All the values below are set to their defaults. The “Start Value” and “End Value” Options are visible below because there were no Data Fields assigned to the Data Roles “Start Value” and “End Value” when this screenshot was taken. 

Figure 1. Gauge Axis Default settings 

<img src="images/GaugeAxisDefaults.png" alt="Drawing" width="200px">

|Option|Default Value|Description|
|---|---|---|
|Start Angle|-120 degrees|Angle to start the axis. Angles are measured from the vertical up with Positive angles measured clockwise. Note. These is NO restriction for “Start Angle” to be smaller than “End Angle”. The “Start Value” from Data Roles always aligns with Start Angle.|
|End Angle|120 degrees|Angle to emd the axis. Angles are measured from the vertical up with Positive angles measured clockwise. Note. These is NO restriction for “Start Angle” to be smaller than “End Angle”. The “End Value” from Data Roles always aligns with End Angle.|
|Start Value|0|Fixed start value. This will be visible only when there is no Data field assigned for the Data Role “Start Value”.|
|End Value|2X”Value”|Fixed end value. This will be visible only when there is no Data field assigned for the Data Role “End Value”. (i.e from the Data Role “Value”)|
|Scale|Linear|Scale to measure data in the gauge. Supported scales are “Linear” and “Log”.|

## Gauge Axis - Start Value
Figure 2 below shows the same Capability Options as above when a Data Field is assigned for the Data Role “End Value”. Compared with Figure 1, you will notice that “End Value” is not provided as a Customizable Option now. Also, notice that we are using “Start Value” option to set the custom start value of 10000.

| Figure 2. “Gauge Axis” Capability Options when a data field is assigned to Data Role “End Value” | Figure 3. Screenshot of Tachometer with Data and Options from Gauge Axis. |
|---|---|
| <img src="images/GaugeAxisEndValueHidden.png" alt="Drawing" width="200px">  | <img src="images/GaugeAxisSample.png" alt="Drawing" width="300px"> |

## Gauge Axis -  Start Angle and End Angle
Figure 5 below shows the effect of changing the Start Angle to -150 degrees and End Angle to 90 degrees. Tachometer will accept any value for Start Angle and End Angle and render the gauge appropriately.

| Figure 4. “Gauge Axis” Changing Start Angle and End Angle | Figure 5. Effect of changing Start Angle and End Angle |
|---|---|
| <img src="images/GaugeAxisChangeAngles.png" alt="Drawing" width="200px">  | <img src="images/GaugeAxisChangeAnglesSample.png" alt="Drawing" width="300px"> |

## Gauge Axis - Scale
Tachometer supports two types of scales, “Linear” and “Log”. </br>
When Linear Scales are used, data values will be mapped in a linear scale along the axis from Start Angle towards the End Angle.</br>
When Log Scales are used, data values will be mapped in a logarithmic scale along the axis from Start Angle towards the End Angle. Keep in mind that logrithm values are defined only for positive values. What this means is, if you have a negative start or end value, then you are not allowed to select log scale.

Please note that the count of axis labels that will be displayed along the axis can be controlled but in different ways based on the type of Axis Scale you use. If you use Linear Scale, there will be approximately 4 Axis Labels by default. However, you can configure the number of data labels and how they are placed. Please see Examples on [Axis Labels](AxisLabels.md) for more details. 
On the other hand, if you select Log scale, then the number of axis labels will be automatically determined based on the Start Value and End Value defined for the axis. You can limit overcrowding Axis Labels when Log Scale is used with the help of “Reduce” option in Axis Label Capabilities.

Figure 6 Shows the Axis Scale Changed to Log Scale and Figure 7 Shows how it impacts the Tachometer Visual. Compare this with Figure 3 to see the impact.

| Figure 6. Change Axis Scale to Log Scale | Figure 7. Effect of changing Axis Scale to Log Scale |
|---|---|
| <img src="images/GaugeAxisChangeScale.png" alt="Drawing" width="200px">  | <img src="images/GaugeAxisChangeScaleSample.png" alt="Drawing" width="300px"> |
