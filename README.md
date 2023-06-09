# 積體電路設計實驗 (IC Lab)
## 概述
- 課程名稱：積體電路設計實驗
- 選修年度：111下
- 授課教師：李鎮宜副校長
- 開課單位：電子碩     
- 永久課號：EEIE30041
- 學分數：4.00
- 必/選修：選修

課程比較有名的別名為 交大IC Lab。是在批批踢和 Dcard 看板上出現頻率比較高的一門課，以其不人性的作業 loading 與紮實程度著稱。我是在專題老師的推薦之下決定利用大四下的時間好好修過，也算是在大學的最後一個學期補上數位電路設計最核心的一門課。修課的同學大部分為電類碩士，接下來是電機系大四的同學。還有為數不少其他科系對於 IC 設計有興趣的同學，希望修過這一門課方便找相關工作。課程設計目的是帶修課同學粗略的跑過一次 Design Flow，當然比較著重在前端的部分。開課的李鎮宜副校長在第一堂課就有特別提醒(警告)沒有準備好的同學最好不要貿然接受這 12 Lab + Midterm/Final Project 的洗禮。最後一堂課李教授還有特別恭喜所有同學已經具備初步 IC 設計的能力，我覺得挺感動的。在那些為了 deadline 而搔頭並熬夜的煎熬，還是非常值得的。

## 上課模式

除了第一堂課和最後一堂課之外，李教授是不會親自到課堂上授課的。而是會由數個助教負責，每個助教的教學品質不同，大多數還算口齒清晰，言之有物。不過講義上的內容還需要同學們自己回去看講義複習，或是從實做中慢慢累積經驗。通常課堂的一開始會由上個 Lab 表現最好的同學來講解自己的設計理念和實作細節，讓其他同學觀摩學習。接下來助教就會接手講解當天設定的課程內容。最後還會帶同學們看過一次當周的 Practice 和 Exercise，讓同學們對於題目有初步的認識。上課時間通常兩個小時就結束了，不會拖到很久。期中考核期末考的內容也是從講義裡面出的，況且當周的 Exercise 都會運用到課堂上講的知識，想要通盤的理解課堂，認真聽講是非常重要的第一步。整個學期所學到的課程主題如下:

#### 單元列表

Week | Course Content | Lab Unit | Pass Rate
:--------|:-----| :----- | :----: 
01| [Introduction (Environment Setting)][L00]                                               | -                                                         | -
02| [Verilog Combination Syntax][L01]                                                       | [Lab01: Chinese Course][s01]                                            | 92.45%
03| [Sequential Logic Design (1/2) + generate syntax][L02]                                  | [Lab02: 12-Queen][s02]                                                  | 73.58%
04| [Testbench Programming Syntax][L03]                                                     | [Lab03: Subway Surfes][s03]                                             | 91.84%
05| [Sequential Logic Design (2/2)][L04]                                                    | [Lab04: Simple RNN][s04]                                                | 91.84%
06| [Memory & coding style & nLint][L05]                                                    | [Lab05: Matrix Multiplication to find Trace][s05]                       | 87.63%
07| [Design Compiler + IP Design (DesignWare) with genvar][L06]                             | [Lab06: Elliptic Curve Group Operation][s06]                            | 88.86%
08| [Midterm Exam][midterm_exam] + [Online Test][OT] + [Midterm Project][midterm_pj]        | [Midterm Project: Gray-level co-occurrence matrix (GLCM)][src_midterm_pj]   | 87.63%
09| [Synthesis & Static Time Analysis + Cross Clock Domain][L07]                            | [Lab07: CDC Doraemon tester][s07]                                       | 81.44%
10| [Low power design][L08]                                                                 | [Lab08: Siamese Neural Network][s08]                                    | 86.46%
11| [SystemVerilog for design][L09]                                                         | [Lab09: Online Shopping Platform Simulation][s09]                       | 75.79%
12| [SystemVerilog for verification][L10]                                                   | [Lab10: OS (from Lab09) Coverage][s10]                                  | 80.85%
13| [Formal Verification (Bonus)][L_bonus]                                                  | Bonus Lab                                                   | -
14| [APR: From RTL to GDSII][L11]                                                           | [Lab11: Matrix Multiplication with Systolic Array][s11]                 | 95.29%
15| [APR: IR-Drop Analysis][L12]                                                            | [Lab12: Train Tour APRII][s12]                                          | 97.65%
16| [Final Exam][final_exam] + [Final Project][final_pj]                                    | [Final Project: Customized ISA Processor][src_final_pj]           | 67.50%


