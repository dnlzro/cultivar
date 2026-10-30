# Changelog
All notable changes to this project will be documented in this file.

## 1.000 (unreleased)
First release of Cultivar, based on JetBrains Mono 2.305 (unreleased):
- Renamed the family to Cultivar and restarted versioning at 1.000
- Redrew the double-storey `g` (`cv03`)
- Swapped the default and alternate glyphs for `cv03` `cv14` `cv20`: the double-storey `g`, the alternate `$` `¢` and the alternate `5` are now the defaults, and the features switch back to the JetBrains Mono glyphs
- Made the slashed zero the default and removed the `zero` feature; the JetBrains Mono zero, with the dot inside, is now `cv13`
- Narrowed the zero, including `cv13`, and slightly widened the `O` and the glyphs drawn from it, so the zero is now about 92% of the width of the `O`; it was wider than the `O` in the lighter weights
- Removed the built font files from the repository; fonts are now built by CI and attached to GitHub Releases

# JetBrains Mono history
Changes made upstream, before Cultivar was forked.

## 2.305 (unreleased)
- Added `IJ` `ij` #578
- Added ligature breaking in `++:` `:++` #434
- Added exclusion in `<>>` sequence #565
- Fixed typo in ss20 name
- Switched source files to Glyphs 3 

## 2.304 (14.01.2023)
### **Major changes**
- Added OT Stylistic Set 1 `ss01`. Performs better with plain text.
- Added OT Stylistic Set 2 `ss02`. Performs better with small line-height.
- Added glyph alternates for `l` `t` `g` `j` `m` `w` `k` `f` `r` `y` `u` - `cv01`–`cv17` #238 #339
- Alt `2` `6` `9` construction - `cv18`.
- Updated construction of `8` and `5` (the old versions can be found in `cv19`& `cv20`, respectively)
- Added less radical alternates for `!=` `!==` `==` `===` ligatures - `ss19` #287
- Added full support for APL #47 #516
- Updated Greek alphabet to be less eccentric
- Different construction of italic `e`
- Added full Double Struck alphabet #440
### **Other updated and fixes**
- Contour polishing
- Alternate `&` - `cv15` #507
- Alt `$` - `cv14` #527
- Shifting the horizontal bar in `f` to match x-height - `ss20`
- Added `﹢` U+FE62 #482
- Added `∴` #480
- `! =` ligature fixed #494
- Debug mode for Cyrillic `c` `C` #27
- Reverted the construction of italic `a` #416
- Dutch diacritics works properly #100
- Fixed the backquotes placement #411
- Reworked control code symbols #491
- Updated marks placement in `Ľ`, `ď`, `ľ`, `ť` #522
- Added `\/` `/\` ligatures #222
- Added `➔` `➝` `➞` #545
- Complete soft doting #345
- Updated `‚` `„` `“` `”` `‘` `‛` `‟` #563
- Added support for Udmurt language #569

## 2.242 Quick Fix (30.07.2021)
- Added `???` `<:<` ligatures #434
- Corrected the `⊈` (u+2288) #475
- Remove second unicode value from `HT` (u+2409 u+0009) `CR` (u+240D u+000D) `LF` (u+240A u+000A) #476

## 2.241 (27.07.2021)
- Made triple equal ligature `===` more spacious #25
- Added 70 symbols from #47 `ƛ` `ϕ` `ϖ` `⁅` `⁆` `⦇` `⦈` `‴` `⟪` `⟦` `⟫` `⟧` `≃` `≔` `≅` `≇` `⋎` `∸` `⋐` `⋰` `⋱` `⋮` `≡` `∹` `≳` `≲` `⋯` `⊈` `≯` `≱` `≢` `≮` `≰` `÷` `≥` `≤` `~` `∅` `≺` `≼` `≟` `⤖` `≗` `⊓` `⊔` `⊑` `≋` `↭` `↞` `↠` `↣` `↥` `↦` `↧` `⇉` `⇑` `⇒` `⇓` `⇔` `⇧` `⇨` `⍳` `⍨` `♭` `♯` `𝔽` `𝕊` `⅀`
- Added `ǒ` `ǐ` `ǔ` `ǖ` `ǘ` `ǚ` `ǜ` #187
- Added Control code support #241
- Tuned `#` #275
- Added `=:` ligature #305
- Added floor and ceiling mathematical characters `⎪` `⎩` `⎨` `⎧` `⎢` `⎣` `⎡` `⎭` `⎬` `⎫` `⎥` `⎦` `⎤` #328
- Corrections in `Θ` `θ` `ξ` `Σ` `∑` #351
- Added `Ɛ` `↋` `↊` `૪` #356
- Added Cyrillic Kazakh letters #391
- Added ligature `;;;` #393
- The ligature `<-` have 3 digit exclusion #403
- Changed the look of `~@` ligature #415
- Fixed regression with `<--` ligature #417
- Fixed interpolation error in Italic #431
- Added EMQuad (u+2001) #439
- Reworked `⚠️` #450
- Made the tail of Italic `f` shorter to render better in kitty #441
- Added SemiBold weight #453
- Added more anchors to the marks #463
- Added replacement (u+FFFD) #461
- Added zeroWidthNoBreakSpace (u+FEFF) #467
- Corrected placement of `*` in `*/` ligature in Regular master
- Tuned `Ч` `ч`
- Fixed consistency of `J` in italic


