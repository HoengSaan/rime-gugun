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

## 簡介 Introduction 紹介

基於[oniondelta/Hangul_Rime_Files](https://github.com/oniondelta/Hangul_Rime_Files)，此爲[RIME | 中州韻輸入法引擎](https://rime.im/)諺文音碼方案。拼音基於粵拼以符合本人習慣。

Based on [oniondelta/Hangul_Rime_Files](https://github.com/oniondelta/Hangul_Rime_Files), a Hangul input method based on RIME. The romanization is based on Jyutping to suit my personal preference.

同文用戶可使用菊韻同文主題，有適配佈局。

Trime User can use trime-gukwan theme for the dedicated layout.

### 更新 Update【v1.1】

- 鍵位・拼音改進
- 刪除腳本

## 輸入 Keymap

<img src="pic\key.jpg"/>

星號爲古諺文。Asterisk stands for Old Hangul.

### 母音 Vowels

| 陰 Negative | 陽 Positive | 中 Neutral |
|----          |----         |----         |
|ㅡ y    | ㆍ v*    | ㅣ i（j） |
|ㅓ e   	      |ㅏ a 	        |          |
|ㅜ u（w/wu）  |ㅗ o  |  |
|**陰介** |**陽介** | |
|ㅕ ie |ㅑ ia | |
|ㅠ iu |ㅛ io | |
|**陰雙** |**陽雙** |**中雙** |
|ㅐ ai |ㅔ e |ㅢ yi |
|ㅒ iai |ㅖ iei | |
|ㅝ ue | ㅘ oa（ua） |ㅟ ui |
|ㅞ uei | ㅙ oai      |ㅚ oi |


### 子音 Consonants
| 全清 | 半清 | 全濁 | 半濁 |
|----         |----       |----       |:---         |
| **Slack** | **Aspirate** | **Tenuis/Voiced*** | **Other** |
|ㄱ g	       |ㅋ k        |ㄲ gg        |ㆁ ng        |
|ㄷ d	       |ㅌ t	       |ㄸ dd  |ㄴ n  |
|ㅂ b	       |ㅍ p  |ㅃ bb        |ㅁ m        |
|ㅅ s	       | ㅎ h |ㅆ ss        | ㅇ q      |
|ㅈ z  |ㅊ c        | ㅉ zz | ㄹ l |
| | | ㅿ r*              |  |
|ᄼ sh* | | ᄽ ssh* |  |
|ᄾ sr* | | ᄿ ssr* |  |
|ᅎ zh* |ᅔ ch* | ᅏ zzh* |  |
|ᅐ zr* |ᅕ cr* | ᅑ zzr* |  |

### 其他 Other

| 上聲 Rising Tone | 去聲 Departing Tone |
| ---------------- | ------------------- |
| 〯（U+302F）xx     | 〮（U+302E）x         |

- 後綴「;」出漢字 Subfix ";" for Chinese Characters ( Hanja )
- 後綴「f」出諺文部件 Subfix "f" for Hangul Jamo
- 後綴「ff」出諺文兼容部件 Subfix "ff" for Hangul Compatibility Jamo
- 前綴「=」倉頡反查 Prefix "=" for Cangjie reverse look-up

由於[諺文音節](https://www.unicode.org/charts/PDF/UAC00.pdf)無古諺文，須以部件輸入。如下 

Since [Hangul Syllables](https://www.unicode.org/charts/PDF/UAC00.pdf) do not support Old Hangul, you need to input Old Hangul by Jamo. Examples below:

- ㆆ：ㅡ＋ㅇ＝yq 
- ㅸ：ㅂ＋ㅇ＝bq
- ᄊᆡ〮：ssfvifx 

## 安裝 Installation

丟去程式文件夾即可。`rime.lua`則丟去用戶文件夾。

Just dump the files to Rime's program folder, only `rime.lua` need to be in user folder. 
