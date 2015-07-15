# CmdFolder
CmdFolder is a wrapper around pseudo-terminal-go that allows the creation of mock terminal environments with "folders" that the user can `cd` into and "commands" that may reside in these folders.

## Usage

```
func main() {
	folder := New()
	folder.AddCommand("do", dostuff)
	folder.Run()
}

func dostuff(_ string) {
	fmt.Println("STUFF GOT DID")
}
```

* Note: subfolders haven't happened yet.
