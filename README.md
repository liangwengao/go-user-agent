# go-user-agent
Gets the "OSName" or "BrowserName" for USER_AGENT

[![License](https://img.shields.io/github/license/wenlng/go-user-agent.svg)](https://github.com/wenlng/go-user-agent/blob/master/LICENSE)
[![Version](https://img.shields.io/github/tag/wenlng/go-user-agent.svg)](https://github.com/wenlng/go-user-agent/releases)
[![Go Report Card](https://goreportcard.com/badge/github.com/wenlng/go-user-agent)](https://goreportcard.com/report/github.com/wenlng/go-user-agent)
[![GoDoc](https://godoc.org/github.com/wenlng/go-user-agent?status.svg)](https://godoc.org/github.com/wenlng/go-user-agent)

- Installation of proxy go module in China
>
>>GoProxy https://github.com/goproxy/goproxy.cn
>
>>AliProxy： https://mirrors.aliyun.com/goproxy/
>
>>OfficialProxy： https://goproxy.io/
>
>>ChinaProxy：https://goproxy.cn
>
>>Other：https://gocenter.io

#### Set Proxy of go module 
- Window
```shell script
set GO111MODULE=on
set GOPROXY=https://goproxy.io,direct

### The Golang 1.13+ can be executed directly
go env -w GO111MODULE=on
go env -w GOPROXY=https://goproxy.io,direct
```
- Linux or Mac
```shell script
vi vim ~/.bash_profile
export GO111MODULE=on
export GOPROXY=https://goproxy.io,direct
source ~/.bash_profile
```

#### 安装模块
```
go get -u github.com/wenlng/go-user-agent
```

#### 获取系统名称
```
import "github.com/wenlng/go-user-agent"

func main(){
    userAgent := "Mozilla/5.0 {Macintosh; Intel Mac OS X 10.6.8; U; en) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36 OPR/26.0.1656.60"
    name := useragent.GetOsName(userAgent)
    fmt.Println(name)   // "Windows 10"
}

```

#### 获取浏览器名称
```
import "github.com/wenlng/go-user-agent"

func main(){
    userAgent := "Mozilla/5.0 {Macintosh; Intel Mac OS X 10.6.8; U; en) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36 OPR/26.0.1656.60"
    name := useragent.GetBrowserName(userAgent)
    fmt.Println(name)   // "Chrome/39.0.2171.95"
}

```

IT技术网站: [witkeycode.com](witkeycode.com)

<div align="center">
    <img src="http://47.104.180.148/reward-support.png" alt="Reward Support">
</div>

## LICENSE
    MIT
