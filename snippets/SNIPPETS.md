
# Find new/old values 2 different lists
* count
  * =IF(ROW(B2)=2,1,IF(C2=C1,D1+1,1))
* flag_gt_2
  * =IF(D2>2,1,0)
* flag_new_derive
  * =IF(D1=1,IF(D2=1,1,0),0)
* flag_new_static

