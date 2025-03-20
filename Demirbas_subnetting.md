

## Übung 1

Teile das Netz 192.168.0.0 mit der Netzmaske /24 in 4 Subnetze auf. Dabei solltest du Netze wählen, die die minimal benötigte Anzahl an Hosts haben, aber nicht darunter liegen. Die Subnetze sollen folgende Anforderungen erfüllen:

- Subnetz a: 20 Hosts
- Subnetz b: 15 Hosts
- Subnetz c: 30 Hosts
- Subnetz d: Die restlichen Adressen

**Antwort**

Für die Subnetzaufteilung beginnt man mit der ersten Subnetzmaske, die ausreichend viele Hosts für das Subnetz a bereitstellt. Das Netz 192.168.0.0 /27 stellt 32 Adressen zur Verfügung, wovon 30 für Hosts verwendet werden können. Daher hat das erste Subnetz (a) die Adresse 192.168.0.0 und geht bis 192.168.0.31. 

Das nächste Netz (b) braucht ebenfalls 15 Hosts. Auch hier reicht eine Subnetzmaske von /27, die 32 Adressen bereitstellt. Das Subnetz b beginnt bei 192.168.0.32 und endet bei 192.168.0.63.

Für das Subnetz c, das 30 Hosts benötigt, wird ebenfalls ein /27-Netz verwendet. Es startet bei 192.168.0.64 und endet bei 192.168.0.95.

Das verbleibende Netz d verwendet die restlichen Adressen und benötigt eine größere Subnetzmaske von /25. Dieses Subnetz beginnt bei 192.168.0.128 und geht bis 192.168.0.255.

---

## Übung 2

Teile das Netz 193.170.20.0 /24 in 8 gleich große Subnetze auf. Erstelle eine Übersicht mit den Netzwerkadressen, den verfügbaren Hosts, den Broadcastadressen und der Subnetzmaske.

**Antwort**

Um das Netz in 8 gleich große Subnetze zu teilen, wird die Subnetzmaske auf /27 angepasst. Jede Subnetzmaske /27 bietet 32 Adressen, wovon 30 für Hosts verwendet werden können. Die Subnetze beginnen bei 193.170.20.0 und werden in Schritten von 32 Adressen aufgeteilt, also:

- Das erste Subnetz startet bei 193.170.20.0 und endet bei 193.170.20.31.
- Das nächste Subnetz beginnt bei 193.170.20.32 und endet bei 193.170.20.63, und so weiter.

Jedes dieser Subnetze hat eine Subnetzmaske von /27 und stellt Platz für 30 Hosts zur Verfügung.

---

## Übung 3

Teile das Netz 172.28.40.0 /26 in zwei Subnetze auf und gib die Details zu den Subnetzgrößen und Adressen an.

**Antwort**

Das Netz 172.28.40.0 /26 bietet Platz für 64 Adressen (62 nutzbare Hosts). Um es in zwei Subnetze zu teilen, wird die Subnetzmaske auf /27 geändert, was 32 Adressen pro Subnetz ergibt. Das erste Subnetz reicht von 172.28.40.0 bis 172.28.40.31 und das zweite Subnetz von 172.28.40.32 bis 172.28.40.63. 

---

## Übung 4

Bestimme die Subnetzmaske für das Netz 17.0.0.0, wenn du 10 Subnetze mit mindestens 12 Hosts pro Subnetz benötigst. 

**Antwort**

Um 10 Subnetze zu erstellen, die mindestens 12 Hosts pro Subnetz unterstützen, benötigen wir eine Subnetzmaske von /28. Diese Subnetzmaske stellt 16 Adressen pro Subnetz bereit, von denen 14 tatsächlich nutzbar sind. Die Subnetze starten bei 17.0.0.0 und werden in Schritten von 16 Adressen aufgeteilt, sodass das erste Subnetz bei 17.0.0.0 beginnt und bei 17.0.0.15 endet. Das nächste Subnetz beginnt bei 17.0.0.16 und endet bei 17.0.0.31, und so weiter.

---

## Übung 5

Bestimme die Subnetzmaske für das Netz 210.52.190.0, wenn du 5 Subnetze benötigst und jedes Subnetz mindestens 10 Hosts unterstützen muss.

**Antwort**

Um 10 Hosts pro Subnetz zu ermöglichen, benötigen wir eine Subnetzmaske von /28. Da jedoch mindestens 5 Subnetze benötigt werden, müssen wir das Netz auf /25 erweitern, was 128 Adressen pro Subnetz bietet und ausreichend für die 5 Subnetze ist. Das erste Subnetz beginnt bei 210.52.190.0 und geht bis 210.52.190.127, das zweite Subnetz beginnt bei 210.52.190.128 und endet bei 210.52.190.255, und so weiter.

---

## Übung 6

Teile ein /30-Netz auf und erkläre, wozu diese Netze verwendet werden.

**Antwort**

Ein /30-Netz bietet nur 4 Adressen, von denen 2 für Hosts verwendet werden können. Diese Netze werden häufig in Punkt-zu-Punkt-Verbindungen zwischen zwei Routern verwendet, da nur zwei Hosts benötigt werden. Durch die geringe Anzahl an Adressen sind diese Netze ideal für direkte Verbindungen zwischen Geräten, ohne unnötige IP-Adressen zu verschwenden.

---

## Übung 7

Bestimme den Netzwerk- und Hostanteil für die Klassen A, B und C.

**Antwort**

- **Klasse A**: Der Netzwerkanteil ist 8 Bits (1 Oktett), der Hostanteil umfasst 24 Bits (3 Oktette). Die Standard-Subnetzmaske ist 255.0.0.0 (/8), und jedes Netz kann bis zu 16.777.214 Hosts unterstützen.
  
- **Klasse B**: Der Netzwerkanteil ist 16 Bits (2 Oktette), der Hostanteil umfasst 16 Bits (2 Oktette). Die Standard-Subnetzmaske ist 255.255.0.0 (/16), und jedes Netz kann bis zu 65.534 Hosts unterstützen.
  
- **Klasse C**: Der Netzwerkanteil ist 24 Bits (3 Oktette), der Hostanteil umfasst 8 Bits (1 Oktett). Die Standard-Subnetzmaske ist 255.255.255.0 (/24), und jedes Netz kann bis zu 254 Hosts unterstützen.

---

