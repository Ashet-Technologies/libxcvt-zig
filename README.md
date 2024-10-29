# libxcvt-zig

A port of the [libxcvt 0.1.2](https://www.x.org/archive//individual/lib/libxcvt-0.1.2.tar.xz) to Zig.

## Usage

**Zig Version:** 0.13.0

```zig
const cvt = @import("cvt");

test {
    const mode = cvt.compute(.{
        .width = 800,
        .height = 600,
        .refresh_rate = 60.0,
    });

    std.debug.print("MODE = {}\n", .{mode});
}
```
