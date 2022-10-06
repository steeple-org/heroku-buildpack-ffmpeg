# heroku-buildpack-ffmpeg

This Heroku buildpack installs a static build of FFmpeg.

It does not require compiling the FFmpeg source code first.

## Usage

```sh
heroku buildpacks:add https://github.com/steeple-org/heroku-buildpack-ffmpeg.git
```

## Testing

```sh
# setup
mkdir -p private/tmp

# once the next command done, manually inspect the content of private/tmp
bin/compile "$(pwd)/private/tmp"

# teardown
rm -r private/tmp
```

## History

This project used to be a fork of https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest.
