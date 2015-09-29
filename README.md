*** Custome golang pkg net/http 

- use for read manga on web browser 

- only use http.ListenAndServe(":8080", http.FileServer(http.Dir("./"))) in main function

```Go
package main

import (
        "log"
        "github.com/neverlock/manga_net/http"
)


func main() {
        log.Println("Service at :8080")
        log.Fatal(http.ListenAndServe(":8080", http.FileServer(http.Dir("./"))))
}
```
