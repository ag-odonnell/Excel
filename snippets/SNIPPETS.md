
# Use the following to convert a numeric value in one cell to a formatted part of a string in another cell.
* =A2&"- delta: (d="&TEXT(D2,"#,##0")&")"

# Find new/old values 2 different lists
* count
  * =IF(ROW(B2)=2,1,IF(C2=C1,D1+1,1))
* flag_gt_2
  * =IF(D2>2,1,0)
* flag_new_derive
  * =IF(D1=1,IF(D2=1,1,0),0)
* flag_new_static