[L00]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec00%20Developmental%20Environment.pdf
[L01]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec01%20Verilog%20Combinational%20Circuits%20Design.pdf
[L02]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec02%20Sequential%20Circuit%201.pdf
[L03]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec03%20Testbench%20and%20Pattern.pdf
[L04]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec04%20Advanced%20Sequential%20Circuit%20Design.pdf
[L05]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec05%20Introduction%20to%20Macros%20and%20SRAM%20Lint.pdf
[L06]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec06%20Synthesis.pdf
[L07]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec07%20Static%20Timing%20Analysis.pdf
[L08]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec08%20Low%20Power%20Design.pdf
[L09]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec09%20SystemVerilog.pdf
[L10]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec10%20SystemVerilog%20Verification.pdf
[L11]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec11%20Cell%20Based%20APR%20Flow.pdf
[L12]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Lec12%20APR(1-2).pdf
[L_bonus]:https://github.com/hankshyu/ICLab_2023/blob/main/lectures/Bonus%20Formal%20Verification.pdf

[s01]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab01
[s02]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab02
[s03]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab03
[s04]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab04
[s05]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab05
[s06]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab06
[s07]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab07
[s08]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab08
[s09]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab09
[s10]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab10/Exercise
[s11]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab11
[s12]:https://github.com/hankshyu/ICLab_2023/tree/main/src/Lab12


[midterm_pj]:https://github.com/hankshyu/ICLab_2023/tree/main/exams/midterm
[src_midterm_pj]:https://github.com/hankshyu/ICLab_2023/tree/main/src/MidtermProject

[final_pj]:https://github.com/hankshyu/ICLab_2023/tree/main/exams/final
[src_final_pj]:https://github.com/hankshyu/ICLab_2023/tree/main/src/FinalProject


[midterm_exam]:https://github.com/hankshyu/ICLab_2023/tree/main/exams/midterm
[OT]:https://github.com/hankshyu/ICLab_2023/tree/main/src/OnlineTest
[final_exam]:https://github.com/hankshyu/ICLab_2023/tree/main/exams/final


想當然爾，只有上課認真在這堂課是遠遠不夠的。這堂課最有名的就是總共 12 次 Lab Exercise。從每個禮拜三公布題目開始，1de 的期限是下個禮拜一中午， 2de 則是到下禮拜三中午，所謂的通過是指通過**所有**的測試資料。也就是說如果你通過了1de就會有兩天的休息時間，否則就整個禮拜都在寫作業。lab 的成績計算方式通常是通過 demo 就有基本分 70，另外的分數是要和其他同學設計做比較，分數按照名次依序遞減到 0，蠻殘酷的。2de 的話會打七折。這套計分系統的設計很大程度模擬了電路設計就業環境的假定: 必須在時間壓力下設計出功能正確的晶片才能夠快速搶佔市場，取得先機。並且通常是贏者全拿的現象。

這堂課也有期中考及期末考，考試內容都從講義上出，形式是紙筆測驗，每一次考試剛好涵蓋六個主題。想要考得好成績，拿到考古題會很有幫助。也會在期中考當天進行一次上機考，可以把他想成難度介於 Practice 和 Exercise 之間的測驗，現場也會有 1de & 2de ，如果沒有當場做出來也可以帶回家慢慢做，但分數就會被打對折。另外上機考試只能使用 Vim 或 Gedit 這兩個文字編輯器，對於原本習慣用其他文字編輯器的同學會是個需要克服的點。

另外就是期中專題和期末專題了。期中專題會是利用 AMBA Bus 來串聯 DRAM 和運算電路並進行高速的資料吞吐，難度是比每個星期的 Lab Exercise 還要複雜一些，需要同學自行設計 Cache 的架構來進行加速。期末專題則是總結整個學期所學的電路設計流程，設計一個簡易版的微處理器。要從前端的RTL 一路到後端的 APR，算是為整個學期的學習做一個很好的總結。專題的內容都會要求使用到 DRAM 以及 SRAM 等記憶體元件，因此 Lab05 介紹有關 Memory 的使用就格外重要。期末專題如果有修過計算機組織(架構)的課程應該會很有幫助，可以更加熟悉處理器架構。

