----------------------------------------------------------------------------
ColorMask v1.0 mod 8

PixInsight JavaScript Runtime API - PJSR Version 1.0

----------------------------------------------------------------------------
ColorMask.js - Released 2017-07-07T12:11:59Z

and later modified by Boris Emchenko (see below)

and by Mike Cranfield (see below)

----------------------------------------------------------------------------
Copyright (C) 2015-2017 Rick Stevenson. All rights reserved.

----------------------------------------------------------------------------


Redistribution and use in both source and binary forms, with or without
modification, is permitted provided that the following conditions are met:

1. All redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.

2. All redistributions in binary form must reproduce the above copyright
   notice, this list of conditions and the following disclaimer in the
   documentation and/or other materials provided with the distribution.

3. Neither the names "PixInsight" and "Pleiades Astrophoto", nor the names
   of their contributors, may be used to endorse or promote products derived
   from this software without specific prior written permission. For written
   permission, please contact info@pixinsight.com.

4. All products derived from this software, in any form whatsoever, must
   reproduce the following acknowledgment in the end-user documentation
   and/or other materials provided with the product:

   "This product is based on software from the PixInsight project, developed
   by Pleiades Astrophoto and its contributors (http://pixinsight.com/)."

   Alternatively, if that is where third-party acknowledgments normally
   appear, this acknowledgment must be reproduced in the product itself.

THIS SOFTWARE IS PROVIDED BY PLEIADES ASTROPHOTO AND ITS CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL PLEIADES ASTROPHOTO OR ITS
CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, BUSINESS
INTERRUPTION; PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; AND LOSS OF USE,
DATA OR PROFITS) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.

----------------------------------------------------------------------------


ColorMask v1.0 mod 8
 
Build a mask to select a color range in an image.
 
Copyright (C) 2015-2017 Rick Stevenson (rsj.stevenson@gmail.com). All rights reserved.
 
Special thanks to Adam Block for his advices and contribution.
 
Modifications made by Boris Emchenko (BE) and Mike Cranfield (MC):

 
1.0 mod 5c (MC) [2023/03/13]
   revised averge hue readings to reflect a circular mean
 
1.0 mod 5b (BE) [2023/03/13]
	added probe size element to average hue readings

1.0 mod 5a (MC) [2023/03/13]
	added STF checkbox for working with linear images

1.0 mod 4 (MC) [2023/03/08]
	interface enhancement - interactive image view added
	start, end and range hue setting via image view

1.0 mod 3 (BE) [2023/03/08]
	interface enhancement - hue wheel added
	displaying hue range on hue wheel

1.0 mod 2 (BE) [2023/02/27]
	execution on target view doesn't shows dialog
	min/max limits for Lum and Chrom are always min/max
	some bigfixes and code optimization

1.0 mod 1 (BE) [2023/02/11]
	engine: new hue calculatiions changed to hue from HSV color space
	engine: luminance & chrominance filter
	UI: hue range step (can be selected 30-60-90-120)
	UI: color buttons
	UI: buttons rearranged
	UI: minor design changes
	UI: saving settings between script calls
	Aux: store start/end hue values in PixelMath script for history explorer
