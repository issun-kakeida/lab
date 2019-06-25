#■error 再登録
git remote rm origin
git remote add origin https://github.com/issun-kakeida/lab.git
git push -u origin master

#■マージが失敗した場合
git merge --allow-unrelated-histories origin/master

#■ローカル側
#新しいローカル
git init　#Gitリポジトリを新たに作成する .git
git add --all　#カレントディレクトリのファイル等をインデックス
git commit -m "# comment"　＃ローカルリポジトリにコミット
#リポジトリ先アドレス
git remote add origin https://github.com/issun-kakeida/GAS.git　#リモートリポジトリに反映
#失敗した場合は一度消す　git remote rm origin
git push -u origin master　#とすると次回から　git pushで　origin master　でpushしてくれる
#以降は
git push


#gitからコピーしてくる　コピー先アドレス
git clone https://github.com/issun-kakeida/lab.git
#リポジトリ先アドレス
git remote add origin https://github.com/issun-kakeida/lab.git
