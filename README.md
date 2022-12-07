# Minimal Dependency Web Sunmap

An exercise in simplifying build and deploy of a Sunmap visualization.

- build without any tool installation:
use  cljs.jar  (ClojureScript 1.11.60  downloaded 2022 Nov 21)
```
$ java -cp "cljs.jar:src" cljs.main --optimizations advanced -c mnd-snmp.main
```
  - local test with included server and browser
```
$ java -cp "cljs.jar" cljs.main --serve
```

- deploy: push Git repo to GitHub repo where  GitHub Pages  enabled

```
...
$ git add   index.html  main.js  worldmap.jpg  worldmap_night.jpg
$ git commit -m "..."
$ git push -u origin main
```


## Credits

File  sunmap.cljs  is the same as  sunmap.clj  except for namespace change; it was translated or freely paraphrased from Java code in SkyviewCafe which carry the following notice:

    ```
    Copyright (C) 2000-2007 by Kerry Shetline, kerry@shetline.com.

    This code is free for public use in any non-commercial application. All
    other uses are restricted without prior consent of the author, Kerry
    Shetline. The author assumes no liability for the suitability of this
    code in any application.

    2007 MAR 31   Initial release as Sky View Cafe 4.0.36.
    ```

## Usage

Open the page  https://lrngquest.github.io/min-dep-websnmp/
a visualization of sunlit portion of Earth will appear, initialized at the UTC
 when the page was opened; as the countdown reaches 0 the image will update,
 the countdown will reset; and so on, continuing until the page is closed.

### Bugs
None known.



## License

Other than credited above:
Copyright © 2018-2022   L. E. Vandergriff

Distributed under the Eclipse Public License either version 1.0 or (at your option) any later version.

   ```
"Freely you have received, freely give."  Mt. 10:8
   ```
