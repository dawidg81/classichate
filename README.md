ClassicHate is a Classic Minecraft-like custom client compatible with CSP and CPE. Some of the code is being forked from ClassiCube e.g. 3d renderer.

Idea by Ludinko23

How to build:
```
g++ -c *.c
g++ *.o -o classichate
```
(I have no clue.)

Please be aware of these compilation errors if you are building from source in Android with architecture aarch64:
```
Graphics_GL2.c:13:10: fatal error: '../misc/opengl/GLCommon.h' file not found
   13 | #include "../misc/opengl/GLCommon.h"
      |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~
1 error generated.
SSL.c:7:10: fatal error: '../third_party/bearssl/bearssl.h' file not found
    7 | #include "../third_party/bearssl/bearssl.h"
      |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1 error generated.
SystemFonts.c:290:10: fatal error: 'freetype/ft2build.h' file not found
  290 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
In file included from Window_Android.c:3:
./_WindowBase.h:107:10: fatal error: 'EGL/egl.h' file not found
  107 | #include <EGL/egl.h>
      |          ^~~~~~~~~~~
1 error generated.
_autofit.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_cff.c:23:10: fatal error: 'freetype/ft2build.h' file not found
   23 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_ftbase.c:20:10: fatal error: 'freetype/ft2build.h' file not found
   20 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_ftbitmap.c:20:10: fatal error: 'freetype/ft2build.h' file not found
   20 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_ftglyph.c:32:10: fatal error: 'freetype/ft2build.h' file not found
   32 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_ftinit.c:41:10: fatal error: 'freetype/ft2build.h' file not found
   41 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_ftsynth.c:20:10: fatal error: 'freetype/ft2build.h' file not found
   20 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_psaux.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_pshinter.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_psmodule.c:20:10: fatal error: 'freetype/ft2build.h' file not found
   20 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_sfnt.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_smooth.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_truetype.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
_type1.c:21:10: fatal error: 'freetype/ft2build.h' file not found
   21 | #include "freetype/ft2build.h"
      |          ^~~~~~~~~~~~~~~~~~~~~
1 error generated.
```
(Nothing weird in the errors, it is just not an Android application)
