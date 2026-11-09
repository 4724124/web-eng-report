# 第7回 Webエンジニアリング演習 レポート
## 学籍番号
4724124
## 2画面の見出しと本文
app.innerHTML = `
            <h1>detail</h1>`
app.innerHTML = `
            <h1>compare</h1>`
## クリック後のURLとNetworkの確認
https://redesigned-acorn-5g7g4q6rvvgv3p6gx-3000.app.github.dev/csr/#detail
確認できました。
https://redesigned-acorn-5g7g4q6rvvgv3p6gx-3000.app.github.dev/csr/#compare
確認できました。
## 画面を切り替える処理の要点
window.addEventListener("hashchange", () => {
    const page = location.hash;
    switch(page){
        case "#detail":
            app.innerHTML = `
            <h1>detail</h1>`
            break
        case "#compare":
            app.innerHTML = `
            <h1>compare</h1>`
            break
        default:
            break
    }
});
