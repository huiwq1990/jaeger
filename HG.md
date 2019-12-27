### BuildtinFormat

用于定义Span在网络传输中序列化方式。默认支持：TextMap，HTTPHeaders、Binary。
每一种方式需要实现的Write、Reader接口，为了方便开发，封装HTTPHeadersCarrier。



### Injector

tracer.go:NewTracer
会注册默认的注入器，

如果希望自己注册，使用config.Injector('dubbo',nil)


docker run --rm -it --link jaeger -p8080-8083:8080-8083 -e JAEGER_AGENT_HOST="jaeger" jaegertracing/example-hotrod:1.14 all


set GOPROXY=https://goproxy.io
set http_proxy=http://localhost:1080
set https_proxy=http://localhost:1080
dep ensure


set GOPROXY="https://goproxy.io"
go mod vendor


### agent调试

设置collector的地址
--reporter.tchannel.host-port 116.196.85.112:14267




### collector 调试
环境变量
CGO_ENABLED=0
SPAN_STORAGE_TYPE=memory
应用参数
--collector.zipkin.http-port=9411


GOOS=linux CGO_ENABLED=0 installsuffix=cgo go build -tags ui -o ./cmd/all-in-one/all-in-one  ./cmd/all-in-one/main.go


nohup ./jaeger-agent --reporter.tchannel.host-port localhost:14267 &
