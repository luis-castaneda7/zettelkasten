# golang-serialization

tags in golang can be used for serialization. similar to 
springs @JsonProperty("label").

example:
```go
func main() {
    type T struct {
       F1 int `json:"f_1"`
       F2 int `json:"f_2,omitempty"`
       F3 int `json:"f_3,omitempty"`
       F4 int `json:"-"`
    }
    t := T{1, 0, 2, 3}
    b, err := json.Marshal(t)
    if err != nil {
        panic(err)
    }
    fmt.Printf("%s\n", b) // {"f_1":1,"f_3":2}
}

```

#searilizatoin #json #golang #tags
