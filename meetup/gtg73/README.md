## Golang Taiwan/Taipei Gathering #70 x Dcard

* 主辦: [COSCUP 2023](https://coscup.org/2023)
* 地點: 國立臺灣科技大學
* 時間: 2023/07/30(Sun) 10:00 ~ 16:00  (UTC+8)

### Live stream link

#### [Youtube](https://www.youtube.com/watch?v=D1hI55EcBB4)

### Talks

#### Complete auto instrumentation go agent for distributed tracing and monitoring / 吳晟 and 劉晗

在這場分享中他們將首次介紹一個完整的自動增強 Go 探針解決方案，由Apache SkyWalking 打造的開箱即用。
Golang 在雲原生和分散式系統中被廣泛使用。為了保持系統的可觀察性，分散式追蹤，指標以及日誌是關鍵技術。以往供應商和開源社群總是建議使用 SDK 來增強代碼，這意味著開發人員必須修改代碼。
在這次演講中，吳晟和劉晗將會讓你
1. 學習如何使用完整的自動增強 Go 探針解決方案。
2. 了解如何保持系統的可觀察性，並進行分散式追踪，指標，以及日誌監控。
3. 探索 Apache SkyWalking 帶來的創新技術和實踐經驗。


#### PGO (Profile-Guided Optimization): The Secret Weapon for Accelerating Golang Programs / 韓吉 Hanji / [Slides](https://speakerdeck.com/msc7wc91w/hanji-coscup)

在這場分享中，我將會向大家介紹 PGO（Profile-Guided Optimization），這個 Golang 1.20版本中導入的一項功能。
在這次分享中，講者將會提到
1. PGO 的原理和應用。。
2. PGO 如何收集執行時的性能資料應用於編譯器，並對程式做性能優化

#### From Event Storming to Clean Architecture in Go / River Lin, Backend Dept. Lead in XRSPACE inc. 

River Lin 將向你介紹從 Event Storming 到 Go 語言的乾淨架構的應用
在這次演講中，你將會得到以下收穫：
1. 學習使用 Event Storming 來搜集需求的方法論。
2. 探索如何將需求轉化為乾淨的程式碼，提高程式碼的可讀性和可維護性。
3. 了解如何在 Go 語言中應用乾淨架構，提高開發效率和代碼品質。


#### Zoraxy - 用 Go 開發的新手向反向代理伺服器與集群管理小工具 / tobychui, 成大資工所研究生 / [Slides](https://docs.google.com/presentation/d/1W7wNIND9H0DvVsfMaEEebWf-DSZQbF2dMY5BjmPL7Zo/edit?fbclid=IwAR3wk81nMTu53T8_u4nayxq2IDGuQzD9N90xXqlHmDByO3Na-XKKWIR_M9A#slide=id.g1f665521969_2_75)

這次 Toby Chui 會為大家帶來他做的 side project - Zoraxy，是個用 Go 開發的新手向反向代理伺服器與集群管理小工具，內容如下
1. 學習如何快速而有效地設定反向代理伺服器
2. 克服 Zerotier 設備限制，無阻礙地發展你的 IoT 網絡
3. 輕鬆設定你的 homelab 集群 (即使是初學者也能輕鬆上手)

#### 深入淺出 Go AST，動手做自己的 Linter / YCKao, SRE in DCARD 

不知道大家有沒有對於程式碼品質的控制有所要求呢？
如果在導入第三方Linter時遇到了一些想功的能沒有支援，怎麼辦呢？

於是乎，以下便是這場會帶給你的：
- AST 結構的基礎
- 使用工具快速檢視 AST
- 使用 analysis.Analyzer 開發自己的 Linter
- 如何將自製 Linter 搭配 golangci-lint 一起使用

#### Protocol Buffers v3 in Go / Rain, Senior Software Engineer in NetScope

在API的發展中，RPC技術已經是個為時很久的東西（比REST還久）。直到近年gRPC的興起，HTTP2.0的引入，服務之間資料的傳遞方法又添了一員生力軍。

於是今天！我們請來了Wu Rain介紹在寫gRPC服務時，一定會碰到的protocol buffer！本次Rain將透過自身經歷，分享一些使用它帶來的生產力提升以及一些適合使用的環境，為聽眾帶來一個入門等級的分享！

#### WebAssembly for the backend / Adrian Cole, Open Source WebAssembly Engineer in Tetrate

This talk covers integration patterns of WebAssembly through backend software, like CLIs and side cars. It shows how to embed WebAssembly into Go applications, and what to watch out for when programming. When we’re done, you’ll have a good sense of how WebAssembly fits into what you’re working on.

#### Go to Generics = Go to hell? What I experienced after Generics Introduced into Go / Hsueh-Tsung Kuo

聽過泛型（Generics）嗎?
對於喜歡Statically typed language 的部分人來說，泛型大概是一個萬惡的代名詞吧。
所以我們的講者將在接下來的時間內，說說在1.18之後引入的Go Generics，以及它對Go 工程師帶來的一些影響吧！至於結論是支持與否，就等你們來現場討論了！