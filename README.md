# rtmp-bench
rtmp-play / rtmp-publish load test tool.

## install

```
npm i rtmp-bench -g
```

## Usage

Create 1000 play instances
```
rtmp-bench -r rtmp://127.0.0.1/live/stream -c 1000
```

Create 100 publish instances
```
rtmp-bench -f video.flv -r rtmp://127.0.0.1/live/stream -c 100
```
> publish to stream: rtmp://127.0.0.1/live/stream_0 ~ rtmp://127.0.0.1/live/stream_99

## Help
```
rtmp-bench -r rtmp://127.0.0.1/live/stream -c 1000
rtmp-bench -f video.flv -r rtmp://127.0.0.1/live/stream -c 100
  rtmp-bench -h // print help information
  rtmp-bench -f // Publish a stream with a FLV file input
  rtmp-bench -r // The load test url for each client to play or publish
  rtmp-bench -c // The concurrency client to start to request. defaut: 1
  rtmp-bench -d // print log
```