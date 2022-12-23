# Class 1

[401 Home](../home401.md)

## Hash Tables

Hash tables are a fantastic "cheat" at data storage that allows immediate access using a known mutator and known data. The key is stored as an index derived from the key itself via hashing / converting the data to a number. Then, the data can be recalled in constant time operations by converting the key you're searching for into the index where it will be. The potential downside is hash collisions where two keys derive to identical indexes, which means their values will collide and overwrite. To solve this, each index can instead be formatted as a linked list of values at that index. Collisions add to this considerably shorter list, and the correct value can be retrieved in far fewer operations still.
