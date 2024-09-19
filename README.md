### Go HTMX Websockets example

Video: https://youtu.be/fBDUn7b9plw

In this video I create a sample modern web application that uses WebSockets in Golang and HTMX to display an autoupdating Hardware Monitor showing data about what is happening on the device.

![image](https://github.com/sigrdrifa/go-htmx-websockets-example/assets/83576392/91314043-10a3-41da-95d1-5a3c5f41bc50)



### Run in local
in the project root you need run 
```
go run cmd/main.go
```
you need run in root because in the cmd/main.go code it use 
```
	s.mux.Handle("/", http.FileServer(http.Dir("./htmx")))

```
otherwise the path is not correct and you will get error 
```
404 page not found 
```