## Golang Taiwan/Taipei Gathering #20

### Time

#### 2017/01/24(Tue) 19:30 ~ 21:40  (UDT+8)

### Resgistration Page:

#### [Regstration Info](http://golang.kktix.cc/events/gtg20)

### Talks

- 19:30 ~ 20:00 Astra IOT - Tommy: Design the high-concurrency and multi-channel worker using AWS-SQS in Golang [[slide](https://docs.google.com/presentation/d/1ApeCwGggO8qBIZvfSOSnKjpoHHmkI62VkQ3CWlbCYis/edit?usp=sharing)] [[video](https://youtu.be/ihw57YKq_T0?list=PLmQD9LZfhqmdQvM_EZmWSHvDNyrHEQ4a8)]


分享如何利用AWS-SQS的特性，用golang實作一個高併發、多通道的Worker，且適用於多人開發的基礎架構，同時降低系統層與應用層間的耦合性

Tommy will share how to take advantage of AWS-SQS features to implement a high-concurrency and multi-channel worker by golang,
then design the infrastructure for cooperation development ,  reducing the coupling between the system layer and the application layer


- 20:10 ~ 20:50 Umbo CV - Kakashi: etcd: a brief introduction  [[slide](https://docs.google.com/presentation/d/15mtcBSLVSqrX4-VntqhOwqtRw2Od9Hn6xHc2hfp0zV0/edit?usp=sharing)],[[video](https://youtu.be/uHskez_kbGk)]

etcd 是 CoreOS 公司用  golang 開發的一個 distributed key-value system，分享如何使用 etcd 還有 etcd 適用於什麼樣的場景。

etcd: a brief introduction. etcd is a golang based distributed key-value system which implement by CoreOS.
Kakashi will introduce how to use etcd and where we could use etcd.


- 21:00 ~ 21:40 Bitmark- Bitmark: the property system for the digital environment [[slide](slide)]

Abstract:
This talk will explain why data property rights are needed. And explain, in-depth the technical details of the Bitmark system. For example: Bitmark’s blockchain is an independent chain, optimized for storing property titles, or bitmarks, and does not have its own internal currency (transaction fees are in bitcoin). The peer-to-peer network is written in Golang and uses the ZeroMQ distributed messaging library. Consensus is secured using argon2 hashing (proof-of-work). Chain of ownership is immutable and digitally signed; long-term, post-quantum signatures (SPHINCS-256) are supported. Digital properties are transferred using the BitTorrent protocol such that only owners can seed and download. 

About Bitmark:
Bitmark creates specialized blockchain technology to convert personal data into property that can be sold, licensed or transferred peer-to-peer. Personal data will be a massive asset class in the emerging data economy. Our property system for the digital environment enables individuals to establish ownership claims for personal data akin to how land registrars track land titles or patent offices track patents.
 
Speaker Bios:
Sean Moss-Pultz, CEO, is an expert in developing technology for consumer electronics and Internet services, especially blockchain related projects. Prior to Bitmark Inc., he was a senior executive for EMQ Limited, a financial technology startup. Recognized as a pioneer of open-source hardware, Moss-Pultz launched and was CEO of Openmoko Inc., the first open-source phone and a precursor to iPhone and Android smartphones. He has led his dedicated team of specialists across a number of successful projects who have now joined him at Bitmark Inc. Moss-Pultz holds bachelor’s degrees in mathematics and physics from UC San Diego. 
 
Christopher Hall, Head of Engineering, is an embedded software programmer accomplished in many of the dominant programming languages of the last 35 years. As one of the foremost experts in Open Source OS and blockchain technology, he’s built Bitmark’s open-source blockchain as well as designing microcontroller firmware and a range of embedded devices. Prior to Bitmark Inc., he worked with Sean Moss-Pultz to lead development of Openmoko and Intelligencia.