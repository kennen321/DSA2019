##  Linked list
連結串列(Linked List)是串列(List)的一種，是一種常見的資料結構，
利用這個資料結構也能進一步實作出其他的資料結構，例如堆疊(Stack)和佇列(Queue)等。

它的特性是能夠不使用連續的記憶體空間的情況下，能夠保有並使用一份連續的資料；相對來看，陣列則需要使用連續的記憶體空間。

他的的實作方式是每個節點除了記錄資料之外，還使用額外的指標指向下一個節點，將節點以此方式串連起來形成一個連結串列。

由以上的說明可以知道，使用連結串列的優點如下：

不需使用連續記憶體空間，不需事先指定串列大小。
能夠容易的修改指標，插入或移除節點。
但也有缺點如下：

使用額外的記憶體空間紀錄節點指標。
無法快速索引到某個節點，必須迭代搜索。
此資料結構可以實作的操作變化相當多，這裡實作以下幾種操作：

getFirst：取得第一個節點。

getLast：取得最後一個節點。

addFirst：加入節點在最前面。

addLast：加入節點到最後。

addBefore：加入節點在某節點之前。

addAfter：加入節點在某節點之後。

removeFirst：移除第一個節點。

removeLast：移除最後一個節點。

remove：移除某一個節點。

size：取得串列的數目。


### 優點：

新增/刪除資料較Array簡單，只要對O(1)個node(所有與欲新增/刪除的node有pointer相連的node)調整pointer即可，

不需要如同Array般搬動其餘元素。

若是在Linked list的「開頭」新增node，只要O(1)。

若要刪除特定node，或者在特定位置新增node，有可能需要先執行O(N)的「搜尋」。

Linked list的資料數量可以是動態的，不像Array會有resize的問題。

### 缺點：


因為Linked list沒有index，若要找到特定node，需要從頭(ListNode *first)開始找起，搜尋的時間複雜度為O(N)。

需要額外的記憶體空間來儲存pointer。





參考資料: https://emn178.pixnet.net/blog/post/93557502

http://alrightchiu.github.io/SecondRound/linked-list-introjian-jie.html
