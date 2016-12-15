# linuxUtil


Collections of unix tutorial


list directory tree console:
 find ./ -type d -print | awk -F "/" '{for (i=1; i<=NF-2; i++){printf "| "} print "|____"$NF}'

remove the first 41 character from the file name:
 for file in * ; do mv $file  $(echo $file |sed 's/^.\{5\}//g'); done
 
rename *.COMPLETED files without '.COMPLETED' string 
 for file in *.completed; do mv "$file" "${file/.completed/}"; done 
 

mvn versions:set -DnewVersion=2.50.1-SNAPSHOT

mvn versions:revert

poi se sbagli nome

mvn versions:commit per confermarla
