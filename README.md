# バラバラゲーム
***
## １、押さえておくポイント、Swift言語特性
### 画面サイズを取得する方法
以下のコードで画面サイズを取得することができる
```
let width: CGFloat = UIScreen.main.bounds.size.width
```

---

### 配列とは
配列とは、データの集まりのようなもので同じ種類のデータをまとめることができ、番号が割り当てられていてその番号で呼び出すことができる。（学校のクラスと出席番号のようなもの）

---

### タイマーの使い方
一定間隔でメゾットを実行したいときなどにタイマーを使う
タイマーは以下のようなコードで設定できる
```
timer = Timer.scheduledTimer(timeInterval: タイマーを実行する時間の幅, target: self, selector: #selector(タイマーのたびに実行するメゾット), userInfo: nil, repeats: 繰り返すか)
```
```
timer.fire()
```
で起動することができる。
___

## ２、エラー

### タイマーのセレクターで選択するメゾットでエラーが発生
funcの前に@objcと入力する
