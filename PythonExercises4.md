# Use of packages in Google with Pypi and Pip in the websites
## Package for working with excel spredsheets for  openpyxl
### Example of using excel spreadshhets with pip install openpyxl
```
import openpyxl as xl
from openpyxl.chart import BarChart, Reference

wb = xl.load_workbook('ListPrices.xlsx')
sheet = wb['Hoja1'] #Ingles is Sheet1
cell = sheet['a1']  # Also use R1C1 Notation
cell = sheet.cell(1, 1)
print(cell.value)
print(sheet.max_row)

for row in range(2, sheet.max_row + 1):
    cell = sheet.cell(row, 3)
    corrected_price = cell.value * 0.9
    corrected_price_cell = sheet.cell(row, 4)
    corrected_price_cell.value = corrected_price

values = Reference(sheet,
                   min_row=2,
                   max_row=sheet.max_row,
                   min_col=4,
                   max_col=4)
chart = BarChart()
chart.add_data(values)
sheet.add_chart(chart, 'e2')

wb.save('transactions2.xlsx')
```
### Example: CharBar module Excel
```
import openpyxl as xl
from openpyxl.chart import BarChart, Reference

def process_workbook(filename):
    wb = xl.load_workbook(filename)
    sheet = wb['Hoja1'] # Ingles is Sheet1

  for row in range(2, sheet.max_row + 1):
    cell = sheet.cell(row, 3)
    corrected_price = cell.value * 0.9
    corrected_price_cell = sheet.cell(row, 4)
    corrected_price_cell.value = corrected_price

 values = Reference(sheet,
                   min_row=2,
                   max_row=sheet.max_row,
                   min_col=4,
                   max_col=4)
 chart = BarChart()
 chart.add_data(values)
 sheet.add_chart(chart, 'e2')
 wb.save('filename')
```







