# 第5回 Webエンジニアリング演習 レポート
## 学籍番号
4724124
## TODO配列のコード
const todos = [
    { id: 1, title: "型を復習する", completed: true},
    { id: 2, title: "配列を学ぶ", completed: false},
    { id: 3, title: "レポートを書く", completed: true},
    { id: 4, title: "課題をする", completed: false},
    { id: 5, title: "お買い物に行く", completed: false},
];
## TODOを更新した条件
const completedBefore = todos.filter((todo) => todo.completed).length;

for (const todo of todos) {
    if (todo.completed === false) {
        todo.completed = true;
        console.log(`更新後: ${todo.title} [完了]`);
    }
}

const completedAfter = todos.filter((todo) => todo.completed).length;
console.log(`完了件数: 更新前 ${completedBefore}件 -> 更新後 ${completedAfter}件`);
## 完了件数の更新前後の実行結果
更新後: 配列を学ぶ [完了]
更新後: 課題をする [完了]
更新後: お買い物に行く [完了]
完了件数: 更新前 2件 -> 更新後 5件
