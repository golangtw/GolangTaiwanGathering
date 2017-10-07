# Golang Taiwan/Taipei Gathering #27

* 主辦：[Golang Taiwan](https://golang.kktix.cc/)
* 地點：Google 臺北台農 101 號會議室／臺北市信義區信義路五段 7 號 73 樓
* 時間：2017/09/26(Tue) 19:00 ~ 21:30  (UDT+8)
* 頁面：[Golang Taipei Gathering #27](https://golang.kktix.cc/events/gtg27)

## Speaker
### Dave Cheney

Software Engineer, Atlassian, Sydney, Australia

David is a programmer, public speaker, and author from Sydney, Australia. David has been a contributor to the Go project since February 2011 and is an organiser of GopherCon Denver. David currently works at Atlassian building Kubernetes infrastructure for their internal platform as a service.

## Talk
### High performance go without the event loop

Conventional wisdom suggests that the key to high performance servers are native threads, or more recently event loops. Neither solution is without downside. Threads carry a high overhead in terms of scheduling cost and memory footprint. Event loops lessen those costs, but introduce their own requirements for a complex callback driven style.

Go is a general purpose programming language in use in a wide range of domains and is well suited to writing network software. Go was introduced in 2009 with the explicit goal of helping programmers write programs that could solve problems of Google’s scale, and that means writing high performance servers.

This talk will focus on the features of the Go language and runtime environment, that allow programmers to write simple, high performance network services without resorting to native threads or event loop-driven callbacks

## Workshop
### Go tool trace

Dave will present a short version workshop how to trace your go code . 

As a complement to my conference talk I’ll be teaching a workshop on the Go execution tracer. This workshop follows on from my GolangUK presentation from last year and my High Performance Go workshop, and specifically focuses on the Go execution tracer,

## Slide
### Go Present Online
[Understanding the Go execution tracer](https://go-talks.appspot.com/github.com/davecheney/understanding-the-execution-tracer/understanding-the-execution-tracer.slide#1)

### Go Present Source Code
github.com/davecheney/[understanding-the-execution-tracer](https://github.com/davecheney/understanding-the-execution-tracer)

## Video（Low Resolution）
### 2017/09/26 19:30 GTG#27 - Dave Cheney: High performance go without the event loop

- [Part01](https://youtu.be/O_1basmpvVI)
- [Part02](https://youtu.be/Q0BTpNH9skY)


Thanks to Dave & Evan,