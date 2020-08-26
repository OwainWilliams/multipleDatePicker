# Multiple Date Picker for Umbraco 8

Multiple Date Picker is a ported version of https://github.com/markwemekamp/Umbraco-Multiple-Date-Picker package for Umbraco 7.

## Installation

Either log in to the backoffice of Umbraco and search the package library or you can now install this via nuget.

`Install-Package oc.MultipleDatePicker`


## Usage

* Log in to the backoffice of Umbraco 8
* ![Demo of how to setup the Multiple Date Picker](https://github.com/OwainWilliams/multipleDatePicker/blob/master/MultipleDatePicker8/assets/CreatePicker.gif)

##Within the frontend view: 

Once you have your data type added to your Document Type, you can get the dates in your view like this : 
```
@{
    foreach (var date in Model.Dates)
    {
        DateTime formatDate = (DateTime)date;
        <b>@formatDate.ToString("dd-MM-yyyy")</b>
    }
} 
```

Dates is the alias that I gave my property in the document type, if you called it something like Date Picker, then your alias would be Model.DatePicker.
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
