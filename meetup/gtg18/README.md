## Golang Taiwan/Taipei Gathering #18

### Time

#### 2016/11/29(Tue) 19:30 ~ 21:40  (UDT+8)

### Resgistration Page:

#### [Regstration Info](http://golang.kktix.cc/events/gtg18)

### Talks

- Umbo CV - Ramax: Write Heavy Service in Go [[Slide](https://docs.google.com/presentation/d/10V9SYlX45Q_dYFdhN0-qakVBSFbEmLvYa3QBQx2K4H4/edit?usp=sharing)], [[Video](https://youtu.be/ztVUWWm2Qbk)]

分享如何使用 Go 語言來實作 heavy service。「Heavy」意指不使用輕量化的 goroutine，而是使用獨立行程來服務各個連線。我們會透過實作一個簡單的 echo server 來講解其中的細節。

Ramax will introduce how to write a heavy service in Go which uses individual processes to serve each request instead of using lightweight
goroutines. He will demonstrate the details by implementing a simple
echo server.

**公司介紹：**

Umbo CV 是間專注在運用 machine learning 和 cloud technology 來解決傳統監控產業痛點的 startup，我們運用 cloud 讓攝影機更容易安裝與使用，我們用 ML 來大幅提升監控影像辨識的準確度。

**講者介紹:**

Ramax Lo 在 Umbo CV 擔任韌體工程師，主要負責監控攝影機的開發。近期也開始涉足後端串流服務的開發工作，也因此開始接觸 Golang。


- LIVEHouse.in - Browny : Structures in Go [[Slide](http://go-talks.appspot.com/github.com/browny/talks/2016/structures-in-go/structures-in-go.slide#1)], [[Video](https://www.youtube.com/watch?v=EIWQ3vJhBlo)]


分享 Go 專案開發在 LIVEHouse.in 是什麼樣貌，從專案結構、團隊協作到佈署流程。
討論怎麼利用 Go 的語言特性架構一個富有彈性易於測試的大型軟體專案。

Browny will share how "Go dev in LIVEHouse.in" feels like. This talk covers project structure, team collaboration and deploy flow. 
How to build a flexible and easy to test software project by Go will be discussed too.

**公司介紹：** 

LIVEhouse.in 為一台灣國產直播平台，讓任何人都能輕輕鬆鬆做直播節目，並支援跨平台觀看。其背後的 infrastructure 目前也以 PaaS 的方式 (straas.io) 提供服務給有 OTT 需求的客戶。

**講者介紹:**

Browny 曾任職於 HTC 以及多家新創公司，電腦視覺 / REST 服務開發 / 大型系統架構均有涉獵，目前專注於 Microservices 系統架構


- Dcard Tommy Chen - REST API 和 gRPC 的協奏曲 [[Slide](slides)], [[Video](https://youtu.be/cWcLFpl0K8o)]

Dcard 的 Tommy 來分享如何讓 REST API 和 gRPC 並行使用．

Tommy will share how to combine their experience REST API with gRPC.

**公司介紹:**

Dcard 一個專注於匿名的大學生交流平台, 每天為你配對一位大學朋友

**講者介紹:**

Tommy：從前端墜入後端的全端工程師，熱愛鑽研新語言，目前的新歡是 Go。


### Lightning Talk

-  toomore - Porting grs to gogrs (from Python to Go) [[Slide](https://docs.google.com/presentation/d/1uJqPdH2PA0BceBpRHXwIigeFu_mDSeXop06rTjDO1XM/edit?usp=sharing)], [[Video](https://youtu.be/RHdcVyumpO0)]
-  Dcard Even Chang - Using Go to interact with Instagram private API [[Slide](https://drive.google.com/open?id=0B6zCZUZLyeo6R29UYTBrajhzYTA)], [[Video](https://youtu.be/tFPFX32J-g0)]

