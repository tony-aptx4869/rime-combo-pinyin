# 宮保拼音

配方： ℞ **combo-pinyin**

[Rime](https://rime.im) 宮保拼音輸入方案

## 簡介

[宮保拼音](https://github.com/rime/home/wiki/ComboPinyin) 是由 [居戎氏](https://github.com/lotem) 設計、在標準電腦鍵盤上多鍵並擊輸入拼音的方法。

*並擊* （chord-typing）是指：數指同時按下鍵盤上的多個按鍵。

可選擇多種 [並擊鍵位佈局](layouts.md)：

  - 七指禪（大衆式），兼容通用鍵盤
  - 八指禪（執鍵人式），爲拆分空格鍵盤優化
  - 九指禪，兼容通用鍵盤
  - 十指禪，爲拆分空格鍵盤優化
  - 皓月九指禪，兼容通用鍵盤

## 定製緣起

我自己在使用七指禪和九指禪時，有一些痛點（就是有一些組合鍵並擊起來手真的很痛），
所以嘗試基於九指禪的佈局做出一些調整。調整簡介如下：

儘量減少組合鍵，尤其是聲母一側，組合鍵減少至三個，也就是只有 zh, ch, sh 的使用是
需要組合的，把 n, m, r 解放成單鍵使用。j, q, x 併入 z/g, c/k, s/h。

韻母一側也做了一些優化，針對我疼痛的手，專門設置 ü 和 üa，調整 -ou 位置。增加了
組合使用方式和單鍵使用方式。
比如 ü-n 爲 ⟨ün⟩，再比如將 üa 簡化爲 ⟨üan⟩。

## 安裝

本方案依賴於Rime輸入法預設的

  - [朙月拼音](https://github.com/rime/rime-luna-pinyin) ℞ **`luna-pinyin`**

[東風破](https://github.com/rime/plum) 安裝口令： `bash rime-install tony-aptx4869/rime-combo-pinyin`

授權條款：見 [LICENSE](LICENSE)

安裝後，請編輯 Rime 用戶設定目錄中的 `default.conf` 文件，
在 `schema_list:` 下面添加內容如下：

    schema_list:
      ...
      - schema: combo_pinyin_hy9  # 添加此條內容喲
      ...