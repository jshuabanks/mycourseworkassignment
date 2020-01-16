# D3 Visulisation Programming Coursework 

This project is a reusable D3 data visulisation using Javascript. The visulisation was made using a class so that when the user calls it they can create their own version of the visulisation.

This project is about taking some existing code and turning it into a reusable element using Javascript classes.

## Sources

In this project, I have made a reference to existing code which I have then used.

Source of Code:  
Author - Lokesh Todwal  
Date - 21st February, 2018  
Title - Platelets  
URL - http://bl.ocks.org/lokesh005/1b23c84b68f5be134ff0  
License - No License  

Source of Dataset:  
Author - World Bank  
Date - 2018  
Title - GDP (current US$)  
URL - https://data.worldbank.org/indicator/NY.GDP.MKTP.CD?end=2018&start=2018&view=map  http://api.worldbank.org/v2/en/indicator/NY.GDP.MKTP.CD?downloadformat=csv  
License - CC BY-4.0


## Installation

No official installation is required to use this project.  

In order to view this project, please download the ZIP file and unpackage it.  
Then double click on the index.html file to open it.  
The index.html file is the only file that you will need to open in order to view the visulisation.  
```file
index.html
```
There is also a script.js file and a style.css file. These do not need to be opened by the user but please feel free to open them to view any of the code.

Also within the folder is another folder titled JSDOC which contains all of the documentation you will need to understand the code.


## Usage
To create a new visulisation with new parameters using the class that I have created you will need to use some code similar to my example below. This is the default code that comes in the index.html file.

In order to change the dataset please alter the URL which is in the d3.csv function below. Be aware that the dataset must fit the format of the CSV in order to work. The data is then passed to the class through the parameter data.
To change anything else please alter the other parameters.

```javascript
d3.csv('https://raw.githubusercontent.com/dwvf58/mycourseworkassignment/master/Current%20Version/top50gdpinworld.csv', (data) => {
      var chart = new Chart(40, 300, 300, data, 0.0, 'Country: ', 'GDP of Country: $');
```
Please see below in the constructor for the order of what the parameters must be and what they will default to if left blank.
```javascript
constructor (margin = 40, width = 300, height = 300, data, spacing = 0.0, keydescriptiontext = 'Country: ', valuedescriptiontext = 'GDP of Country: $')
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)