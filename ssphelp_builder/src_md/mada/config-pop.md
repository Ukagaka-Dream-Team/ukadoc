<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE.html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/.htmll1/DTD/.html1-frameset.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" lang="ja" xml:lang="ja">
<head>
  <meta http-equiv="content-type" content="text/html; charset=UTF-8" />
  <meta http-equiv="content-style-type" content="text/css" />
  <title>設定：POP</title>
  <link rel="stylesheet" type="text/css" href="about.css" />
</head>
<body>
<div id="sidebar">
	<iframe src="contents.html" name="sidebar">
		フレーム非対応の環境では以下の目次ページからご覧ください。

[目次](contents.html)
	</iframe>
</div>
<div id="text">
<div id="breadcrumb">
	<span class="Upper">[目次](contents.html)</span>
	<span class="Upper">[設定](config.html)</span>
	<span class="Upper">本体設定</span>
	POP
</div>
<!-------------------------------------------------------------------------------------------------------------------------------->

# 設定：POP

	画像左側のリストを<span class="Doing">クリック</span>で、それぞれのダイアログのページに対応する解説のページへ移動します。

![本体設定ダイアログPOP](image/config-pop/0.png)
	<map name="configdialog" id="configdialog">
		<area shape="rect" coords="14,31,137,46" href="config-ippan.html" alt="一般">
		<area shape="rect" coords="14,47,137,66" href="config-ghost.html" alt="ゴースト(1)">
		<area shape="rect" coords="14,66,137,82" href="config-ghost2.html" alt="ゴースト(2)">
		<area shape="rect" coords="14,82,137,98" href="config-folder.html" alt="フォルダ">
		<area shape="rect" coords="14,98,137,114" href="config-disp.html" alt="表示">

		<area shape="rect" coords="14,115,137,133" href="config-talk.html" alt="喋り/バルーン">
		<area shape="rect" coords="14,134,137,152" href="config-conn1.html" alt="接続(1)">
		<area shape="rect" coords="14,150,137,168" href="config-conn2.html" alt="接続(2)">
		<area shape="rect" coords="14,167,137,185" href="config-pop.html" alt="POP">
		<area shape="rect" coords="14,184,137,202" href="config-extprog.html" alt="外部アプリ">

		<area shape="rect" coords="14,201,137,219" href="config-im.html" alt="IM">
		<area shape="rect" coords="14,218,137,236" href="config-ipmes.html" alt="IPMessenger">
		<area shape="rect" coords="14,235,137,253" href="config-i18n.html" alt="国際化">
		<area shape="rect" coords="14,252,137,270" href="config-dev.html" alt="開発/その他">
	</map>

このページでは右クリックメニューの「設定」サブメニューにある項目「本体設定」で開くダイアログの、「POP」ページについて解説しています。

SSPのメールが届いているかをチェックする機能に関する設定です。

## 各項目の解説

<dl>
  <dt>メールヘッダも取得する</dt>
  <dd>ゴースト側でメールヘッダ（タイトルなど）を解析できるように、メールヘッダも取ってきます。

ゴーストにヘッダを渡したくない場合は、OFFにしてください。</dd>

  <dt>新着メールの数をメール件数として表示</dt>
  <dd>通常、「メールが&times;&times;通あります」とゴーストが言ってくれるはずですが、この数はサーバ上に残っているメールの数で、新着メールの数ではありません。

この設定を有効にすると、サーバ上にあるメールの数ではなく新着メールの数を喋るようになります。</dd>

  <dt>新着メールがあった時のみメッセージを表示</dt>
  <dd>新着メールが存在した時のみ、ゴーストがメールがあったことを喋ってくれるようになります。</dd>
</dl>

### メール着信時に鳴らす音の設定

新しくメールが届いた場合に、ここで設定した音声ファイルを再生します。

### アカウント設定

アカウントを追加したい場合は「追加」ボタン、削除したい場合は下のリストから選んで「削除」ボタンを押してください。

また、設定を修正したい場合は、「変更」ボタンを押してください。

<dl>
	<dt>アカウント名</dt>
	<dd>
	自分の分かりやすい適当な名前をつけてください。これがメールチェックメニューに現れます。
	</dd>

	<dt>種類</dt>
	<dd>APOP/通常のPOP3/IMAP4に対応しています。

	プロバイダやその他メールサービスの利用説明書を読んで設定してください。

通常はPOP3、もしくはAPOPで接続できると思います。
	</dd>

	<dt>サーバ</dt>
	<dd>
	あなたのメールを保管してあるPOPサーバの場所を入力します。

通常、プロバイダの方からもらった書類に「POPサーバアドレス」といったような項目があるはずなので、それを(半角で)書き写してください。
	</dd>

	<dt>ポート番号</dt>
	<dd>
	通常は標準のままでかまいません。

特別にポート番号を指定されている場合のみ変更してください。
	</dd>

	<dt>ユーザID/パスワード</dt>
	<dd>
	あなたのメールのユーザ名とパスワードを入力します。

インターネット接続用のユーザ名/パスワードとは通常違ったものが割り当てられているはずですので注意してください。</dd>

	<dt>サーバへの接続にSSL/TLSを使う</dt>
	<dd>
	メールサーバに接続する際に、SSL/TLSで暗号化して情報を保護します。

通常は設定しなくても接続できるかと思いますが、GMail等常に設定する必要がある場合もあります。
	</dd>

	<dt>SSL/TLSのサーバ証明書を検証する</dt>
	<dd>
	上記SSL/TLS機能の追加設定項目です。通常はONのまま使用してください。

一部無料サービス等、これをOFFにしないと通信エラーになる場合があります。
	</dd>

	<dt>自動チェック</dt>
	<dd>
	指定した時間おきに自動でメールが届いているかチェックします。

あまり短い時間を設定しないようにしてください。
	</dd>
</dl>

## 下部のボタン

<dl>
	<dt>ヘルプ</dt>
	<dd>
		本体設定ダイアログの、設定中のページのヘルプ（つまりこのページ）を開きます。

ダイアログ右上の「？」マークも同様です。
	</dd>

	<dt>閉じる</dt>
	<dd>
		本体設定ダイアログを閉じます。

ダイアログ右上の「×」マークも同様です。
	</dd>
</dl>

<!-------------------------------------------------------------------------------------------------------------------------------->
<div id="navigation">
	<span class="Prev">[設定：接続(2)](config-conn2.html)</span>
	<span class="Return">[目次](contents.html)</span>
	<span class="Next">[設定：外部アプリ](config-im.html)</span>
</div>
</div>
</body>
</html>