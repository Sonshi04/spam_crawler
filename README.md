# spam_crawler

- 各スパム確認サイトを巡回するスクリプト
- 入力はip.xlsxのA行のip  
- 出力はresult.xlsx  


■環境
python3.11, windows10 64bit
ライブラリ
selenium openpyxl 
(多分2つだけ)

■環境構築
1. python3.11インストーラをを公式サイトからダウンロードしてpythonをインストール
https://www.python.org/ > Downloads > Download for Windows から最新版のpythonをダウンロード
インストーラーのオプション等はすべてデフォルトでOK
2. ライブラリをインストール
コマンドプロンプトを開き、以下を実行
#pip install openpyxl selenium

■操作手順
1. このコードを右上のCodeからzipでダウンロード、任意の場所に展開する
2. cralwer.pyと同一ディレクトリにip.xlsxを作成し、1列目に調べたいip列を貼り付けて保存した後閉じる
- - 
3. result_template.xlsxを複製してresult.xlsxとしてリネームする
4. コマンドプロンプトでcralwer.pyと同一ディレクトリに移動し、以下のようにcralwer.pyを実行する
#python cralwer.py
5. 終了したらresult.xlsxを開いて結果を確認する


※注意事項
- このスクリプトで参照中のIPでエラーが出た場合、そのIP部分の結果は空白になるので手動で埋める必要あり
- スクリプトを実行中にxlsxファイルを開くとエラーでスクリプトが止まる可能性があるので注意(最初からやり直し)
- chromeのバージョンがある程度新しくなるとこのスクリプトが動かなくなるので、
- 適宜今のchromeバージョンにあったchromedriver.exeをダウンロードする

↓バージョン違いでこのようなエラーがでる

Current browser version is 123.0.6312.60 with binary path C:\Program Files\Google\Chrome\Application\chrome.exe

- 以下最新版chromedriver.exeのダウンロード場所 win64のchromedriverをダウンロードし、chromedriver.exeを置き換える
https://googlechromelabs.github.io/chrome-for-testing/#stable

