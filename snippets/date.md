# Derive DATE from a STRING
* =IF(NOT(ISBLANK(A2)),DATE(LEFT(A2,4),MID(A2, 5, 2),MID(A2, 7, 2)),"")
