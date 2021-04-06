# videocli

CLI for common ffmpeg commands that I use all the time. Not intended for other people to use but take what you want.


### Usage

```
videocli command

Commands:
  cut  <input file>       cut video
  *         Help
```

#### Cut

Cuts a video file `<input_file>` using the same audio and video codec.

Usage:
```
  cut <input_file> [--o <output_file>] [--p <extra_params>] [--d]
```

Options:
```
    --o <output_file>
        If not present, the output is saved with the same
        name and extension as `<input_file>`, followed by _cut.
        Example:
            the output of cut ../input.mp4 will be saved as ../input_cut.mp4

    --p <extra_params>
        String of params that is directly passed to ffmpeg command.
    --d
        Only prints ffmpeg command. For debug purposes.
```


#### Compress

Compress a video file `<input_file>` for web usage.

Usage:
```
  compress <input_file> [--o <output_file>] [--d]
```

Options:
```
    --o <output_file>
        If not present, the output is saved with the same
        name and extension as `<input_file>`, followed by _compress.
        Example:
            the output of compress ../input.mp4 will be saved as ../input_cut.mp4

    --d
        Only prints ffmpeg command. For debug purposes.
```
