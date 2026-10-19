# 第4回 Webエンジニアリング演習 レポート
## 学籍番号
4724124
## `const`と`let`の宣言・再代入に使用したコード
const courseName = "Web Engineering";
let retryCount = 1;


retryCount = 2;
console.log(`${courseName},${retryCount}`);
## VSCodeと`pnpm run check`に表示されたエラー番号・メッセージ
$ tsc --noEmit src/index.ts
src/index.ts:23:1 - error TS2588: Cannot assign to 'courseName' because it is a constant.

23 courseName = "Other Course";
   ~~~~~~~~~~


Found 1 error in src/index.ts:23

[ELIFECYCLE] Command failed with exit code 2.
## 修正後の実行結果と`const`・`let`の違いの説明
$ tsx src/index.ts
キーボード 4800 2 true
960
キーボードを2個購入する
税込み合計は960円である
Web Engineering,2

constは値が常に一定なので再代入ができず、letは値が常に一定ではないので値の再代入が可能。
