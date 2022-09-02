# Possible matrix multiplication

## Description

5 _ 7 matrix by 7 _ 5 matrix

###

#### Before

<pre>
BGOAMVOEIATSIRLNGTTNEOGRERGXNTEAIFCECAIEOALEKFNRFLWEFCHDEEAEEEHNMDRXXF
[1, 6, 14, 0, 12, 21, 14, 4, 8, 0, 19, 18, 8, 17, 11, 13, 6, 19, 19, 13, 4, 14, 6, 17, 4, 17, 6, 23, 13, 19, 4, 0, 8, 5, 2, 4, 2, 0, 8, 4, 14, 0, 11, 4, 10, 5, 13, 17, 5, 11, 22, 4, 5, 2, 7, 3, 4, 4, 0, 4, 4, 4, 7, 13, 12, 3, 17, 23, 23, 5]
</pre>

#### After

<pre>
380	478	152	312	386	490	132
314	218	156	290	306	592	138
573	486	245	537	647	949	288
572	700	175	526	543	792	285
356	312	176	268	370	496	227
686	844	209	656	681	990	285
150	228	38	126	98	178	69
</pre>

#### Mod 26

<pre>
[19, 14, 25, 25, 2, 21, 13, 19, 2, 17, 17, 14, 7, 3, 18, 10, 2, 4, 17, 0, 25, 14, 13, 7, 16, 14, 22, 1, 7, 16, 9, 19, 24, 13, 25, 6, 9, 23, 24, 4, 20, 9, 9, 10, 1, 7, 12, 7, 25]
</pre>

#### Map back to alphabet

<pre>
['T', 'O', 'Z', 'Z', 'C', 'V', 'N', 'T', 'C', 'R', 'R', 'O', 'H', 'D', 'S', 'K', 'C', 'E', 'R', 'A', 'Z', 'O', 'N', 'H', 'Q', 'O', 'W', 'B', 'H', 'Q', 'J', 'T', 'Y', 'N', 'Z', 'G', 'J', 'X', 'Y', 'E', 'U', 'J', 'J', 'K', 'B', 'H', 'M', 'H', 'Z']
</pre>

### AHHHHH

<pre>
mylist = [ord(char) - 97 for char in "BGOAMVOEIATSIRLNGTTNEOGRERGXNTEAIFCECAIEOALEKFNRFLWEFCHDEEAEEEHNMDRXXF".lower()]

print(mylist)

matrixsolve = [380,478,152,312,386,490,132,314,218,156,290,306,592,138,573,486,245,537,647,949,288,572,700,175,526,543,792,285,356,312,176,268,370,496,227,686,844,209,656,681,990,285,150,228,38,126,98,178,69]

newlist = [chr((x % 26) + 65) for x in matrixsolve]

print(newlist)
</pre>
