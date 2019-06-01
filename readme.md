# GopherCon EU2019 Notes

## [Ultimate Go](https://github.com/ardanlabs/gotraining/blob/master/topics/courses/go/README.md) Workshop Takeaways

Review course materials, specifically:
 
* [Profiling](https://github.com/ardanlabs/gotraining/blob/master/topics/courses/go/tooling/README.md)
* [Data Semantics](https://github.com/ardanlabs/gotraining/blob/67e33a36da51d394b0fe6f925b8023e10a29878d/topics/go/language/methods/example5/example5.go)
* [Concurrency](https://github.com/ardanlabs/gotraining/blob/master/topics/courses/go/concurrency/README.md)

#### Guidelines

##### On data semantics (when to use value versus pointer semantics)

Don't mix value and pointer semantics in a function

Built-in types
Pass built-in types using value semantics
	Exception: we want nils, only then is it okay to use pointer semantics. Comment these instances

Value semantics safest way to do mutation

Reference types - arrays, slices, maps, interfaces, functions
Use value semantics to pass these around
	Exception: unless you're writing to it

##### Other 

Method receivers can be value or pointer - can call these in either way.

Use functions until it's not practical anymore, then use methods on a struct

Methods allow data to exhibit behaviour

Use var to always get a zero value
var u User 
vs
u:=User() may or may not give you a zero value

go routines - fan out pattern vs pooling

## Finding Dependable Go Packages

### Discovery 
* Ask Twitter 
* Google
* Github

###Evaluate 
1. License
2. Popularity - Stats on github - is it forked, depended on a lot, contributed to recently? 
3. Code quality - is documentation comprehensive, good tests, is it clear idiomatic Go code?
4. Upkeep - are the contributors well regarded, active? Do issues get responded to?
5. Indirect dependencies - check the package's packages!

###Maintenance 
* Stay up to date with packages
* Maybe contribute to them

The Go team is working on a site for discovering and evaluating packages.

## Distributed Tracing
[Jaegar Tracing](https://www.jaegertracing.io/)

![Distributed Tracing Example Diagram](distributed_tracing.jpg "Distributed Tracing Example Diagram")

## [How I write Go HTTP services after seven years](https://medium.com/statuscode/how-i-write-go-http-services-after-seven-years-37c208122831)

## Tools
* [GraphViz](http://graphviz.org/)

## Refactor Considerations
* get it working
* refactor, make interfaces where appropriate
* profile
* readability according to 4+-1 items working memory idea, things need to be in chunks

## Links

* [GoBridge](https://github.com/gobridge/about-us/blob/master/README.md)
* [Go Report Card](https://goreportcard.com/)
* [Golang Weekly (email newsletter)](https://golangweekly.com/issues/264)
* [Go Time Podcast](https://changelog.com/gotime)
* [r/golang](https://www.reddit.com/r/golang/)

## Non-Go Stuff

Learn
* JavaScript
* HTML
* CSS

Links
* [Spectre Bug](https://en.wikipedia.org/wiki/Spectre_(security_vulnerability)
* [Binary Tree](https://appliedgo.net/bintree/)
* [Hacker News](https://thehackernews.com/)

### JavaScript Recommendation

[VueJS](https://vuejs.org/)