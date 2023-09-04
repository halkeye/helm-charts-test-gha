COPS Book Server
================

You pretty much want to have a /books mount somewhere.

Right now I'm using:

```
extraVolumes:
  - name: books
    hostPath:
      path: /smb/odin/Books

extraVolumeMounts:
  - mountPath: /books
    name: books
    readOnly: true
```

But might change in the future
