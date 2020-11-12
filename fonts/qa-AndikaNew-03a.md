## Fontbakery report

Fontbakery version: 0.7.31

<details>
<summary><b>[9] AndikaNewBasic-Bold.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---

Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.


</pre>

* 🔥 **FAIL** Missing required codepoints: 0x2074 (SUPERSCRIPT FOUR) and 0x2215 (DIVISION SLASH) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---

An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;


</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright (c) 2004-2015, sil international (http://scripts.sil.org), "

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---

A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.

The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.

Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;


Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.

When in doubt, please choose OFL for new font projects.


</pre>

* 🔥 **FAIL** Font lacks NameID 13 (LICENSE DESCRIPTION). A proper licensing entry must be set. [code: missing]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Copyright notices match canonical pattern in fonts</summary>

* [com.google.fonts/check/font_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/font_copyright)

* 🔥 **FAIL** Name Table entry: Copyright notices should match a pattern similar to: "Copyright 2019 The Familyname Project Authors (git url)"
But instead we have got:
"Copyright (c) SIL International, 2004-2015." [code: bad-notice-format]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: fi	Contours detected: 2	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking with ots-sanitize.</summary>

* [com.google.fonts/check/ots](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ots)

* ⚠ **WARN** ots-sanitize passed this file, however warnings were printed:

ERROR: Silf: SILSub: passOffset check failed
ERROR: Silf: Failed to read tables[0]
ERROR: Dropping all Graphite tables
ERROR: Feat: Discarding Graphite table
ERROR: Table discarded
ERROR: Glat: Discarding Graphite table
ERROR: Table discarded
ERROR: Gloc: Discarding Graphite table
ERROR: Table discarded
ERROR: Silf: Discarding Graphite table
ERROR: Table discarded
ERROR: Sill: FeatureDefn: Required Feat table is missing
ERROR: Sill: Failed to read a LangFeatureSetting
ERROR: Table discarded


</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class)</summary>

* [com.google.fonts/check/gdef_spacing_marks](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_spacing_marks)
<pre>--- Rationale ---

Glyphs in the GDEF mark glyph class should be non-spacing.
Spacing glyphs in the GDEF mark glyph class may have incorrect anchor
positioning that was only intended for building composite glyphs during design.


</pre>

