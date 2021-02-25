# 以放射狀辨識中文字

這項目是想沿用[上一項專案](https://github.com/him121415/Chinese_chess_recognition)的方式來辨識中文字，步驟可至上一個專案觀看，但辨識率極低無繼續進展。
與上一項專案的差別為，並未做到分群Fuzzy C-Means分群動作，只有先進行劃分初始環以及角度，這部分我們是進行8環8角，共會劃分出64個區域，計算每個區域內的黑點數量，以來當作特徵。

後期回來研究該專案程式碼，發現取的特徵並非上述區域中黑點數量而是角度，因未進行分群動作每個文字的角度會是相同，也就無法比對出差異，才導致出辨識率極低狀況，但當時以為效果太差而以轉至其他專案製作，此項目也無繼續進展。