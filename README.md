A short script that iterates your Pinboard.in bookmarks, deleting
shortened t.co, bit.ly, and other shortened URLS, and replacing them
with fully resolved, unshortened URLs.

```bash
npm install --global unshorten-pinboard-urls
PINBOARD_TOKEN="..." unshorten-pinboard-urls
```

Works great as a cron job:

```cron
# M  H    DOM  M  DOW  Command
  0  */4  *    *  *    unshorten-pinboard-urls >/dev/null 2>&1
```