* ⚠ **WARN** The following spacing glyphs may be in the GDEF mark glyph class by mistake:
	 uni031B [code: spacing-mark-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class</summary>

* [com.google.fonts/check/gdef_mark_chars](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_mark_chars)
<pre>--- Rationale ---

Mark characters should be in the GDEF mark glyph class.


</pre>

* ⚠ **WARN** The following mark characters could be in the GDEF mark glyph class:
	 U+035E and U+035F [code: mark-chars]

</details>
<details>
<summary>⚠ <b>WARN:</b> Does GPOS table have kerning information?</summary>

* [com.google.fonts/check/gpos_kerning_info](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gpos.html#com.google.fonts/check/gpos_kerning_info)

* ⚠ **WARN** GPOS table lacks kerning information. [code: lacks-kern-info]

</details>
<br>
</details>
<details>
<summary><b>[9] AndikaNewBasic-BoldItalic.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---

Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.


</pre>

* 🔥 **FAIL** Missing required codepoints: 0x2074 (SUPERSCRIPT FOUR) and 0x2215 (DIVISION SLASH) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---

An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;


</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright (c) 2004-2015, sil international (http://scripts.sil.org), "

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---

A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.

The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.

Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;


Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.

When in doubt, please choose OFL for new font projects.


</pre>

* 🔥 **FAIL** Font lacks NameID 13 (LICENSE DESCRIPTION). A proper licensing entry must be set. [code: missing]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Copyright notices match canonical pattern in fonts</summary>

* [com.google.fonts/check/font_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/font_copyright)

* 🔥 **FAIL** Name Table entry: Copyright notices should match a pattern similar to: "Copyright 2019 The Familyname Project Authors (git url)"
But instead we have got:
"Copyright (c) SIL International, 2004-2015." [code: bad-notice-format]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: fi	Contours detected: 2	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking with ots-sanitize.</summary>

* [com.google.fonts/check/ots](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ots)

* ⚠ **WARN** ots-sanitize passed this file, however warnings were printed:

ERROR: Silf: SILSub: passOffset check failed
ERROR: Silf: Failed to read tables[0]
ERROR: Dropping all Graphite tables
ERROR: Feat: Discarding Graphite table
ERROR: Table discarded
ERROR: Glat: Discarding Graphite table
ERROR: Table discarded
ERROR: Gloc: Discarding Graphite table
ERROR: Table discarded
ERROR: Silf: Discarding Graphite table
ERROR: Table discarded
ERROR: Sill: FeatureDefn: Required Feat table is missing
ERROR: Sill: Failed to read a LangFeatureSetting
ERROR: Table discarded


</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class)</summary>

* [com.google.fonts/check/gdef_spacing_marks](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_spacing_marks)
<pre>--- Rationale ---

Glyphs in the GDEF mark glyph class should be non-spacing.
Spacing glyphs in the GDEF mark glyph class may have incorrect anchor
positioning that was only intended for building composite glyphs during design.


</pre>

* ⚠ **WARN** The following spacing glyphs may be in the GDEF mark glyph class by mistake:
	 uni031B [code: spacing-mark-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class</summary>

* [com.google.fonts/check/gdef_mark_chars](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_mark_chars)
<pre>--- Rationale ---

Mark characters should be in the GDEF mark glyph class.


</pre>

* ⚠ **WARN** The following mark characters could be in the GDEF mark glyph class:
	 U+035E and U+035F [code: mark-chars]

</details>
<details>
<summary>⚠ <b>WARN:</b> Does GPOS table have kerning information?</summary>

* [com.google.fonts/check/gpos_kerning_info](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gpos.html#com.google.fonts/check/gpos_kerning_info)

* ⚠ **WARN** GPOS table lacks kerning information. [code: lacks-kern-info]

</details>
<br>
</details>
<details>
<summary><b>[9] AndikaNewBasic-Italic.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---

Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.


</pre>

* 🔥 **FAIL** Missing required codepoints: 0x2074 (SUPERSCRIPT FOUR) and 0x2215 (DIVISION SLASH) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---

An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;


</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright (c) 2004-2015, sil international (http://scripts.sil.org), "

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---

A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.

The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.

Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;


Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.

When in doubt, please choose OFL for new font projects.


</pre>

* 🔥 **FAIL** Font lacks NameID 13 (LICENSE DESCRIPTION). A proper licensing entry must be set. [code: missing]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Copyright notices match canonical pattern in fonts</summary>

* [com.google.fonts/check/font_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/font_copyright)

* 🔥 **FAIL** Name Table entry: Copyright notices should match a pattern similar to: "Copyright 2019 The Familyname Project Authors (git url)"
But instead we have got:
"Copyright (c) SIL International, 2004-2015." [code: bad-notice-format]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: fi	Contours detected: 2	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking with ots-sanitize.</summary>

* [com.google.fonts/check/ots](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ots)

* ⚠ **WARN** ots-sanitize passed this file, however warnings were printed:

ERROR: Silf: SILSub: passOffset check failed
ERROR: Silf: Failed to read tables[0]
ERROR: Dropping all Graphite tables
ERROR: Feat: Discarding Graphite table
ERROR: Table discarded
ERROR: Glat: Discarding Graphite table
ERROR: Table discarded
ERROR: Gloc: Discarding Graphite table
ERROR: Table discarded
ERROR: Silf: Discarding Graphite table
ERROR: Table discarded
ERROR: Sill: FeatureDefn: Required Feat table is missing
ERROR: Sill: Failed to read a LangFeatureSetting
ERROR: Table discarded


</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class)</summary>

* [com.google.fonts/check/gdef_spacing_marks](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_spacing_marks)
<pre>--- Rationale ---

Glyphs in the GDEF mark glyph class should be non-spacing.
Spacing glyphs in the GDEF mark glyph class may have incorrect anchor
positioning that was only intended for building composite glyphs during design.


</pre>

* ⚠ **WARN** The following spacing glyphs may be in the GDEF mark glyph class by mistake:
	 uni031B [code: spacing-mark-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class</summary>

* [com.google.fonts/check/gdef_mark_chars](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_mark_chars)
<pre>--- Rationale ---

Mark characters should be in the GDEF mark glyph class.


</pre>

* ⚠ **WARN** The following mark characters could be in the GDEF mark glyph class:
	 U+035E and U+035F [code: mark-chars]

</details>
<details>
<summary>⚠ <b>WARN:</b> Does GPOS table have kerning information?</summary>

* [com.google.fonts/check/gpos_kerning_info](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gpos.html#com.google.fonts/check/gpos_kerning_info)

* ⚠ **WARN** GPOS table lacks kerning information. [code: lacks-kern-info]

</details>
<br>
</details>
<details>
<summary><b>[9] AndikaNewBasic-Regular.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---

Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.


</pre>

* 🔥 **FAIL** Missing required codepoints: 0x2074 (SUPERSCRIPT FOUR) and 0x2215 (DIVISION SLASH) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---

An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;


</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright (c) 2004-2015, sil international (http://scripts.sil.org), "

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---

A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.

The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.

Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;


Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.

When in doubt, please choose OFL for new font projects.


</pre>

* 🔥 **FAIL** Font lacks NameID 13 (LICENSE DESCRIPTION). A proper licensing entry must be set. [code: missing]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Copyright notices match canonical pattern in fonts</summary>

* [com.google.fonts/check/font_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/font_copyright)

* 🔥 **FAIL** Name Table entry: Copyright notices should match a pattern similar to: "Copyright 2019 The Familyname Project Authors (git url)"
But instead we have got:
"Copyright (c) SIL International, 2004-2015." [code: bad-notice-format]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: fi	Contours detected: 2	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking with ots-sanitize.</summary>

* [com.google.fonts/check/ots](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ots)

* ⚠ **WARN** ots-sanitize passed this file, however warnings were printed:

ERROR: Silf: SILSub: passOffset check failed
ERROR: Silf: Failed to read tables[0]
ERROR: Dropping all Graphite tables
ERROR: Feat: Discarding Graphite table
ERROR: Table discarded
ERROR: Glat: Discarding Graphite table
ERROR: Table discarded
ERROR: Gloc: Discarding Graphite table
ERROR: Table discarded
ERROR: Silf: Discarding Graphite table
ERROR: Table discarded
ERROR: Sill: FeatureDefn: Required Feat table is missing
ERROR: Sill: Failed to read a LangFeatureSetting
ERROR: Table discarded


</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class)</summary>

* [com.google.fonts/check/gdef_spacing_marks](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_spacing_marks)
<pre>--- Rationale ---

Glyphs in the GDEF mark glyph class should be non-spacing.
Spacing glyphs in the GDEF mark glyph class may have incorrect anchor
positioning that was only intended for building composite glyphs during design.


</pre>

* ⚠ **WARN** The following spacing glyphs may be in the GDEF mark glyph class by mistake:
	 uni031B [code: spacing-mark-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check mark characters are in GDEF mark glyph class</summary>

* [com.google.fonts/check/gdef_mark_chars](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gdef.html#com.google.fonts/check/gdef_mark_chars)
<pre>--- Rationale ---

Mark characters should be in the GDEF mark glyph class.


</pre>

* ⚠ **WARN** The following mark characters could be in the GDEF mark glyph class:
	 U+035E and U+035F [code: mark-chars]

</details>
<details>
<summary>⚠ <b>WARN:</b> Does GPOS table have kerning information?</summary>

* [com.google.fonts/check/gpos_kerning_info](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gpos.html#com.google.fonts/check/gpos_kerning_info)

* ⚠ **WARN** GPOS table lacks kerning information. [code: lacks-kern-info]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 16 | 20 | 341 | 24 | 281 | 0 |
| 0% | 2% | 3% | 50% | 4% | 41% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
