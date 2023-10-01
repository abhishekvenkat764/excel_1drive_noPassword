<h1>excel_1drive_noPassword</h1>   
_____________________________________________  

The package is immensely useful for data analysts and scientsits who work with files placed in Excel Onedrive files.

This package can be used to directly import all the sheets and their data in an excel file placed in the Onedrive without the need for username or password in a hssle free manner.

The excel file in the Onedrive should be configured to be accessible by anyone with a valid url.


_____________________________________________

<h2>Instructions.</h2>  

To install the package, perform:  

```python
pip install excel_1drive_noPassword
```
 
How to use the methods:  

<h3>1. To extract the entire excel sheet as a Dictionary where the keys are the sheet names and the values are the dataframes:  </h3>

```python
#Importing Library.
import excel_1drive_noPassword as odrxl

#The url of the excel file in the onedrive.
url = "https://1drv.ms/x/s!ApzxvrDY1mm1gTt1N0uvVwITl91i?e=z7YP4T"

data_dict = odrxl.excel_1drive_toDict(url)

```

<h3>2. To extract the sheetnames of the excel file.  </h3>

```python
#Importing Library.
import excel_1drive_noPassword as odrxl

#The url of the excel file in the onedrive.
url = "https://1drv.ms/x/s!ApzxvrDY1mm1gTt1N0uvVwITl91i?e=z7YP4T"

sheetnames = odrxl.excel_1drive_sheetnames(url)

print(sheetnames)

```

<h3>3. To extract a single sheet from the excel file as a dataframe.  </h3>

```python
#Importing Library.
import excel_1drive_noPassword as odrxl

#The url of the excel file in the onedrive.
url = "https://1drv.ms/x/s!ApzxvrDY1mm1gTt1N0uvVwITl91i?e=z7YP4T"

sheetname = "sheet_1"

df_sheet = odrxl.excel_1dr_SingleSheet_toDF(url, sheetname)

```



_____________________________________________

<h3>Have fun. :-) </h3>