## 2.225 (27.01.2021)
- Added exclusion in `<-` ligature to look reasonable in negative arguments for C++ `<-1>` #107
- `/**` brought back #202
- `*/` `/*` aligned to match `*`  #215
- Added multiline bracket characters `⎛` `⎞` `⎝`  `⎠` `⎜` #290
- Tuned Greek letters construction and contour polish #336
- Removed `[||]` ligature to more consistence with `[|`  `|]` #353
- Added `ϖ` #369
- Fixed monospace breaking by tuning `⟵` `⟶` `⟷` arrows to fit standard width #387
- Added exclusion in `[<` `>]` to perform in `[<=5]` expression #388
- Fixed Powerline arrows height #395

## 2.221 (28.12.2020)
- Tuned Vietnamese diacritics more, removed errors in `Ẫ`
- Removed `0x0` ligature #346
- Added `⟵` `⟷` `⟶` #255
- Corrected vertical placement on BoxDrawing elements
- Removed `.-` ligature #76
- Disabled ligatures for lookahead/lookbehind prefixes (regex) #126
- Added support for combined marks #228
- Added `∪` #244
- Added `➜`(U+279C), `✗`(U+2717), and `✓`(U+2713) #246
- Added `<<~` #291
- Added `‾` Overline #298
- Tuned Cyrillic `в` #335
- Increase height of BoxDraving #382
- Added `‿` `∁` `∎` `⊸` `⊎` `⨀` `⨆` `∩` `∶` `⊢` `⊤` `⊥` `⊛` `⊖` `⊗` `⊙` `⊕` `◦` `⋆` `ℚ` `ℤ` `slashshortcomb`
- Corrected placement of bar in `Đ`
- Polished Digits

## 2.210 (12.11.2020)
- Vertical metrics (win, hhea, typo) made equal to prevent different line-height #334 #286. In some cases it will increase line-height by 1px but in some cases it will decrease by 3px
- Because of vertical metrics unification Vietnamese diacritics was made more compact in capital letters
- Added symbols `□` `△` `▽` `◁` `▷` `▻` `◅` `►` `◄` `▪` `▫` `▴` `▾` `◂` `▸` `▵` `◃` `▹` `▿` `∘` `❮` `❯` `❰` `❱` `◌` `◯` `◎` `✕` `⚠` `⚡` `⌂` `◔` `◧` `◨` `◩` `◪` `◫` `⌄` `⌅` `◕` `⌥` `⌃` `⇧` `⌘` #277
- Added Bitcoin symbol #292
- Correction in Greek letters `Θ` `ρ` #336
- Removed `0xFF` ligature #346

## 2.200 (21.10.2020)
### Major changes
- Added Greek alphabet #58
- Reworked diacritics #228
- Removed *x-height* increasing from hinting. Affects non Retina screens. #286 #265 #272 #262 #275
- A lot of tiding up of contours to meet Google Fonts criteria
### Other updated and fixes
- Ligature for `0x` (hexadecimal) prefix #98
- Lowered horizontal bar in *Florin* to make it more distinguishable form italic `f` #129
- Changes the `8` construction to make it more distinguishable from `B` and `0` #188
- Added Changelog #263
- Variable font correctly grouped in one family with Italics #270
- Reverted to previous construction of f #273
- Corrected OneNote line height #278
- Removed kerning pair #297
- Add Overline #298
- Increased difference between hyphen, en-dash, and em-dash #318
- Removed the "tail" in the italic `a` 

## 2.002 (27.08.2020)
- Changed license from Apache 2.0. to SIL 1.1.
- Corrected _Extra Light_ weight name in metadata #274

## 2.001 (13.07.2020)
- Corrected proportion string in metadata in Italic #266
- Changed the naming of source files to match previous

