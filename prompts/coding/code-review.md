
# Code Review Prompt

## Prompt

"Please review the following Bash script and provide feedback on how it can be improved. The script is intended to back up a directory to a remote server using `rsync`.

```bash
#!/bin/bash

SRC='/path/to/source'
DEST='user@remote:/path/to/dest'

rsync -avz $SRC $DEST
```

Consider the following aspects:
- **Error Handling:** What happens if the `rsync` command fails? How can the script be made more robust?
- **Logging:** How can the script be modified to log the output of the `rsync` command to a file?
- **Readability:** Is the script easy to read and understand? How can it be improved?
- **Security:** Are there any security considerations to keep in mind? For example, how can we avoid hardcoding credentials in the script?
"
