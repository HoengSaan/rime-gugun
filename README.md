# 菊韻諺文

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

本作品採用[創意共享 署名-非商業性-相同方式共享 4.0 國際版許可證](cc-by-nc-sa)。

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

**元方案中無聲明任何許可，只禁止任何商業利用行爲。**

### 其他菊韻項目

- 菊韻粵語：[rime-gukwan: 菊韻粵語輸入方案 基於中州韻 Cantonese IME (RIME Scheme)](https://github.com/HoengSaan/rime-gukwan)
- 菊韻同文主題：[trime-gukwan: 同文輸入法36鍵鍵盤主題 Trime IME 36 Keys Keyboard Theme](https://github.com/HoengSaan/trime-gukwan/)
- 菊韻和語【停止維護】：[rime-kikwin: 菊韻日本語入力法 基於中州韻 Japanese IME (RIME Scheme)](https://github.com/HoengSaan/rime-kikwin)

## 簡介 Introduction

此爲[RIME | 中州韻輸入法引擎](https://rime.im/)諺文方案，基於[oniondelta/Hangul_Rime_Files](https://github.com/oniondelta/Hangul_Rime_Files)。造輪目的是因爲我對其他諺文羅馬字方案不滿，創造基準爲一個部件（非諺文字母）對應一個拉丁字母。

A RIME Hangul input method based on [oniondelta/Hangul_Rime_Files](https://github.com/oniondelta/Hangul_Rime_Files). The purpose of reinventing the wheel is that I am dissatisfied with existing romanizations for Hangul. The basic principle of this wheel is that each component (not equivalent to Jamo) corresponds to one Latin letter.

同文用戶可使用菊韻同文主題，有適配佈局。

Trime User can use trime-gukwan theme for the dedicated layout.

### 更新 Update【v1.3】

- 優化Spelling Algebra
- 新增終聲專用後綴「w」，「w」元功能被取消。

## 指南 Guide

演示 Showcase：https://youtu.be/pPqiRuUQ7SE

<img src="pic\keyboard-layout.png"/>

- 後綴「;」出漢字｜Subfix ";" for Chinese Characters ( Hanja )
- 後綴「f」出諺文字母｜ Subfix "f" for Hangul Jamo
- 後綴「ff」出諺文兼容字母｜Subfix "ff" for Hangul Compatibility Jamo
- 後綴「w」出諺文字母（終聲專用）｜Subfix "f" for Hangul Jamo ( Only Final )
- 前綴「=」倉頡反查｜Prefix "=" for Cangjie reverse look-up
- 「x」爲去聲；「xx」爲上聲｜"x" for departing tone; "xx" for rising tone.

### 輸入 Input

- 此方案中，二重母音被視爲兩個部件；In this scheme, diphthongs are treated as two components.
  - ㅑ：ㅣ＋ㅏ＝i+a＝ia
  - ㅒ：ㅣ+ㅏ+ㅣ＝i+a+i＝iai
  - 뾿：ㅂ＋ㅂ+ㅣ＋ㅗ＋ㄹ＋ㅎ=(b+b)+(i+o)+(l+h)＝bbiolh
- 由於[諺文音節](https://www.unicode.org/charts/PDF/UAC00.pdf)無古諺文，須利用諺文字母（後綴「f」）輸入。Since [Hangul Syllables](https://www.unicode.org/charts/PDF/UAC00.pdf) do not support Old Hangul, it is necessary to input using Hangul Jamo with suffix "f".
  - ㆆ：ㅡ＋ㅇ＝y+q+f
  - ㅸ：ㅂ＋ㅇ＝b+q+f
  - ᄊᆡ：ㅅ＋ㅅ＋ᆞ＋ㅣ＝(s+s+f)+(vi+f)
- 可用後綴「w」指定終聲，毋須手動指定。Use suffix "w" to type Hangul Jamo final for smoother typing experience.
  - ᄅᆞᆯ：ㄹ＋ᆞ＋ㄹ＝(l+f)+(v+f)+(l+w)
  - ᄠᅳᆷ〯：ㅂ＋ㄷ＋ㅡ＋＋ㅁ＋〯＝(b+d+f)+(y+f)+(m+w)+xx


星號爲古諺文。井號爲部件。Asterisk stands for Old Hangul. Hash stands for component.

#### 母音 Vowels

- 「i」作爲介音時可用「j」替代｜When "i" is used as a prenuclear gilde, it can be replaced with "j."
- 「oa」可用「wa」替代｜"oa" can be replaced with "wa"

| 陰 Negative | 陽 Positive | 中 Neutral |
|----          |----         |----         |
|ㅡ y#    | ㆍ v* | ㅣ i# |
|ㅓ e#   	      |ㅏ a# 	        |          |
|ㅜ u#  |ㅗ o#  |  |
|ㅕ ie（je） |ㅑ ia（ja） | |
|ㅠ iu（ju） |ㅛ io（jo） | |
|ㅐ ai |ㅔ ei |ㅢ yi |
|ㅒ iai（jai） |ㅖ iei（jei） |  |
|ㅝ ue | ㅘ oa（ua） |ㅟ ui |
|ㅞ uei | ㅙ oai（uai） |ㅚ oi |

#### 子音 Consonants

- 十個中古漢語用古諺文不能被拆解，有專用輸入碼。There are 10 Old Hanguls for Middle Chinese cannot be decomposed, they have dedicated input codes.
- 「ㆁ」被視作「ㅇ」，但仍可用`ng`輸入。"ㆁ" is regarded as "ㅇ", but still can be input using `ng`. 
  - 롱：ㄹ＋ㅗ+ㅇ＝l+o+q＝long
- 初聲「ㅇ」可被省畧。此功能對輸入有影響，可自行在方案文件關閉。Initial "ㅇ" can be omitted. This function affects input and can be turned off manually in the scheme file.
  - 앜：ㅇ＋ㅏ+ㅋ＝q+a+k＝ak

| 全清 | 半清 | 全濁 | 半濁 |
|----         |----       |----       |:---         |
| **Slack** | **Aspirate** | **Tenuis/Voiced*** | **Other** |
|ㄱ g#	       |ㅋ k#        |ㄲ gg        |ㆁ ng*        |
|ㄷ d#	       |ㅌ t#	       |ㄸ dd  |ㄴ n#  |
|ㅂ b#	       |ㅍ p#  |ㅃ bb        |ㅁ m#        |
|ㅅ s#	       | ㅎ h# |ㅆ ss        | ㅇ q# |
|ㅈ z#  |ㅊ c#        | ㅉ zz | ㄹ l# |
| | | ㅿ r#*             |  |
|ᄼ sh* | | ᄽ ssh* |  |
|ᄾ sr* | | ᄿ ssr* |  |
|ᅎ zh* |ᅔ ch* | ᅏ zzh* |  |
|ᅐ zr* |ᅕ cr* | ᅑ zzr* |  |

## 安裝 Installation

丟去程式文件夾即可。Just dump the files to Rime's program folder. 
