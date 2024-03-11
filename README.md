## Target the ASP.NET Core SDK with an Excel-DNA add-in.

Excel-DNA v1.80-alpha3 adds the option to apply the project's .runtimeconfig.json file when initializing the .NET 6+ runtime.

```
    <ExcelAddInCustomRuntimeConfiguration>true</ExcelAddInCustomRuntimeConfiguration>
```

### Instructions 
Debug project or load add-in in Excel, then connect from a browser to http://localhost:5144/weatherforecast

### Note
Note that the first add-in targeting .NET 6+ loaded into the Excel process will decide what version of the runtime and SDK is loaded. 

If the loaded version of the runtime or SDK is not compatible with this add-in , the following message will be displayed when loading the conflicting add-in.

![image](https://github.com/govert/TestAspNetAddIn/assets/414659/aea15a4e-2a22-45a3-a2ca-4eee203a92fc)
