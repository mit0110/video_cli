# video_cli
CLI for common ffmpeg commands that I use all the time. Not intended for other people to use but take what you want.


### Usage

```
videocli command

Commands:
  cut  <input file>       cut video
  *         Help
```

#### Cut

```
Usage:
  cut <input_file> [--o <output_file>] [--p <extra_params>]
```
Cuts a video file `<input_file>` using the same audio and video codec.
If `<output_file>` is not present, the output is saved.
with the same name and extension as input_file, followed by `_cut`.
Example:
  the output of cut `../input.mp4` will be saved as `../input_cut.mp4`

`<extra_params>` are directly passed to `ffmpeg` command.
