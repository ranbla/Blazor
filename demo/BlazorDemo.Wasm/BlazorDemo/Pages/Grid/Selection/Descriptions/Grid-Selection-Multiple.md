The DevExpress Blazor [Grid](https://docs.devexpress.com/Blazor/403143/grid) supports both single and multiple row selection. Enable the [AllowSelectRowByClick](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.AllowSelectRowByClick) option to select rows via mouse clicks.

In this demo, users can select multiple rows simultaneously (the [SelectionMode](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.SelectionMode) property is set to [GridSelectionMode.Multiple](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridSelectionMode)- the default value). To select a range of rows, a user can click the first row in the range, hold down the **Shift** key, and click the last row in the range. To add/remove a row to/from selection, users must hold down the **Ctrl** key and click the appropriate row.

Implement two-way binding for the [SelectedDataItems](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.SelectedDataItems) property to specify and access selected data items. 

The Grid compares and identifies data items to ensure accurate selection operations. If your data object has a primary key, assign it to the [KeyFieldName](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.KeyFieldName) or [KeyFieldNames](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.KeyFieldNames) property. Otherwise, the Grid uses standard [.NET value equality comparison](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/statements-expressions-operators/equality-comparisons) to identify data items.