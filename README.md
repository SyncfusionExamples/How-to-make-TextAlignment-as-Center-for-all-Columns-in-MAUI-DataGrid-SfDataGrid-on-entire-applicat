# How-to-make-TextAlignment-as-Center-for-all-Columns-in-MAUI-DataGrid-SfDataGrid-on-entire-applicat

The .NET [MAUI DataGrid](https://www.syncfusion.com/maui-controls/maui-datagrid)(SfDataGrid) allows to set the TextAlignment as Center for all columns in DataGrid on entire application through the implicit style as shown in the below code snippets.

## XAML
Step 1 : Write the implicit style for [DataGridCell](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.DataGridCell.html) and [DataGridHeaderCell](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.DataGridHeaderCell.html) with TextAlignment property value as Center in App.Xaml.

```XML
<Application xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             xmlns:local="clr-namespace:DataGridMAUI"
             xmlns:syncfusion="clr-namespace:Syncfusion.Maui.DataGrid;assembly=Syncfusion.Maui.DataGrid"
             x:Class="DataGridMAUI.App">
    <Application.Resources>
        <ResourceDictionary>
            <Style TargetType="syncfusion:DataGridCell">
                <Setter Property="TextAlignment" Value="Center"></Setter>
            </Style>
            <Style TargetType="syncfusion:DataGridHeaderCell">
                <Setter Property="TextAlignment" Value="Center"></Setter>
            </Style>
        </ResourceDictionary>
    </Application.Resources>
</Application>
```

![TextAlignment](TextAlignmentAsCenter.png)

