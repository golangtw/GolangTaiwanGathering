# Golang Taiwan/Taipei Gathering #58

* 主辦: [COSCUP 2021](https://coscup.org/2021)
* 地點: Online
* 時間: 2021/07/31(Sun) 10:00 ~ 16:00  (UTC+8)

## 主題

### Yang Hau -- 在 Golang 召喚 SIMD 加速魔法 [[slides](https://www.slideshare.net/YangHaoYuan/golang-simd)]

SIMD 是常見的硬體加速手段，透過 SIMD 指令集的加速，我們可以將多筆資料進行平行運算，進而達到加速的效果。
通常若是要使用 SIMD 的話我們都會透過 C 語言 inline 組合語言或者使用 C 語言的 intrinsics 去呼叫。
相同的手法在 golang 中可以簡單地透過 cgo 完成，但是呼叫 cgo 所造成的時間成本在極度要求效率的場景下會造成不小的問題，
好死不死會應用 SIMD 的場合就是需要極度在意效率的狀況，在此我們以 ARM64 為例子，
以組合語言試著跟大家分享如何在 golang 中實做出 SIMD 的演算法，去避免 cgo 造成的時間成本。

### Julian Chu -- Learning go error handling design from open source [[slides](https://docs.google.com/presentation/d/1IfEJRc-tr4OcJUpTBkGq7J35UdB5F0QeZIdvbmaiGn8/edit?usp=sharing)]

go 的錯誤處理上一直被大家所抱怨, 但是回歸到開發本身, 錯誤處理的設計議題卻常常被忽略,
讓我們以 Dave 的文章 “Don’t just check errors, handle them gracefully” 爲基礎,
學習開源專案怎麼做錯誤處理設計

* 快速複習 errors API
* standard library 如何減少錯誤處理的程式碼
* errors 的種類, 以及針對不同層級 package 的應用
* 開源專案的錯誤處理設計

### 郭學聰 -- 從 Go 的 runtime 源碼發掘瘋狂的 slice 用法 [[slides](https://hackmd.io/@fieliapm/BkdNrol6O#/)]

Go 的 slice 型態在程式語言中是相當獨特的。
因為 slice 特別的設計以及實作，我們能夠以各種奇淫技巧去應用之。
這個演說會帶大家爬 Go 的 runtime 源碼，並從中解釋為何我們能夠用各種奇怪的方式去應用 slice。

### Gaston Qiu -- Go memory allocation and deallocation [[slides](https://docs.google.com/presentation/d/15U64otW4_dAI3gqxnr9IQ_TfGZ98WqDd/edit?usp=sharing&ouid=112628335219252558277&rtpof=true&sd=true)]

In the modern programming language, the memory usually separated into stack and heap.
The heap size changes during runtime. I want to introduce the mechanism and strategy
Go used to allocate new memory and deallocate the memory. Start from tcallocator component,
mcache, mcentral, and mheap and how they interact with each other when the allocation happened.
The garbage collector is responsible for deallocation. How to reuse the memory in the heap?
When should we release the memory to OS?

### Ronald Hsu (hothero) -- Orion: Golang framework building microservices [[slides](https://www.slideshare.net/hothero0705/202107-orion-introduction-coscup)]

Orion 是 Carousell 旋轉拍賣創立的 Golang 框架，已經被廣泛運用在 Carousell 超過 100 個服務上面。
可以簡單地透過 Protobuf 定義 Endpoint，接著一行指令就產生 HTTP 與 gRPC 兩種 Protocol
，搭配 Prometheus、Hystrix、NewRelic、Jaeger 的支援，快速大量構建具備良好 Observability 的 Microservice。

介紹框架之外，也會與大家分享演化到千萬 MAU 的服務中，Orion 更具備怎樣的彈性支援你的需求，
我們遇到的一些困難如何透過 Golang 與框架去一一解決。換句話說，
帶你藉由 Orion 這個框架從 0 走到破千 RPS 的旅程。

### Jalex Chang -- Memory Management in High-Performance Go Applications: A Case Study of Pebble [[slides](https://slides.com/jalex-chang/memory-management-in-pebble)]

透過研究 Pebble (CockroachDB 底層的 key-value storage engine)，談談在高效能的需求情境下， Go 專案要如何進行記憶體管理。

### Cherie Hsieh -- User authentication in Go Web Server [slides]

介紹目前 Web application 中主流的 User authentication 機制，其中包含：

* 經典 user / password，將說明在實作中大家可能忽略而造成弱點的地方
* OTP multi-factor 機制與實作流程
* 可能成為未來主流的 Web authentication protocol 流程說明
* 比較 Go user authentication 相關的 open source projects

### David Chou -- Fuzzying test in Go [[slides](https://speakerdeck.com/david74chou/fuzzying-test-in-go)]

Fuzzing test 在各領域已被證明可以有效的找到系統中的 bug 或漏洞，在 go standard library 當中也採
用 fuzzing test 的方式成功的找到並修復上百個 issue。在本 session 中，我們會來聊聊什麼是 fuzzing test、
它為什麼會有用、該如何做 fuzzing test 以及 continuous fuzzing。

### I-Fan Wang -- From System Engineer to Gopher [[slides](https://www.slideshare.net/IFanWang1/from-system-engineer-to-gopher)]

從System software engineer轉職成Golang backend engineer的心路歷程