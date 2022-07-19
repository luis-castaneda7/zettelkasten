# regex-golang

An example of using regex in go to replace any invalid characters with a blank

```go
func fixString(sentence string) bool {                                                                                                  
  reg, _ := regexp.Compile("[^a-zA-Z0-9]+")                                                                                             
                                                                                                                                        
  processedString := reg.ReplaceAllString(sentence, "")                                                                                 
                                                                                                                                        
  return isPalindrome(strings.ToLower(processedString))                                                                                 
}                                                                                                                                       

```

#golang #regex