## 評分方式
在學期初就有公布課程配分如下:

- Weekly Lab Exercise x12 (60%)
- Midterm Project (10%)
- Midterm Exam (6%)
- Online Test (8%)
- Final Project (10%)
- Final Exam (6%)
- Bonus (Formal Verification) (3%)

雖然理論上助教期末會進行調分，不過調分的比例不是很固定，希望追求高分或是想抵免研究所學分的同學，最好盡量避免 2de 的情況。也可以參考下面的幾點建議，有效的提高分數。

## 給未來修課同學的建議

#### 1. 優質的 Pattern

邏輯驗證在複雜的軟硬體系統中至關重要，尤其在低容錯率的電路設計上更為關鍵。在這堂課中提到兩種驗證電路的方式: PATTERN-based 和 Formal Verification。後者會以 Bonus Lab 的形式出現讓同學們練習。大多數形況下都是依靠 00_TESTBED 裡面的PATTERN 來測試自己的 RTL 是否正確。因此擁有一個高 coverage 的 PATTERN 非常非常的重要，是你需不需要 2de 的關鍵。1de 後助教就會公布測試的 PATTERN，這時候 debug 起來也會變得異常輕鬆。大部分的同學取德 PATTERN 的方式就是直接把群組裡面的拿來用或是跟其他同學要。我會說種方式或許是最聰明的。因為撰寫 TESTBED 所需花費的精力通常大於設計 RTL 所花費的精力。另外也可以省下寶貴的時間多優化 RTL，衝高自己的排名。

雖然在業界確實分為DE 及 DV，且 DE 通常待遇比較好。但我們永遠無法預期將來產業的趨勢，特別是在電路愈發複雜的今天，電路驗證早已成為電路設計的瓶頸。在學生時期就選擇抄近路對於實力的累積有負面的影響，也有可能限制未來發展的可能性。自己撰寫測試程式雖然對短期的成績比較不利，但是長遠來看，同時精通測試以及設計對於未來的發展有不可抹滅的優勢。這也是我自認為在這堂課學到最多的地方。我通常會先用高階語言寫一些模擬的軟體來幫助我探索題目和設計我的電路架構。而寫 PATTTERN 通常可以分為兩種方法:

- 直接利用 Verilog / SystemVerilog 生成 stimulus 進行驗證
- 利用高階語言生成測試資料，並利用 Verilog file IO 的方式進行驗證

後者的好處是高階語言寫起來比較快速簡單，應用在對應關係明確的 TESTCASE 上效率很高，缺點是比較難追蹤資料處理的過程，訊號的取得比較困難。相反的直接利用 Verilog 原生語言來產生 stimulus 則有利各種訊號的追蹤。也更容易直接加上新的邏輯方便除錯並直接顯示在波型圖上。缺點就是寫起來比較費工，需要更長的開發時間。我非常建議想要精進自己的修課同學自己手動寫 PATTERN，對於實力的累積非常有幫助，也可以當個好人分享給大家。當然用公版的也不失一種方法。

#### 2. 像要輕鬆一點請抱團，想學到東西盡量自己完成

如果要比較資工和電機有什麼鮮明的個性特點，那組團大概是屬於電機系的標籤。有別於資工系同學多數都採單打獨鬥的英雄主義，電機系的同學早已習慣狼群戰術，而這一堂課組團也能為你贏得許多好處。除了能拿到基本沒有成本的 PATTERN、可以和同學在作業初期就一同討論架構設計，獲得起跑優勢、如果有任何一個同學發現了一些神奇的做法，所有人都可以跟著受惠以及有問題可以一群人一起 debug 等等，好處不勝枚舉。而可憐如我只能自己一個人經歷這一切，自己設計 PATTERN、自己做架構設計、自己 debug ... 話雖如此，到了期末我也發現我進步很多，可能也要受惠於我什麼都自己來吧! 還是建議未來修課的同學盡量抱團，但如果你跟我一樣喜歡 do it the hard way，你很可能會有更多的收穫。

#### 3. 熟悉EDA tool，探索更多功能來增加效率

