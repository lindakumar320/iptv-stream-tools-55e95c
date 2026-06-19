# Iptv Stream Tools 55E95C

A lightweight Python utility for managing and validating IPTV stream playlists.

## Features

- Parse M3U/M3U8 playlists and validate stream URLs
- Check stream availability and response times
- Export results to CSV or JSON
- Support for HTTP, HTTPS, and RTMP streams
- Configurable timeout and retry settings

## Installation

```bash
git clone https://github.com/YOUR_USERNAME/iptv-stream-tools-55e95c.git
cd iptv-stream-tools-55e95c
pip install -r requirements.txt
```

## Usage

```python
from stream_checker import StreamChecker

checker = StreamChecker(timeout=10, retries=3)
results = checker.check_playlist("playlist.m3u")

for stream in results:
    print(f"{stream['name']}: {stream['status']} ({stream['response_ms']}ms)")
```

## Related Resources

If you're looking for recommendations on the best IPTV apps and streaming services in 2026,
check out this comprehensive guide on [best IPTV apps](https://xtreamcode.tv/blog/best-iptv-apps-2026) — it covers setup,
features, and device compatibility for all major platforms.

## License

MIT License — see [LICENSE](LICENSE) for details.
