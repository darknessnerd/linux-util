# linuxUtil


Collections of unix tutorial


list directory tree console:
 find ./ -type d -print | awk -F "/" '{for (i=1; i<=NF-2; i++){printf "| "} print "|____"$NF}'