在課堂上會用到許許多多的工具軟體來輔助電路設計，例如使用 Verdi 的 nWave 來看波形圖，PrimeTime 來分析時序等等。裡面都有許多功能能顯著的增加效率的。拿 nWave 舉例，可以調整不同訊號的顏色和調整不同數字表示法來輔助除錯，也可以將不同訊號組成 bus 方便觀察。在使用 Design Compiler 時也可以加上一些參數，讓合成結束後的 Report 顯示更多資訊。善用各種 EDA tool 可以為你帶來許多隱形的優勢，也符合課程的設計目標: "convey the senior and graudated EE students techniques to design the VLSI chips using state-of-the-art CAD tools" 

#### 4. 向 Best Code 學習，了解自己的不足

每次助教都會請上次 Exercise 表現最好的 Best Code 講解自己的作法並公開程式碼給大家參考。我覺得可以善加利用這個機會，了解厲害的同學採用的架構設計為什麼能拿到比較好的分數。是不是有哪些技巧可以延伸使用到其他場景? 如果能慢慢學習其他人的優點，將其融入自己的設計中，就會越來越進步。我身邊有一個反面例子，有一位同學就是因為每次都只求通過就好，導致到最後的Final Project都還不太清楚 shift register 的用處。這樣就會很可惜，也少學到很多東西。

#### 5. 不要害怕問問題
每個 Exercise 和 Project 助教都會在 e3平台上開一個討論區供同學們問問題。一定要善用這個公開的平台，特別是當你的背後沒有一個優良的團隊時。上面別人遇到的問題也是很好的參考，畢竟別人遇到的問題你也有很高機率會遇上。如果碰上什麼疑難雜症也可以善用這個平台發問，助教通常會在一天內回覆。我也私訊過個別的修課同學請教問題，也接收過一些其他修課同學的私訊。以親身經歷體會到不要害怕提問真的可以學到很多。

#### 6. 善用網路資源，但避免抄襲

網路上其實不乏這一堂課的參考資料，在許多平台上都可以找到之前修課同學的原始碼。站在巨人肩膀上的同時，也別忘記參考別人的作法不等於直接 Ctrl + c/v 別人的作品，除了侵犯智慧財產權之外，也違反了自己在第一堂課上簽訂的 honour code。抄襲也應該是助教要嚴格防範的事情，才能保證所有修課同學的公平性。像是我修課這一屆就有出現四五個人每次的作業面積、速度等參數都非常接近。一看就知道事情不單純。我也不是在指控他們都直接複製貼上，而是這樣不免讓人起疑。當然如果是組團一起打怪不免會互相參考，這也是課程助教需要拿捏的尺度問題。雖然我們這一屆沒有任何人被抓抄襲，尺度比較鬆散。但也有耳聞前幾屆有大規模抓抄襲的情況，同學們好自為之。

#### 7. Never Give up

想想之前所花費的時光和努力，中途退出不是太可惜了? 就算有一兩次成績不理想，也請堅持下去。在學期結束時一切都會值得的! 


## 結語

我在和專題老師聊到這門課時，都覺得這堂課有些過譽了。能夠修過交大有名的課程當然是很值得驕傲的事情，不過其實也沒有網路上誇示的那樣: 修過就直接 XXX。交大還有許多課程難度完全不輸給這堂課，帶給同學的思考空間或許還更多。我和一些修課同學聊天的時候發現很多人都只是因為薪水的緣故而選擇走數位電路設計: 我其實也沒有特別喜歡IC設計，就是出去薪水比較好就來修了。"Find a job you love and you'll never have to work a day in your life"。金錢至上的價值觀很容物讓人失去目標，相反的追尋興趣才能淵遠流長。

上面那一段不代表我在黑這門課，相反的，我認為他絕對擔當的起交大王牌課程的美譽。教學內容非常紮實且重要，能夠讓修課同學在一個學期內有如此大的進步真的很不可思議，只是他的光環也常讓修過的人對自己的實力過度自信，扼殺了持續進步的可能。修完之後我覺得我很幸運能利用大四的時間修完這樣一堂很花時間卻很重要的課。我也期待能運用課堂上學到的技巧和知識在我感興趣的領域上。當然我也要感謝和我一起討論問題的電機系同學們，以及推薦我去上課的老師。

推薦這門課給想要挑戰自己，且對於數位電路設計有興趣的同學。

