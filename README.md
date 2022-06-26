# Laravel 9 品脫

引入 laravel 的 pint 套件來擴增專為極簡主義者設計的 PHP 程式碼風格修正器，理想狀況下，應該遵循一個已知的標準來撰寫 PHP 程式碼。可能是 PSR 的組合或者是 PEAR 或 Zend 程式碼標準的其中一個。這代表其他開發者能夠方便的閱讀與使用你的程式碼，且使用這些套件的應用程式能夠平順地與許多第三方套件一起使用。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 你可以使用 `./vendor/bin/pint` 指令來執行程式碼風格修正。
```sh
$ ./vendor/bin/pint
```

----

## 畫面截圖
![](https://i.imgur.com/OcrwVQ8.png)
> 修正程式碼語法，讓其符合標準，不用自己手動修復
