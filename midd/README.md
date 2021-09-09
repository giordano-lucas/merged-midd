#  Information on how to use our Multi-layout Invoice Document Dataset (MIDD) : A Dataset for Named Entity Recognition

######

Inside this folder there are Four Layout Invoices IOB from four different suppliers.
IOB files are transformed into .csv extension so that you can use it readily for model training.

| Layout   |      Number of `.csv` files      | 
|----------|---------------------------------:|
| 1        |  196                             | 
| 2        |   29                             |
| 3        |   14                             |
| 4        |  391                             |

Total : 630 .csv files

The labels used for annotations are:

| Label   |      Full Label      | 
|----------|---------------------------------:|
| `Supp_N`        |  Supplier name                            | 
| `Supp_G`        |  Supplier GST number                             |
| `BUY_N`        |   Buyer Name                             |
| `BUY_G `       |   Buyer GST number                            |
| `INV_NO `      |   Invoice Number  |
| `INV_DT  `     |   Invoice Date  |
| `GT_AMT   `    |   Grand Total Amount  |

These labels are used to denote a string used to show the key fields.
For example (Invoice No: 2778888),so Invoice No is a label with INV_L and its actual value is INV_NO.
Similar for other fields.

`INV_L` for Invoice Number Label, 
`INV_DL` for Invoice Date Label,
`GT_AMTL` for Grand Total Amount Label, 
`GSTL` for GST Label. 

In each `IOB` ,there are two columns:
First Column: Every word or token from invoice.
Second Column: Token's or word's `I` or `O` or `B` tag.




