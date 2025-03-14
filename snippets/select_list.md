# MS Excel: to make a drop down select (in this example)
1) Make a worksheet called "Select"
2) Place the values of the column of the Select worksheet
3) Go to Data -> Validation -> reference the cells of the data to be included in the drop down list.

# MS Excel: IF any cell in current sheet matches the values in the declared "COUNTIF" in the cells of the current sheet
=COUNTIF($E$2:$E$40, A1)>0
=COUNTIF($F$2:$F$40, A1)>0
=COUNTIF($G$2:$G$40, A1)>0
=COUNTIF($H$2:$H$40, A1)>0
=COUNTIF($I$2:$I$40, A1)>0
=COUNTIF($J$2:$J$40, A1)>0
=COUNTIF($K$2:$K$40, A1)>0
=COUNTIF($L$2:$L$40, A1)>0
=COUNTIF($M$2:$M$40, A1)>0
=COUNTIF($N$2:$N$40, A1)>0
=COUNTIF($O$2:$O$40, A1)>0

# MS Excel: IF any cell in current sheet matches the values in the declared "COUNTIF" in the cells of the sheet "Select"
=COUNTIF(Select!$E$2:$E$40, E1)>0
=COUNTIF(Select!$F$2:$F$40, E1)>0
=COUNTIF(Select!$G$2:$G$40, E1)>0
=COUNTIF(Select!$H$2:$H$40, E1)>0
=COUNTIF(Select!$I$2:$I$40, E1)>0
=COUNTIF(Select!$J$2:$J$40, E1)>0
=COUNTIF(Select!$K$2:$K$40, E1)>0
=COUNTIF(Select!$L$2:$L$40, E1)>0
=COUNTIF(Select!$M$2:$M$40, E1)>0
=COUNTIF(Select!$N$2:$N$40, E1)>0
=COUNTIF(Select!$O$2:$O$40, E1)>0
