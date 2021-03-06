# rime-hoisanva
A RIME IME for Taishanese

## Hoisanva IME Windows Install Instructions (credits to [suspiciouscactus](https://github.com/suspiciouscactus)) ##
1. Follow [this guide](https://github.com/rime/rime-cantonese/wiki/Windows-%E5%AE%89%E8%A3%9D%E6%95%99%E7%A8%8B#%E7%AC%AC%E4%B8%80%E6%AD%A5%E5%AE%89%E8%A3%9D%E5%B0%8F%E7%8B%BC%E6%AF%AB%E5%89%8D%E8%87%BA%E7%A8%8B%E5%BC%8F-step-1-install-the-weasel-frontend) until you click 獲取更多輸入方案.
2. Instead of typing `cantonese`, `emoji`, and `sgalal/rime-opencc-32bit-latest` in the console, type `pearapple123/rime-hoisanva`.
3. Follow the rest of [the guide](https://github.com/rime/rime-cantonese/wiki/Windows-%E5%AE%89%E8%A3%9D%E6%95%99%E7%A8%8B#%E7%AC%AC%E4%B8%89%E6%AD%A5%E9%81%B8%E5%8F%96%E8%BC%B8%E5%85%A5%E6%B3%95-step-3-enable-the-cantonese-input-method) and make sure to check the box for 台山話.

## 台山話輸入法Windows安裝指南 ##
1. 遵守[依個指南](https://github.com/rime/rime-cantonese/wiki/Windows-%E5%AE%89%E8%A3%9D%E6%95%99%E7%A8%8B#%E7%AC%AC%E4%B8%80%E6%AD%A5%E5%AE%89%E8%A3%9D%E5%B0%8F%E7%8B%BC%E6%AF%AB%E5%89%8D%E8%87%BA%E7%A8%8B%E5%BC%8F-step-1-install-the-weasel-frontend)直到點擊咗「獲取更多輸入方案」。
2. 而唔係喺指令打字`cantonese`，`emoji`同`sgalal/rime-opencc-32bit-latest`，打字`pearapple123/rime-hoisanva`。
3. 遵守其餘[個指南](https://github.com/rime/rime-cantonese/wiki/Windows-%E5%AE%89%E8%A3%9D%E6%95%99%E7%A8%8B#%E7%AC%AC%E4%B8%89%E6%AD%A5%E9%81%B8%E5%8F%96%E8%BC%B8%E5%85%A5%E6%B3%95-step-3-enable-the-cantonese-input-method)，就打勾「台山話」勾選。

## Manual Installation ##
1. Place all files except for `README.md` in:
  - `C:\Users\[user]\Appdata\Roaming\Rime` (Windows)
  - `/home/[user]/.config/ibus/rime` (Linux, ibus)
2. Add `    - {schema: gene}` and `    - {schema: gene_numeric}` to `default.custom.yaml`'s patch section
3. Redeploy.

## 手工安裝 ##
1. 攞嗮文件除咗`README.md`喺：
  - `C:\Users\[user]\Appdata\Roaming\Rime` (Windows)
  - `/home/[user]/.config/ibus/rime` (Linux, ibus)
2. 喺`default.custom.yaml`中打字`    - {schema: gene}`同`    - {schema: gene_numeric}`
3. 重新部署

## Tone input in / 打字聲調喺 hoisanva_numeric.schema ##

### Base Tones
| Input / 輸入 | Output / 產值 |
| ----------- | ------------ |
| qr          | 55           |
| q           | 33           |
| r           | 11           |
| w           | 31           |
| z           | 21           |

To input 55, type any two-letter combination of q, r, w, or z that aren't duplicates eg. qr, qw, qz; rq, rw, rz; etc.
/ 為咗輸入聲調55、打字任何第啲兩個字母嘅組合個「q」、「r」、「w」定係「z」

Duplicates qq, rr, ww, and zz are reserved for the changed tones mentioned below.

### Changed Tones

The changed tones are input by duplicating the corresponding input letter.

| Input / 輸入 | Output / 產值 |
| ----------- | ------------ |
| qq          | 35           |
| rr          | 15           |
| ww          | 325          |
| zz          | 215          |

## Collaborators / 合作者 ##
- [suspiciouscactus](https://github.com/suspiciouscactus)
- Ace Dystopia#2150 (His YT Channel / 佢嘅YT頻道: https://www.youtube.com/channel/UC_TJP_igpDN7HijY-JrWEqg)
- baatyrdyk#9595
