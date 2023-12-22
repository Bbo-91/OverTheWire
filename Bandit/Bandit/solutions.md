<table>
<tr>
<td>level 0</td>
<td>

`ssh bandit0@bandit.labs.overthewire.org -p 2220`
</td>
</tr>
<tr>
<td>level 1</td>
<td>

`ls`\
`cat readme`
</td>
</tr>
<tr>
<td>level 2</td>
<td>

`ls`\
`cat ./-`
</td>
</tr>
<tr>
<td>level 3</td>
<td>

`ls`\
`cat 'spaces in this filename'`
</td>
</tr>
<tr>
<td>level 4</td>
<td>

`cd inhere`\
`ls -a`\
`cat .hidden`
</td>
</tr>
<tr>
<td>level 5</td>
<td>

`cd inhere`\
`ls -a`\
`file ./*`\
`cat ./file07`
</td>
</tr>
<tr>
<td>level 6</td>
<td>

`ls -alR`\
`find . -readable -size 1033c -not -executable`\
`cat ./maybehere07/.file2`
</td>
</tr>
<tr>
<td>level 7</td>
<td>

`find -user bandit7 -group bandit6 -size 33c 2>/dev/null`\
`cat /var/lib/dpkg/info/bandit7.password`
</td>
</tr>
<tr>
<td>level 8</td>
<td>

`grep -rw ./ -e millionth` or `ack 'millionth`

</td>
</tr>
<tr>
<td>level 9</td>
<td>

`sort data.txt | uniq -u`
</td>
</tr>
</table>
