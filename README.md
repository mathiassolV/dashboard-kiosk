# dashboard-kiosk

Site rotation for the office dashboard (Raspberry Pi kiosk).

Edit [`sites.conf`](sites.conf) and commit. The Pi picks up the change
within about 5-10 minutes (it checks every 5 minutes; GitHub caches raw
files for a few minutes).

```
30m https://google.com
2m  https://bing.com
```

Each line is `<duration> <url>`: `45s`, `30m`, `2h`, or a plain number of
seconds. Sites are shown top to bottom and then loop.

This repo is public: don't put internal URLs here that must stay secret.
