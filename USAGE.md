<!-- Start SDK Example Usage -->
```go
package main

import (
	"context"
	templatesdk "github.com/speakeasy-sdks/template-sdk"
	"log"
	"net/http"
)

func main() {
	s := templatesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->