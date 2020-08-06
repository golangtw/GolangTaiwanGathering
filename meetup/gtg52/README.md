# Golang Taiwan/Taipei Gathering #52

* 主辦: [COSCUP 2020](https://coscup.org/2020)
* 地點: 國立臺灣科技大學
* 時間: 2020/08/02(Sun) 10:00 ~ 16:00  (UDT+8)

## 主題

### Hsueh-Tsung Kuo -- net & http & timeout [[slides](https://hackmd.io/@fieliapm/rkmPNSx-P#/)]

Go 的 standard library 內已經內建了 net package，並以此為基礎提供方便的 net/http package。
實務上為了避免連線資源長時間被佔用，甚至是被挾持，我們會針對 http request 的各個進行階段設定相對應的 timeout，確保沒有資源 leak 的風險。
但 Go 官方的 http timeout 參數都只能控制各階段的完成時間，沒有一項 timeout 設定適合 streaming request 與 streaming response 的應用場合。
故在此提出新的開源小 package，逐一解釋其實作考量，並點出當前實作上不甚完美，卻沒有簡單解法之處。
希望能普渡眾碼農，同時抛磚引玉，讓有想法的人能夠建議與改良這個 package。

### Gaston Chiu -- 使用Go channel的正確姿勢 [[slides](https://slides.com/gastonchiu/deck)]

對於有寫過Go的人來說，對channel應該不算陌生，channel讓我們更方便的進行不同Go routine之間的溝通，我將由淺入深的從介紹channel的正確使用姿勢開始，再來介紹channel的實作，如何正確的在goroutine之間傳遞訊息，並且達到thread safe。

### lschyi -- cgo 與 channel 的陷阱如何造成讀取 usb message 失敗 [[slides](https://hackmd.io/@_Zlxrb-rRNucaVTNB_4_yQ/HyR_eHMZv#/)]

分享在使用 cgo 串接現有的 c library 讀取， usb 裝置送來的訊息的應用所遇到之困難。此應用目的是讀取一把自製的 usb 鍵盤的 debug message，但因 cgo call performance，channel 的特性而讀取到異常的訊息。我將分析問題的成因，以及最後的解決方法。。

### Peter Lai -- Debug golang program with delve [slides 待補]

1. how delve works.
2. debug with delve.
3. deterministinic debug with delve.

### David Chou -- 談談 go 測試的二三事 [[slides](https://slides.com/ting-lichou/go-test-experience-sharing)]

雖然 go 已經把測試做了很好的整合，但仍有許多眉角需要注意的，本 session 將由淺入深，從最簡單的 unit test 講起到 table-driven test、interface mocking、dependency injection 最後再到做 integration test 的心得分享，還有如何利用 fake data 來簡化產生「測資」這件煩人的小事。

### Rain Wu -- Functional verification test framework with Go [[slides](https://www.slideshare.net/RainWu1/coscup-2020-rain-wu-functional-verification-test-framework-with-go)]

當工程師發覺自己的腦袋無法確保自己寫的程式正確運作時，決定透過寫測試來解決這問題。作為一個使用 Go 語言的新手，在摸完 go test 方便簡潔的功能後，一時手癢就決定自己動手寫一個更適用於 Functional Verification Test 的工具。本次議程講者會從 go test 使用思維開始，整理開發中遇到的 Unit Test、Functional Verification Test 性質及需求，並分享設計和實作測試框架的經驗。

### Cherie Hsieh -- Goroutine stack and local variable allocation in Go [[slides](https://www.slideshare.net/CherrieHsieh/goroutine-stack-and-local-variable-allocation-in-go)]

相信蠻多 Gopher 都知道改寫自 tcmalloc 的 Go dynamic allocator，不過你有了解過 Go 的 goroutine stack 與其 local variable allocation 機制嗎？本次分享將由工程師最熟悉的 C local variable allocation 講起，然後再來說明 Go 是如何實現它的 goroutine stack 和 local variable allocation，並且也會提到 goroutine stack extension 議題。

### kakashi-- 從零開始貢獻 Go 相關 open source project [slides 待補]

生為長期使用 Go 的開發者，難免會用到很多相關的 opensource tool，而一般來說，很多的 open source project 都相對比較成熟，也讓人比較難以參與，這邊講者想要分享一個比較容易貢獻的模式，並且分享從中學習的過程。

### Yu-Lang Chu-- Go Go Power Slice! [[slides](https://www.slideshare.net/JulianYuLangChu/go-go-power-slice)]

slice in golang is a very important type to perform operations on collection data. When you have experience with other programming languages, will find the design of slice has some differences when compared to similar type in other programming languages. These differences make us need to pay attention to memory allocation by doing slice manipulation in order to get better performance or avoid some mistakes. Let’s start from source code to discuss more details in slice manipulation.