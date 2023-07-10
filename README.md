# Network-101

## Lesson1
### Bridge
交換器是一種負責網路橋接（network bridging）的網路硬體設備，會讀取網路卡的MAC位址來轉發資料，將資料準確地送達目的地


### L2 ARP(Address Resolution Protocol)
是利用乙太網路的廣播功能所設計出來的位址解析協定，利用查詢的方式來獲得IP Address和MAC Address(實體位址)的對應關係。當發送主機(Sender)有一個封包要傳送給目標主機(Target)時，並且已獲得目標主機的IP位址，那發送主機會先檢查自己的ARP table中是否有該IP address與Mac Address的對應。
1. If True，就直接將此IP所對應的MAC Address填入Layer 2 header。
2. If False，則向網路發出一個ARP Request的Broadcast封包，查詢目標主機的Mac Address。

### HW:
1. 利用wireshake觀察ARP broadcast封包
2. 在linux環境下尋找ARP cache
3. 預習bridge概念


## Lesson2
