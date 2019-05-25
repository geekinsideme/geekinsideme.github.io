# bash

## links

* [Bash scripting cheatsheet](https://devhints.io/bash)

## コマンド

```bash
var=value  # 変数代入
echo $var1  # 変数参照
echo ${var1}  # 変数参照
echo $1 $2 … $9 ${10}  # 引数参照
echo $?  # 終了ステータス

# if
if 条件式
then
    処理
else
    処理
fi

# 条件式
test ${foo} -eq 1
[ ${foo} -eq 1 ]

# case
case 値 in
    パターン1 ) 処理1 ;;
    パターン2 ) 処理2 ;;
esac

# while
while 条件式
do
    処理
done

# for
for 変数 in 値リスト
do
    処理
done
```

## 展開

```bash
# ブレース展開
abc{0,9} # abc0 abc9
abc{0..9} # abc0 abc1 ... abc9
abc{0..9..2} # abc0 abc2 ... abc8
~ # ホームディレクトリ
~+ # カレントディレクトリ
~- # ひとつ前の作業ディレクトリ
${var} # 変数展開
`コマンド` $(コマンド) # コマンド置換
$(( 計算式 )) # 算術式展開
IFS=" \t\n" # 単語分割 デフォルトは 空白 タブ 改行
a* a? a[xy] # パス名展開 任意の文字列 任意の1文字 含まれる任意の1文字
<(コマンド) >(コマンド) # プロセス置換
```

## カスタマイズ

```bash
PS1='\u@\h:\w\n\$ ' # \u ログイン名 \h ホスト名 \n 改行 \w カレントディレクトリ \$ $ または ＃

```


corntab

```corntab
# 分    時  日   月  曜日    user command
*/10    *   *   *   *   name    /home/…

9,10,11 リスト形式
9-17 範囲指定
*/10 繰り返し指定
0-30/5 0から30分の間5分毎

```
