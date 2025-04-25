# crosswalk values if "found"
* Find value in B2 somewhere in Column I
  * =IF(COUNTIF($I:$I, $B2), "Found", "Not Found")
* Find value in B2 somewhere in Column I, if "Found" Crosswalk it to the same row value of Column J
  * =IF(COUNTIF($I:$I, $B2), INDEX($J:$J, MATCH($B2, $I:$I, 0)), "Not Found")
