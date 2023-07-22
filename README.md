# Logger

Simple helper to reuse the log-to-file function in the rest of our libs.

## Usage

- Init the logger in your main function

```go
import (github.com/bocha-io/logger)
...

// Log to file
file := logger.LogToFile("indexerlogs.txt")
defer file.Close()
```

- Call the logger from any file

```go
logger.LogInfo("hello from log")
```
