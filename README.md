# 隨便打 Suibianda

macOS 的注音輸入法：照自己的節奏打，中文、英文、打錯的字都交給它判斷，一般句子不用手動選字。

介紹與使用說明：<https://cerry0524.github.io/suibianda/>

這個倉庫只放安裝檔與版本說明（Releases），不含輸入法本身的原始碼。

## 下載與安裝

1. 到 [Releases](https://github.com/Cerry0524/suibianda-releases/releases/latest) 下載 `Suibianda-<版本>.zip`，解壓縮後打開「SuibiandaInstaller」，按「我接受」安裝。
2. 安裝程式裡可以一鍵下載整句重讀的模型（約 188 MB）；之後再打開安裝程式下載也可以。
3. 打開「系統設定」›「鍵盤」›「文字輸入」，按「輸入方式」旁的「編輯⋯」，再按「＋」，在「繁體中文」選「隨便打-繁」。清單裡找不到時，登出再登入一次。

需要 macOS 12 以上，Apple 晶片與 Intel Mac 都可以；整句重讀需要 macOS 13 以上。

## 授權

- 隨便打免費使用，所有功能都免費。
- 組字引擎（LibVanguard）與匯入模組（OtherIMEDataReader）以 LGPL-3.0-or-later 授權。每個版本都附上這兩部分的原始碼壓縮檔 `Suibianda-<版本>-LGPL-source.tar.gz`，包含隨便打所做的修改；兩者都以動態函式庫隨輸入法出貨，可以自行替換。
- 整句重讀的模型由中央研究院 CKIP Lab 的 bert-base-chinese 轉換而來，以 GPL-3.0 散佈；模型壓縮檔 `HomophoneScorer-<版本>.zip` 內附授權全文與轉換程式。
- 中英混打的英文詞頻表衍生自 wordfreq（CC BY-SA 4.0）。
- 詞庫的詞頻資料僅限非商業使用。
