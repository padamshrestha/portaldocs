
<a name="extension-controls"></a>
# Extension Controls

<!--  required section -->


<a name="extension-controls-overview"></a>
## Overview

Controls are the building blocks of the Azure extension experience. They allow users to view, edit, and analyze data.

The Azure Portal team ships sample code that extension developers can leverage. All developers who install the Portal Framework SDK that is located at [http://aka.ms/portalfx/download](http://aka.ms/portalfx/download) also install the samples on their computers during the installation process. The source for the samples is located in the `Documents\PortalSDK\FrameworkPortal\Extensions\SamplesExtension` folder.

First-party extension developers, i.e. Microsoft employees, have access to the Dogfood environment, therefore they can view the samples that are located at [https://aka.ms/portalfx/viewSamples](https://aka.ms/portalfx/viewSamples).

The Azure components of the experience are documented several ways. 
*  There may be a document that provides guidance about the component, in terms of what it is, what it does, or how it is used. 
* The location of the sample code is included  so that the developer can view the source for the component, or modify it as appropriate for the extensions they develop.  
* A completed version of the component can be viewed in the Dogfood environment; in some instances, links are provided to the API reference for the component.

**NOTE**: In the following tables, `<dir>` is the `SamplesExtension\Extension\` directory, and  `<dirParent>`  is the `SamplesExtension\` directory, based on where the samples were installed when the developer set up the SDK. If there is a working copy of the sample in the Dogfood environment, it can be experienced by using the link in the table.

The following tables include information about Portal controls, including the location of samples that are shipped with the SDK and working copies in the Dogfood environment.

<a name="extension-controls-controls-that-are-used-by-other-controls"></a>
## Controls that are used by other controls

<!-- TODO:  Determine whether there are samples and experiences that do not need to be documented in separate documents.  If so, determine whether it is appropriate for them to be combined into the following separate table.-->

| Control        | Sample | Experience |
| -------------- | --------- | -------------- |
| Copyable Label | `<dir>\Client\V2\Controls\ CopyableLabel\CopyableLabelBlade.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/CopyableLabelBlade |

<a name="extension-controls-basic-screen-controls"></a>
## Basic Screen Controls

| Control |  Document | Sample | Experience |
| ------- | -------- | ------ | ---------- |
| Button  | | |  http://aka.ms/portalfx/samples#blade/SamplesExtension/SimpleButtonBlade |
| File Download Button |  | `<dir>\Client\V1\Controls\FileDownloadButton\ViewModels\ FileDownloadButtonViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/FileDownloadButtonInstructions/selectedItem/FileDownloadButtonInstructions/selectedValue/FileDownloadButtonInstructions |  
| File Upload (async) |  | `<dir>\Client\V1\Controls\AsyncFileUpload\ViewModels\ AsyncFileUploadViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/AsyncFileUploadInstructions/selectedItem/AsyncFileUploadInstructions/selectedValue/AsyncFileUploadInstructions |
| Markdown Control | |`<dir>\Client\V1\Controls\Markdown\ViewModels\ MarkdownViewModels.ts`| http://aka.ms/portalfx/samples#blade/SamplesExtension/MarkdownInstructions/selectedItem/MarkdownInstructions/selectedValue/MarkdownInstructions |
| OAuth Button  | | `<dir>\Client\V2\Controls\ OAuthButton\OAuthButtonBlade.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/OAuthButtonBlade | 
| Settings | | `<dir>\Client\V1\Controls\Settings\ViewModels\ SettingsViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/SettingsInstructions/selectedItem/SettingsInstructions/selectedValue/SettingsInstructions | 
| Single Setting |   | `<dir>\Client\V1\Controls\SingleSetting\ViewModels\ SingleSettingViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/SingleSettingInstructions/selectedItem/SingleSettingInstructions/selectedValue/SingleSettingInstructions | 
| Splitter | | `<dir>\Client\V2\Controls\ Splitter\SplitterBlade.ts` |  http://aka.ms/portalfx/samples#blade/SamplesExtension/SplitterBlade | 
| Text Block  |  | `<dir>\Client\V1\Controls\TextBlock\ViewModels\ TextBlockViewModels.ts` | https://df.onecloud.azure-test.net/?samplesExtension=true#blade/SamplesExtension/TextBlockInstructions/selectedItem/TextBlockInstructions/selectedValue/TextBlockInstructions | 
| Text Box |  [portalfx-controls-textbox.md](portalfx-controls-textbox.md)  | `<dir>\Client\V2\Controls\TextBox\TextBoxBlade.ts` | [http://aka.ms/portalfx/samples#blade/SamplesExtension/Textboxblade](http://aka.ms/portalfx/samples#blade/SamplesExtension/Textboxblade) | 
| Toolbar   | [portalfx-controls-toolbar.md](portalfx-controls-toolbar.md)  |  `<dir>\Client\V1\Controls\Toolbar\ViewModels\ ToolbarViewModels.ts` | (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/ToolbarInstructions/selectedItem/ToolbarInstructions/selectedValue/ToolbarInstructions |

<a name="extension-controls-date-and-time"></a>
## Date and Time

| Date/time Object | Document | Sample | Experience |
| ---------------- | -------- | ------ | ---------- |
| Essentials Control | [portalfx-controls-essentials.md](portalfx-controls-essentials.md)  |   `<dir>\Client\V2\Controls\ Essentials/EssentialsDefaultBlade.ts`  |     |
|  Date Picker  |  | `<dir>\Client\V2\Controls\ DatePicker\DatePickerBlade.ts` |   (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/DatePickerInstructions/selectedItem/DatePickerInstructions/selectedValue/DatePickerInstructions |
| Date/Time Picker   |  [portalfx-controls-datetimepicker.md](portalfx-controls-datetimepicker.md)  |  `<dir>\Client\V2\Controls\ DateTimePicker\DateTimePickerBlade.ts`   | (experience does not work) <br>  http://aka.ms/portalfx/samples#blade/SamplesExtension/DateTimePickerInstructions/selectedItem/DateTimePickerInstructions/selectedValue/DateTimePickerInstructions |
| Date/Time Range Picker  | [portalfx-controls-datetimerangepicker.md](portalfx-controls-datetimerangepicker.md)  |   `<dir>\Client\V2\Controls\ DateTimeRangePicker\DateTimeRangePickerBlade.ts` | (experience does not work) <br>  http://aka.ms/portalfx/samples#blade/SamplesExtension/DateTimeRangePickerInstructions/selectedItem/DateTimeRangePickerInstructions/selectedValue/DateTimeRangePickerInstructions |
| Date Polyfills |  | `<dir>\Client\V1\Controls\DatePolyFills\ViewModels\ DatePolyFillsViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/DatePolyFillsInstructions/selectedItem/DatePolyFillsInstructions/selectedValue/DatePolyFillsInstructions |
| Day Picker (does not work) |  | `<dir>\Client\V2\Controls\ DayPicker\DayPickerBlade.ts`   |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/DayPickerInstructions/selectedItem/DayPickerInstructions/selectedValue/DayPickerInstructions |
| Duration Picker |  | `<dir>\Client\V1\Controls\DurationPicker\ViewModels\ DurationPickerViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/DurationPickerInstructions/selectedItem/DurationPickerInstructions/selectedValue/DurationPickerInstructions |
| Time Picker |  | `<dir>\Client\V1\Controls\TimePicker\ViewModels\ TimePickerViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/TimePickerInstructions/selectedItem/TimePickerInstructions/selectedValue/TimePickerInstructions |

<a name="extension-controls-drop-downs"></a>
## Drop downs

| Drop Down | Document | Sample | Experience |
| --------- | -------- | ------ | ---------- |
| Drop Down | [portalfx-controls-dropdown.md](portalfx-controls-dropdown.md) | `<dir>\Client\V2\Controls\ DropDown\DropDownBlade.ts` | |
| Console   | [portalfx-controls-console.md](portalfx-controls-console.md) | `<dir>\Client\V2\Controls\ Console\ConsoleBlade.ts` | |

<a name="extension-controls-editors"></a>
## Editors

| Editor      | Document | Sample | Experience |
| ----------- | -------- | ------ | ---------- |
| Code editor | [portalfx-controls-editor.md](portalfx-controls-editor.md) | | 
| Diff editor |  |  |http://aka.ms/portalfx/samples#blade/SamplesExtension/DiffEditorInstructions/selectedItem/DiffEditorInstructions/selectedValue/DiffEditorInstructions | 

<a name="extension-controls-forms"></a>
## Forms

| Forms | Document | Sample | Experience |
| --------- | -------- | ------ | ---------- |
| Standard Check Box  |   |   |  (experience does not work) <br>  http://aka.ms/portalfx/samples#blade/SamplesExtension/CheckBoxInstruction |
| Tri State Check Box  |   |   |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/TriStateCheckBoxInstructions  |
| Custom HTML |   |   | http://aka.ms/portalfx/samples#blade/SamplesExtension/CustomFormFieldsBlade  |
| MultiLine Text Box  |   |   |  (experience does not work) <br>  http://aka.ms/portalfx/samples#blade/SamplesExtension/MultiLineTextBoxInstructions/selectedItem/MultiLineTextBoxInstructions/selectedValue/MultiLineTextBoxInstructions |
| Numeric Text Box  |   |   |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/NumericTextBoxInstructions/selectedItem/NumericTextBoxInstructions/selectedValue/NumericTextBoxInstructions  |
| Text Box  |   |   |   (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/TextBoxInstructions/selectedItem/TextBoxInstructions/selectedValue/TextBoxInstructions |
| Option Picker  |   |   |   (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/OptionPickerInstructions/selectedItem/OptionPickerInstructions/selectedValue/OptionPickerInstructions |
| Password Box   |   |   |   (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/PasswordInstructions/selectedItem/PasswordInstructions/selectedValue/PasswordInstructions |
| Search Box |   |   |  http://aka.ms/portalfx/samples#blade/SamplesExtension/SearchBoxBlade/selectedItem/SearchBoxBlade/selectedValue/SearchBoxBlade |
| Standard Slider |   |   |   (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/SliderInstructions/selectedItem/SliderInstructions/selectedValue/SliderInstructions |
| Custom Value Slider |   |   |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/SlidersInstructions/selectedItem/SlidersInstructions/selectedValue/SlidersInstructions |
| Range Slider |   |   |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/RangeSliderInstructions/selectedItem/RangeSliderInstructions/selectedValue/RangeSliderInstructions  |
| Custom Range Slider |   |   |   (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/RangeSliderInstructions/selectedItem/CustomRangeSliderInstructions/selectedValue/CustomRangeSliderInstructions  |

<a name="extension-controls-lists"></a>
## Lists

| Gallery | Document | Sample | Experience |
| ------- | -------- | ------ | ---------- |
| Gallery | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/GalleryInstructions/selectedItem/GalleryInstructions/selectedValue/GalleryInstructions |
| List View | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/ListViewInstructions/selectedItem/ListViewInstructions/selectedValue/ListViewInstructions
| Tree View | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/TreeViewInstructions/selectedItem/TreeViewInstructions/selectedValue/TreeViewInstructions
| String List | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/StringListInstructions/selectedItem/StringListInstructions/selectedValue/StringListInstructions
| Query Builder | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/QueryBuilderInstructions/selectedItem/QueryBuilderInstructions/selectedValue/QueryBuilderInstructions
| Grid |  [portalfx-controls-grid.md](portalfx-controls-grid.md) | | | 

<a name="extension-controls-helpers-and-indicators"></a>
## Helpers and Indicators

| Helpers | Document | Sample | Experience |
| ------- | -------- | ------ | ---------- |
| Docked Balloon | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/DockedBalloonInstructions/selectedItem/DockedBalloonInstructions/selectedValue/DockedBalloonInstructions | 
| Info Box | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/InfoBoxInstructions/selectedItem/InfoBoxInstructions/selectedValue/InfoBoxInstructions |
| Progress Bar | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/ProgressBarInstructions/selectedItem/ProgressBarInstructions/selectedValue/ProgressBarInstructions |

<a name="extension-controls-data-visualization-objects"></a>
## Data Visualization Objects

| Screen Objects  | Document | Sample | Experience |
| ------------- | -------- | ------ | ---------- |
| | | Aggregates  | |
| Chart         | [portalfx-controls-chart.md](portalfx-controls-chart.md) | | |
| Monitor Chart | [portalfx-controls-monitor-chart.md](portalfx-controls-monitor-chart.md) | | |
| Donut         | [portalfx-controls-donut.md](portalfx-controls-donut.md) | `<dir>\Client\V2\Controls\Donut\DonutBlade.ts`  | |
|       | |  Gauges | |
| Quota Gauge   | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/QuotaGaugeBlade |
| Single Value Gauge | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/SingleValueGaugeBlade |
| Step Gauge | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/StepGaugeBlade |
| | | Graphs   | | |
| Standard Graph  | [portalfx-controls-graph-nuget.md](portalfx-controls-graph-nuget.md)| | http://aka.ms/portalfx/samples#blade/SamplesExtension/graphInstructions |
| Custom Html Nodes | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/graphCustomNodeInstructions
| Metrics | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/MetricsInstructions/selectedItem/MetricsInstructions/selectedValue/MetricsInstructions | 
| | | Maps  | |
| Base Map | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/BaseMapInstructions |
| Hexagon Layout Map | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/HexagonMapInstructions |
| Menu | | |http://aka.ms/portalfx/samples#blade/SamplesExtension/MenuInstructions/selectedItem/MenuInstructions/selectedValue/MenuInstructions |
| Log Stream | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/LogStreamInstructions/selectedItem/LogStreamInstructions/selectedValue/LogStreamInstructions |
| Spec Comparison Table | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/SpecComparisonTableInstructions/selectedItem/SpecComparisonTableInstructions/selectedValue/SpecComparisonTableInstructions |
| Video Control | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/VideoInstructions/selectedItem/VideoInstructions/selectedValue/VideoInstructions |
| Legend | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/Legend/selectedItem/Legend/selectedValue/Legend  | 
| HotSpot | | | http://aka.ms/portalfx/samples#blade/SamplesExtension/HotSpotInstructions/selectedItem/HotSpotInstructions/selectedValue/HotSpotInstructions |
| Video | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/VideoInstructions/selectedItem/VideoInstructions/selectedValue/VideoInstructions |
| Terminal Emulator | | |  (experience does not work) <br> http://aka.ms/portalfx/samples#blade/SamplesExtension/TerminalEmulatorInstructionsBlade/selectedItem/TerminalEmulatorInstructionsBlade/selectedValue/TerminalEmulatorInstructionsBlade |

<a name="extension-controls-deprecated-controls"></a>
## Deprecated controls

The following controls have been deprecated.  They have been replaced with more performant controls, or  with best practices that reduce issues in usability testing and improve the Create success rate. However, they are included in the following list for backward compatibility.

| Control  | Document | Sample | Experience |
| -------- | -------- | ------ | ---------- |
| Selector |  |  `<dir>\Client\V1\Controls\Selector\ViewModels\ SelectorViewModels.ts` | http://aka.ms/portalfx/samples#blade/SamplesExtension/SelectorInstructions/selectedItem/SelectorInstructions/selectedValue/SelectorInstructions | 




<a name="extension-controls-faqs-for-extension-controls"></a>
## FAQs for Extension Controls


   <!-- TODO:  FAQ Format is ###Link, ***title***, Description, Solution, 3 Asterisks -->

<a name="extension-controls-faqs-for-extension-controls-how-to-use-a-monitorchartpart-from-legacy-blade"></a>
### How to use a MonitorChartPart from Legacy Blade

***My extension is still using legacy blades (locked or unlocked). Is this still applicable to me? If yes, do I get the benefits mentioned above?***

SOLUTION: Even if you are not using template blades, you can reference the MonitorChartPart from the Hubs extension, as specified in [portalfx-controls-monitor-chart.md#legacyBladeUsage](portalfx-controls-monitor-chart.md#legacyBladeUsage).

If there is an Insights/Monitoring Metrics part on your blade already, you can reference the part from Hubs extension instead of referencing the metrics part from Insights/Monitoring extension. Because the Hubs extension is always loaded when you load the portal, it will be loaded before the user loads your extension blade. Hence, you will not load an additional extension and get significant performance benefits. However, for the best performance, we strongly recommend that your extension should use the [Monitor Chart control](#the-monitor-chart control) directly on a template blade. For more information about migrating to template blades, see []().

* * * 

<a name="extension-controls-faqs-for-extension-controls-changing-the-metrics-time-range-chart-type"></a>
### Changing the metrics/time range/chart type

***Can the users change the metrics/time range/chart type of the charts shown in the overview blade?***

SOLUTION: No, users cannot customize what is displayed in the overview blade. For customizations, users can click on the chart, navigate to Azure Monitor, make changes the chart if needed, and then pin it to the dashboard. The dashboard contains all the charts that users want to customize and view.

This means the extension has a consistent story.
1. View the metrics in overview blade
1. Explore the metrics in Azure Monitor
1. Track and monitor metrics in the Azure Dashboard

Removing customizations from blades also provides more reliable blade performance.

    
* * * 
    
<a name="extension-controls-glossary"></a>
## Glossary

This section contains a glossary of terms and acronyms that are used in this document. For common computing terms, see [https://techterms.com/](https://techterms.com/). For common acronyms, see [https://www.acronymfinder.com](https://www.acronymfinder.com).
 
| Term             | Meaning |
| ---              | --- |
| big data | Data sets that are  very large or very diverse,  including  structured, semi-structured and unstructured datathat may be located in  different sources. The variation in sizes or types of data stores is beyond the ability of traditional databases to capture, manage, and process the data with low-latency.  | 
| IANA | Internet Assigned Numbers Authority | 
| timezone         | The local time of a region or a country, based on factors like time zone maps and Daylight Savings Time. | 
| timezone offset  | The difference, in minutes, between UTC time and the current time in the current locale.|
| UTC              | Universal Coordinated Time  |