## 2.000 (10.07.2020)
### Major changes
- Added 3 lighter weights with matching italics #1 SemiLight — Special for the dark background. It’s a slightly more thin version of Regular. Light — Will perform best on HiDpi in more big sizes. ExtraLight — If you want to go even thinner. Recommended for presentation mode.	
- Added Variable format for more precise weight tuning. 
- Project migrated from _FontLab_ to _Glyphs_. Source in UFO provided.
### Other updated and fixes
- *ML comment ligatures are vertically misaligned #77 
- Ligatures in a glob pattern look inconsistent #88 
- Zero - hinting the dot #104
- Big space above text in OneNote #210 
- Corrected hinting #218 #235 #239 #252
- Monospaced detection errors #227 #230
- Corrected wrong interpretation in `<||> |>`#234
- Reworked `%`, `‰` #236
- Missing some Powerline symbols #240
- Disable `>-` ligature when followed by `<` (`>-<`) #251
- Add the Latin Capital Letter Sharp S `U+1E9E` #262
- Added superior & inferior numbers `⁰¹²³⁴⁵⁶⁷⁸⁹₀₁₂₃₄₅₆₇₈₉`
- Fine tuning of capital, ascender & descender metrics
- Raised the bar in `f` to work better in context of the line
- More spacing tuning in arrow ligatures 
- Corrections in `-<` `-<<` `<-` `<!--`
- More pronounced bar in `Ħ` `Ŧ` `ћ` `ħ` `đ` `ŧ`
- Correct `u+02C9` placement
- Corrected placement of _Ogonek_ in `Ų`
- Corrections in Vietnamese diacritics

## 1.0.6 (29.04.2020)
### Major changes
- Fixed problems with rendering of Powerline symbols #189 
- Added support of Vietnamese language #14 #209
- All diacritics redone. Corrected a bunch of problems of placing & more balanced mass.
- Added DesignSpace+UFO source files. Just converted & dumped as they are, for now. There are issues with Masters compatibility. Tested in Glyphs app.
### Other updated and fixes
- Fixed construction of `†` `‡` `∏` `∐` #205 #206
- Added exclusion in `/*` ligature #88
- Refactored `ß`
- `~=` ligature removed #204 
- Added `>->` ligature #194
- Added `u0336` Long stroke overlay #190
- Added ligature `//=` #185
- Corrected contour of the arrows in ligatures #196
### Known issues
- In Medium weights the height of `[` `]` `{` `}` decreased by one pixel in 12px, 13px sizes. This is a hinting bug.

## 1.0.5 (24.03.2020)
- Lowered the height of Powerline arrows #172
- `<*>` Interpolation bug fix #180
- Removed ligatures from loading sequences `[->` `[=>` #151
- Tuned `1` to be more distinguishable from `i` in small sizes #176
- Sorted glyphs by unicode order #170
- Added `U+02BC` "Modifier Letter Apostrophe" #168
- Added new ligature `@_`
- Added 29 glyphs: `Ə` `ə` `Ǧ` `ǧ` `Ǫ` `ǫ` `Ǵ` `ǵ` `∀` `∃` `∈` `∋` `∐` `⟨` `⟩` `∧` `∨` `∷` `∼` `≈` `≡` `⍴` `■` `▲` `▶` `▼` `◀` `◆` `●`
- Added support of https://unicodepowersymbol.com/
- Refactored `¶` `l` `j`

## 1.0.4 (11.03.2020)
- Added No Ligature version. Only in `.ttf` format. It called **JetBrains Mono NL**. #19
- Fixed problems with tiny gaps between the Box Drawing elements. #84
- Balanced the size of `<>` `</>` ligatures to match in mass. #116
- Fixed problem with not working `<--` ligature. #95
- Added `U+FEFF` symbol. No-break zero space. #147
- `<!--` `-->` ligatures now should be on the same heights. #77
- Corrected `===>` behaviour in loading sequences. #151
- Corrected `A` placement in italics.
- Made dot in the `0` smaller, so it will be more distinguishable from `8` at small sizes.

## 1.0.3 (07.02.2020)
- Added support of Box Drawings 159 symbols #84 #55
- Added ligature `<--` #95
- Removed the `\/` & `/\` ligatures #65 #76 #78 #83
- Corrected behaviour of ligatures in a glob pattern #88
- Changed the `$` `&` dependent glyphs #110
- Added _no-break space_ #94
- Corrected unexpected `>=` ligature usage in `>=<` sequence
- Refactored `w` `W` `m` `M`
- Slightly tuned ascenders & descenders
- Added support of Mongolian language #81
- Better placement of the dot in `0` #104
- Reorganised family names #122

## 1.0.2 (24.01.2020)
- Reorganised font family names for better recognition in Terminal apps
- Added powerline glyphs
- Added `₽` `λ` `←` `↑` `→` `↓` `↔` `↕` `↖` `↗` `↘` `↙`
- New ligature `<#--`
- Fixed bug with escape sequence ligature `\/`
- `[+->]` excluded from ligature sequence
- Dutch language now presented in Mac Font Book app

## 1.0.1 (21.01.2020)
- Update PANOSE and PostScript metadata to be visible as monospaced font on Windows 10
- Corrected the italic `ß` `ſ`
