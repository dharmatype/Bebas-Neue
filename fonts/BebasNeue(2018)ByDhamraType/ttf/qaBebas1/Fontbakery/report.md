## Fontbakery report

Fontbakery version: 0.7.10

<details>
<summary><b>[1] Family checks</b></summary>
<details>
<summary>⚠ <b>WARN:</b> Is the command `ftxvalidator` (Apple Font Tool Suite) available?</summary>

* [com.google.fonts/check/ftxvalidator_is_available](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ftxvalidator_is_available)
* ⚠ **WARN** ftxvalidator is not available.

</details>
<br>
</details>
<details>
<summary><b>[9] BebasNeue-Regular.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Substitute copyright, registered and trademark symbols in name table entries.</summary>

* [com.google.fonts/check/name/unwanted_chars](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/unwanted_chars)
* 🔥 **FAIL** NAMEID #0 contains symbols that should be replaced by '(c)'. [code: unwanted-chars]
* 🔥 **FAIL** NAMEID #0 contains symbols that should be replaced by '(c)'. [code: unwanted-chars]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Are there non-ASCII characters in ASCII-only NAME table entries?</summary>

* [com.google.fonts/check/name/ascii_only_entries](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/ascii_only_entries)
* 🔥 **FAIL** There are 2 strings containing non-ASCII characters in the ASCII-only NAME table entries. [code: non-ascii-strings]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Copyright notices match canonical pattern in fonts</summary>

* [com.google.fonts/check/font_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/font_copyright)
* 🔥 **FAIL** Name Table entry: Copyright notices should match a pattern similar to: "Copyright 2019 The Familyname Project Authors (git url)"
But instead we have got:
"Copyright © 2010 by Dharma Type." [code: bad-notice-format]
* 🔥 **FAIL** Name Table entry: Copyright notices should match a pattern similar to: "Copyright 2019 The Familyname Project Authors (git url)"
But instead we have got:
"Copyright © 2010 by Dharma Type." [code: bad-notice-format]

</details>
<details>
<summary>🔥 <b>FAIL:</b> PPEM must be an integer on hinted fonts.</summary>

* [com.google.fonts/check/integer_ppem_if_hinted](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/integer_ppem_if_hinted)
* 🔥 **FAIL** This is a hinted font, so it must have bit 3 set on the flags of the head table, so that PPEM values will be rounded into an integer value.

This can be accomplished by using the 'gftools fix-hinting' command.

# create virtualenvpython3 -m venv venv
# activate virtualenvsource venv/bin/activate
# install gftoolspip install git+https://www.github.com/googlefonts/tools [code: bad-flags]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 usWinAscent & usWinDescent.</summary>

* [com.google.fonts/check/family/win_ascent_and_descent](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/family/win_ascent_and_descent)
* 🔥 **FAIL** OS/2.usWinAscent value should be equal or greater than 912, but got 900 instead [code: ascent]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 Metrics match hhea Metrics.</summary>

* [com.google.fonts/check/os2_metrics_match_hhea](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/os2_metrics_match_hhea)
* 🔥 **FAIL** OS/2 sTypoAscender and hhea ascent must be equal. [code: ascender]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
* ⚠ **WARN** OS/2 VendorID value 'dhrm' is not a known registered id. You should set it to your own 4 character code, and register that code with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
* ⚠ **WARN** Even though unitsPerEm (1000) in this font is reasonable. It is strongly advised to consider changing it to 2000, since it will likely improve the quality of Variable Fonts by avoiding excessive rounding of coordinates on interpolations. [code: legacy-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uniF000	Contours detected: 0	Expected: 14
Glyph name: b	Contours detected: 3	Expected: 2
Glyph name: e	Contours detected: 1	Expected: 2
Glyph name: g	Contours detected: 1	Expected: 2 or 3
Glyph name: i	Contours detected: 1	Expected: 2
Glyph name: j	Contours detected: 1	Expected: 2
Glyph name: r	Contours detected: 2	Expected: 1
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: ae	Contours detected: 2	Expected: 3
Glyph name: egrave	Contours detected: 2	Expected: 3
Glyph name: eacute	Contours detected: 2	Expected: 3
Glyph name: ecircumflex	Contours detected: 2	Expected: 3
Glyph name: edieresis	Contours detected: 3	Expected: 4
Glyph name: eth	Contours detected: 3	Expected: 2
Glyph name: uniE0FF	Contours detected: 0	Expected: 7
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: emacron	Contours detected: 2	Expected: 3
Glyph name: ebreve	Contours detected: 2	Expected: 3
Glyph name: edotaccent	Contours detected: 2	Expected: 3
Glyph name: ecaron	Contours detected: 2	Expected: 3
Glyph name: gcircumflex	Contours detected: 2	Expected: 3 or 4
Glyph name: gbreve	Contours detected: 2	Expected: 3 or 4
Glyph name: gdotaccent	Contours detected: 2	Expected: 3 or 4
Glyph name: gcommaaccent	Contours detected: 2	Expected: 3 or 4
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: ij	Contours detected: 2	Expected: 3 or 4
Glyph name: oe	Contours detected: 2	Expected: 3
Glyph name: racute	Contours detected: 3	Expected: 2
Glyph name: rcommaaccent	Contours detected: 3	Expected: 2
Glyph name: rcaron	Contours detected: 3	Expected: 2
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: florin	Contours detected: 3	Expected: 1
Glyph name: aeacute	Contours detected: 3	Expected: 4
Glyph name: uni1E03	Contours detected: 4	Expected: 3
Glyph name: uniEFFD	Contours detected: 0	Expected: 9 or 7 [code: contour-count]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS |
|:-----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 6 | 4 | 71 | 7 | 70 |
| 0% | 4% | 3% | 45% | 4% | 44% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
