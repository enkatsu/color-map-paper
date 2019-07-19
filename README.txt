=== 芸術科学会学術会議(NICOGRAPH等)用 LaTeX サンプルファイル ===

1. ファイル

README.txt		このファイル
conference_samp.tex	LaTeX サンプルファイル
conference_samp.pdf	conference_samp.tex から生成した PDF ファイル
bibtex_samp.bib		BibTeX サンプルファイル
artsci-jour-j.sty	学術会議用スタイルファイル
latexmkrc_samp		latexmk 設定サンプルファイル
fig/fig-sample.eps	図用 EPS ファイル
fig/fig-sample.png	図用 PNG ファイル

2. コンパイル

latexmk コマンドを利用することができるのであれば、それを用いることが最も簡単です。
うまくいかない場合、同梱の latexmkrc_samp を latexmkrc に変更して再度試みて下さい。

% latexmk conference_samp

latexmk コマンドを使用せず、BibTeX を利用する場合は、以下のコマンドを入力して下さい。

% platex conference_samp
% pbibtex conference_samp
% platex conference_samp
% platex conference_samp
% dvipdfmx conference_samp

BibTeX を利用しない場合は、上記から pbibtex コマンドを抜いて下さい。

3. 問い合わせ

本サンプルで何か質問がありましたら、芸術科学会までお問い合わせ下さい。

4. 履歴

Ver.1.0: 2014/12/10
	作成: 渡辺大地@東京工科大
	初期バージョン

Ver.1.1: 2019/2/26
	作成: 渡辺大地@東京工科大
	TeXLiveの寸法に関する仕様が変更となったことを踏まえて修正

Ver.1.2: 2019/4/27
	作成: 渡辺大地@東京工科大
	概要に用いていた quote 環境が不具合を生じる場合があることへの対応。
	その他若干の内容変更。
