Ensure that ImageMagick is installed:

```sh
brew install ImageMagick
```

Then run the command below from this directory to re-create the animation:

```sh
convert -delay 100 $(ls *.png | sort -V) out.gif
```

The `-delay 100` flag adds a 100 millisecond pause between each frame.

I originally read about this in [a StackOverflow answer](https://stackoverflow.com/a/65388750).
