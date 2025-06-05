#### Task

You are provided with a gzipped JSON Lines file. Each line in the file represents an event where a user either starts or stops watching a stream. <br/>

- Step 1: compute the total watch time<br/>
- Step 2: output in human-readable and in ascending order the watch time per user


#### Details
Sample input:
```json lines
{"time":"2025-01-22T20:26:25.244Z","action":"stream_start","user":"🦐"}
{"time":"2025-01-22T20:32:27.827Z","action":"stream_start","user":"🐳"}
{"time":"2025-01-22T20:32:37.250Z","action":"stream_start","user":"🐃"}
{"time":"2025-01-22T20:34:31.353Z","action":"stream_stop","user":"🐃"}
{"time":"2025-01-22T20:39:47.454Z","action":"stream_stop","user":"🦐"}
{"time":"2025-01-22T20:40:01.013Z","action":"stream_stop","user":"🐳"}
```
* `action` can be either `stream_start` or `stream_stop`
* inputs are sorted by time in ascending order
* for each user there is always a `stream_start` before a `stream_stop`, every `stream_start` has a `stream_stop`.