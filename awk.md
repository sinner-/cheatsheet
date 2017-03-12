# awk Cheatsheet

* Print the nth column of stdin:
  * `awk '{print $n}'`
* Use a non-whitespace delimiter (e.g. comma) to print nth column:
  * `awk -F "," '{print $n}'`
* Sum a list of values from stdin and print them:
  * `awk '{sum+=$n} END {print sum}'`
