# Windows音声認識アプリ
OpenAI の Whisper を使用して音声認識を行い、GPT-5 mini を使用して「えっと」などを除去して、クリップボードに認識結果をコピーします。

## 使用方法
インストールすると、スタートメニューに緑のマイクアイコンの Whisper Speech Recoginition が追加になるので、起動すると、タスクトレイに常駐します。
`Ctrl + Shift + スペース` を押すと、録音が始まり、もう一度 `Ctrl + Shift + スペース` を押すと認識が終了します。
認識結果はクリップボードにコピーされます。

タスクトレイのアイコンを右クリックすると終了できます。

## インストール方法
https://github.com/yukoba/WhisperSpeechRecognition/releases からインストールしてください。

OpenAI を使用しているので API キーは https://platform.openai.com/api-keys から作成してください。
その API キーを環境変数 OPENAI_API_KEY に書くか、もしくは、以下の内容で `%USERPROFILE%\WhisperSpeechRecognition.json` に書いてください。

```json
{
	"OpenAI": {
		"ApiKey": "sk-proj-AAAAAAAAA"
	}
}
```

## ライセンス
アイコンは https://www.flaticon.com/free-icon/circle_14025057 より。ソースコードはMITライセンスです。
