

# ezapi
`import "github.com/paijerry/ezapi"`

* [Overview](#pkg-overview)
* [Index](#pkg-index)

## <a name="pkg-overview">Overview</a>
Package ezapi can help you call api easier




## <a name="pkg-index">Index</a>
* [type EzAPI](#EzAPI)
  * [func New() *EzAPI](#New)
  * [func (ez *EzAPI) Do(method string) (rspn Rspn, err error)](#EzAPI.Do)
  * [func (ez *EzAPI) Form(form url.Values) *EzAPI](#EzAPI.Form)
  * [func (ez *EzAPI) FormData(form url.Values) *EzAPI](#EzAPI.FormData)
  * [func (ez *EzAPI) Header(header http.Header) *EzAPI](#EzAPI.Header)
  * [func (ez *EzAPI) JSON(body []byte) *EzAPI](#EzAPI.JSON)
  * [func (ez *EzAPI) URL(url string) *EzAPI](#EzAPI.URL)
  * [func (ez *EzAPI) URLQuery(urlquery url.Values) *EzAPI](#EzAPI.URLQuery)
* [type Rspn](#Rspn)


#### <a name="pkg-files">Package files</a>
[ezapi.go](/src/github.com/paijerry/ezapi/ezapi.go) 






## <a name="EzAPI">type</a> [EzAPI](/src/target/ezapi.go?s=181:315#L4)
``` go
type EzAPI struct {
    // contains filtered or unexported fields
}
```
EzAPI is the main struct of this package







### <a name="New">func</a> [New](/src/target/ezapi.go?s=457:474#L21)
``` go
func New() *EzAPI
```
New create an api object





### <a name="EzAPI.Do">func</a> (\*EzAPI) [Do](/src/target/ezapi.go?s=1509:1566#L75)
``` go
func (ez *EzAPI) Do(method string) (rspn Rspn, err error)
```
Do the http request




### <a name="EzAPI.Form">func</a> (\*EzAPI) [Form](/src/target/ezapi.go?s=848:893#L39)
``` go
func (ez *EzAPI) Form(form url.Values) *EzAPI
```
Form add form("application/x-www-form-urlencoded") by a url.Value object ("Content-Type", "application/x-www-form-urlencoded")




### <a name="EzAPI.FormData">func</a> (\*EzAPI) [FormData](/src/target/ezapi.go?s=1005:1054#L45)
``` go
func (ez *EzAPI) FormData(form url.Values) *EzAPI
```
FormData add formdata by a url.Value object (no Content-Type)




### <a name="EzAPI.Header">func</a> (\*EzAPI) [Header](/src/target/ezapi.go?s=539:589#L26)
``` go
func (ez *EzAPI) Header(header http.Header) *EzAPI
```
Header add head by a http.Header object




### <a name="EzAPI.JSON">func</a> (\*EzAPI) [JSON](/src/target/ezapi.go?s=1202:1243#L57)
``` go
func (ez *EzAPI) JSON(body []byte) *EzAPI
```
JSON add json of []byte




### <a name="EzAPI.URL">func</a> (\*EzAPI) [URL](/src/target/ezapi.go?s=1417:1456#L69)
``` go
func (ez *EzAPI) URL(url string) *EzAPI
```
URL set url




### <a name="EzAPI.URLQuery">func</a> (\*EzAPI) [URLQuery](/src/target/ezapi.go?s=1309:1362#L63)
``` go
func (ez *EzAPI) URLQuery(urlquery url.Values) *EzAPI
```
URLQuery add urlquery into url




## <a name="Rspn">type</a> [Rspn](/src/target/ezapi.go?s=349:428#L14)
``` go
type Rspn struct {
    Header     http.Header
    Body       string
    StatusCode int
}
```
Rspn - contains response data














- - -
Generated by [godoc2md](http://godoc.org/github.com/davecheney/godoc2md)
