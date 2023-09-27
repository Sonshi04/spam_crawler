# spam_crawler

- 各スパム確認サイトを巡回するだけのスクリプト(最新版)
- 入力はip.xlsxのA行のip  
- 出力はresult.xlsx  


■環境
python3.11, windows 10
ライブラリ
selenium openpyxl 
(多分2つだけ)

■環境構築
1. python3.11インストーラをを公式サイトからダウンロードしてpythonをインストール
2. ライブラリをインストール
#pip install openpyxl selenium

■操作手順
1. ip.xlsxを作成し、1列目に調べたいip列を貼り付けて保存した後閉じる
2. result_template.xlsxを複製してresult.xlsxとしてリネームする
3. 以下のようにcralwer.pyを実行する(実行中はこの2つのxlsxファイルを開かないこと)
#python .\cralwer.py
4. 終了したらresult.xlsxを開いて結果を確認する