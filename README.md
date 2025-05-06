#### Task

You are provided with a gzipped JSON Lines file. Each line in the file represents an event where a user either starts or stops watching a stream. <br/>
Compute the total watch duration per user, then output it in ascending order in a human-readable format.


#### Details
Sample input:
```json lines
{"time":"2025-01-22 20:26:25.244","action":"stream_start","user":"🦐"}
{"time":"2025-01-22 20:32:27.827","action":"stream_start","user":"🐳"}
{"time":"2025-01-22 20:32:37.250","action":"stream_start","user":"🐃"}
{"time":"2025-01-22 20:34:31.353","action":"stream_stop","user":"🐃"}
{"time":"2025-01-22 20:39:47.454","action":"stream_stop","user":"🦐"}
{"time":"2025-01-22 20:40:01.013","action":"stream_stop","user":"🐳"}
```
* `action` can be either `stream_start` or `stream_stop`
* inputs are sorted by time in ascending order
* for each user there is always a `stream_start` before a `stream_stop`, every `stream_start` has a `stream_stop`.