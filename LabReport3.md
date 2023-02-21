I choose the command grep
1. -c: Output count of matching lines
This is useful if you want to find how many times a string appear in a txt. 
command:
```
grep -c "the" written_2/travel_guides/berlitz1/IntroItaly.txt. 
```
output:

```
116
```
command:
```
grep -c "this " written_2/travel_guides/berlitz2/*.txt 
```
output:
```
written_2/travel_guides/berlitz2/Algarve-History.txt:1
written_2/travel_guides/berlitz2/Algarve-Intro.txt:1
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:20
written_2/travel_guides/berlitz2/Amsterdam-History.txt:4
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt:1
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt:3
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:22
written_2/travel_guides/berlitz2/Athens-History.txt:4
written_2/travel_guides/berlitz2/Athens-Intro.txt:2
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:32
written_2/travel_guides/berlitz2/Bahamas-History.txt:2
written_2/travel_guides/berlitz2/Bahamas-Intro.txt:2
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt:8
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:21
written_2/travel_guides/berlitz2/Bali-History.txt:6
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:20
written_2/travel_guides/berlitz2/Barcelona-History.txt:5
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt:22
written_2/travel_guides/berlitz2/Beijing-History.txt:4
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt:23
written_2/travel_guides/berlitz2/Berlin-History.txt:0
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt:16
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:10
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:15
written_2/travel_guides/berlitz2/Bermuda-history.txt:4
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:12
written_2/travel_guides/berlitz2/Budapest-History.txt:4
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:24
written_2/travel_guides/berlitz2/California-History.txt:5
written_2/travel_guides/berlitz2/California-WhatToDo.txt:2
written_2/travel_guides/berlitz2/California-WhereToGo.txt:11
written_2/travel_guides/berlitz2/Canada-History.txt:9
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:61
written_2/travel_guides/berlitz2/CanaryIslands-History.txt:6
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:5
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:38
written_2/travel_guides/berlitz2/Cancun-History.txt:2
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt:6
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:25
written_2/travel_guides/berlitz2/China-History.txt:7
written_2/travel_guides/berlitz2/China-WhatToDo.txt:3
written_2/travel_guides/berlitz2/China-WhereToGo.txt:72
written_2/travel_guides/berlitz2/Costa-History.txt:3
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:29
written_2/travel_guides/berlitz2/CostaBlanca-History.txt:3
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Crete-History.txt:5
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt:5
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:36
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:13
written_2/travel_guides/berlitz2/Cuba-History.txt:2
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:18
written_2/travel_guides/berlitz2/Nepal-History.txt:7
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt:12
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt:38
written_2/travel_guides/berlitz2/NewOrleans-History.txt:4
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:12
written_2/travel_guides/berlitz2/Poland-History.txt:1
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Portugal-History.txt:2
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:26
written_2/travel_guides/berlitz2/PuertoRico-History.txt:2
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt:7
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt:22
written_2/travel_guides/berlitz2/Vallarta-History.txt:9
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:9
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:37
```
2. -o: Output the matched parts of a matching line. 
This is useful because it directly returns the string you want to find. 
command:
```
grep -o "replete " written_2/travel_guides/berlitz2/*.txt
```
output:
```
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:replete 
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:replete 
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:replete 
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:replete 
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:replete 
```
command:
```
grep -o "Hong Kong.*" written_2/travel_guides/berlitz1/HandRHongKong.txt
```
output:
```
Hong Kong has some of the most luxurious hotels in the
Hong Kong hotels
Hong Kong Hotel Reservation Center at the
Hong Kong dollars, based on double

```
3. -rl: Searches recursively through subdirectories and returns only the names of the files that contain the pattern. 
This is very useful because it can search the all the text file contain in the directory, and return just the file name. 

command:
```
grep -rl "watch them" written_2
```
output:
```
written_2/travel_guides/berlitz1/WhereToDublin.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
```
command:
```
grep -rl "he see" written_2/travel_guides
```
output:
```
written_2/travel_guides/berlitz1/HistoryJapan.txt
written_2/travel_guides/berlitz1/HistoryIndia.txt
written_2/travel_guides/berlitz1/HistoryItaly.txt
written_2/travel_guides/berlitz1/HistoryMallorca.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Amsterdam-History.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-Intro.txt
written_2/travel_guides/berlitz2/Algarve-History.txt
written_2/travel_guides/berlitz2/Cuba-History.txt
```

4. -rn: Searches recursively through subdirectories and precede each matching line with a line number. 
This is useful because it tells you the line number, which makes it easier for you to locate the line of txt with matching string. 

command:
```
grep -rn " Lucayans" written_2/
```
output:
```
written_2//travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
written_2//travel_guides/berlitz2/Bahamas-History.txt:7:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```
command:
```
grep -rn " historic cities" written_2/travel_guides/berlitz1
```
output:
```
written_2/travel_guides/berlitz1/IntroMadrid.txt:13:        catch up to Spain’s more historic cities, including Seville, Toledo and
written_2/travel_guides/berlitz1/IntroItaly.txt:81:        golden triangle of historic cities, the Assisi of St. Francis, the
```

Citation:
Vivek Gite. "How To Use grep Command In Linux / UNIX With Practical Examples". February 14, 2023 
https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/
