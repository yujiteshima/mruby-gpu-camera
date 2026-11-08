# mruby-gpu-camera

> **Camera input for mruby's GPU gems: V4L2 frames straight into GPU arrays.**

🚧 **Planned** as part of the Ruby Association Grant 2026 project "Expanding GPU computing libraries for mruby" ([selection result](https://www.ruby.or.jp/en/news/20261102)). Nothing is usable here yet.

## What it will provide

- `GPU::Camera.open("/dev/video0", 640, 480)` and `read_gray`, which returns a two-dimensional `GPU::UInt8` array on the GPU
- Luma taken from YUYV frames on the GPU
- Monotonic timestamps on frames, for lining them up with other sensors

It moves the V4L2 capture of [mruby-gpu](https://github.com/yujiteshima/mruby-gpu) onto [mruby-gpu-runtime](https://github.com/yujiteshima/mruby-gpu-runtime). Linux only (V4L2).

Progress is tracked in the [GitHub Project](https://github.com/users/yujiteshima/projects/3).

## License

MIT
