# Golang Taiwan/Taipei Gathering #26

* 主辦: [COSCUP 2017](https://coscup.org/2017/#/)
* 地點: 台大社科院
* 時間: 2017/08/06(Sun) 13:30 ~ 16:45  (UDT+8)

## 主題

### 鮑承佑 -- Go,Java,C# 的 gRPC + Protocol Buffer 共同大亂鬥 [[slides](https://www.slideshare.net/ChenYuPao/go-java-cgrpcprotocol-buffer)][[video](https://www.youtube.com/watch?v=4EWAatxGS6Q&t=23200)]

介紹 Google 的 [gRPC](http://www.grpc.io) 和 [Protocol Buffer](developers.google.com/protocol-buffers ) 在跨程式語言的互動應用

### 郭學聰 -- Marshal 不給你的, 自己來 [[slides](https://hackmd.io/p/BkY59g9Bb#/)][[video](https://www.youtube.com/watch?v=4EWAatxGS6Q&t=18479)]

Golang 雖然有相當完整的 struct serialize 與 deserialize 功能。 但是在預設情形下，定義好 struct field 的資料型態，就等於確定了 serialize 後得到的資料格式。 這對於文字表示方式有多種方法的常用資料型態 (如 time.Time) 相當不方便。 雖然可以重新定義 field 型態，進而改變 struct field 的 serialize 方式。 但是對於相同資料型態，卻得在不同 struct 內產生不同的 serialized 資料的場合，依然相當不方便。 本 topic 將向 Golang 新手介紹如何修改 Marshal/Unmarshal method，讓不同 struct 內的同型態 field，能夠依需求 serialize 成不同的資料表示格式。

### 陳憶賢 -- GoLearn: 簡單利用 Go 語言處理機器學習 [[slides](https://github.com/frozenkp/COSCUP-2017/blob/master/slide.pdf)][[video](https://www.youtube.com/watch?v=4EWAatxGS6Q&t=20830)]

說到機器學習，大部分的人第一時間想到的必定是 python 的 scikit-learn，但實際上 Go 也有 Go 的解決方案，也就是 Golearn，結合了 Go 語言本身的速度以及並行，在效能方面或許更適合用在機器學習。此次將介紹幾個已經完成的 Model，並帶領各位使用 Golearn 以及幾個簡單的 model 實做機器學習。

### 林士翔 -- Dependency Injection in Go [[slides](https://speakerdeck.com/brownylin/dependency-injection-in-go)][[video](https://www.youtube.com/watch?v=4EWAatxGS6Q&t=25678)]

介紹 Dependency injection 的基本概念，及其帶來的優缺點。也實際以一套 open source 的 injection framework 說明其如何在專案中使用。- Introduction - What is DI - DI framework - facebookgo/inject - Conlusion

### appleboy -- 自架 Git 伺服器的選擇 Gitea [[slides](https://www.slideshare.net/appleboy/introduction-to-gitea-with-drone)][[video](https://www.youtube.com/watch?v=4EWAatxGS6Q&t=27452)][[post](https://blog.wu-boy.com/2017/08/2017-coscup-introduction-to-gitea-drone/)]

Gitea 是一個可自行託管的 Git 服務，用 Go 語言撰寫。它就像網路上常見的 GitHub、Bitbucket 或 GitLab 服務。最初版本是從 Gogs 而來並且重新命名為 Gitea。本議程會帶您瞭解什麼是 Gitea 及如何快速安裝在 DigitalOcean，並且搭配 Jenkins 或 Drone 等 CI/CD 服務來達成自動化測試及部署。
