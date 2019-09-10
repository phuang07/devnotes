# Logs

```
// Show results
zgrep -R 'get_events' logs/* | ag '06/Aug'

// Show # of results
zgrep -R 'get_events' logs/* | ag '06/Aug' | wc -l
```
