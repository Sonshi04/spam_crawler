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
1. python3.11インストーラをを公式サイトからダウンロードしてpythonをインストール <br>
https://www.python.org/ > Downloads > Download for Windows から最新版のpythonをダウンロード <br>
インストーラーのオプション等はすべてデフォルトでOK <br>
2. ライブラリをインストール <br>
コマンドプロンプトを開き、以下を実行 <br>
#pip install openpyxl selenium <br>

■操作手順  ※上の環境構築は行っておくこと
1. ツール一式をダウンロードする <br>
   右上のCodeをクリックし、表示された「Download ZIP」をクリック <br>
   任意の場所に展開する <br>
2. cralwer.pyと同一ディレクトリにip.xlsxを作成し、<br>
   1列目に調べたいip列を貼り付けて保存した後閉じる <br>
3. result_template.xlsxを複製し、result.xlsxとしてリネームする  <br>
4. コマンドプロンプトでcralwer.pyと同一ディレクトリに移動し、以下のようにcralwer.pyを実行する <br>
   #python cralwer.py  ※ 実行中にxlsxファイルを開かないこと
5. 終了したらresult.xlsxを開いて結果を確認する <br>


※注意事項
- ツール動作中はip.xlsx, result.xlsxのファイル名を変更しないこと
- このスクリプトで参照中のIPでエラーが出た場合、そのIP部分の結果は空白になるので手動で埋める必要あり
- chromeのバージョンがある程度新しくなるとこのスクリプトが動かなくなるので、適宜今のchromeバージョンにあったchromedriver.exeをダウンロードする
  -   バージョンによるエラーの場合は、以下から最新版chromedriver.exeのダウンロードする
  -   https://googlechromelabs.github.io/chrome-for-testing/#stable
  -   win64のchromedriverをダウンロードし、chromedriver.exeを置き換える


↓バージョン違いでこのようなエラーがでる

Current browser version is 123.0.6312.60 with binary path C:\Program Files\Google\Chrome\Application\chrome.exe



