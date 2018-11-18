## あなたが必要とするもの



### Software

#### Software installation

Minecraftは、2014年9月以降、Raspbianにデフォルトでインストールされています。

![Minecraft Pi desktop icon](images/minecraft-pi-shortcut.png)

古いバージョンのRaspbianを使用している場合は、ターミナルウィンドウを開き、次のコマンドを入力します（オンラインにする必要があります）。

```bash
sudo apt-get update
sudo apt-get install minecraft-pi
```

それが終わったら、Minecraft PiとPythonライブラリをインストールする必要があります。

#### Test Minecraft

To run Minecraft double click the desktop icon or enter `minecraft-pi` in the terminal.

![](images/mcpi-start.png)

Minecraft Piがロードされたら、** Start Game **をクリックし、** New create **をクリックします。ウィンドウを含むウィンドウがわずかにオフセットされていることがわかります。これは、あなたがMinecraftウィンドウの後ろのタイトルバーをつかむ必要があるウィンドウをドラッグすることを意味します。

![](images/mcpi-game.png)

あなたは今、Minecraftのゲームに入っています！

#### Test Python

Minecraftが走って世界が創り出されたら、あなたのマウスを解放する `Tab`キーを押して、あなたの焦点をゲームから遠ざけてください。デスクトップ上でPython 3（IDLE）を開き、ウィンドウが並んでいるように移動します。

Pythonウィンドウに直接コマンドを入力するか、ファイルを作成してコードを保存してもう一度実行することができます。

ファイルを作成したい場合は、 `File> New window`と` File> Save`に行きます。ホームフォルダまたは新しいプロジェクトフォルダに保存することをお勧めします。

まず、Minecraftライブラリをインポートし、ゲームへの接続を作成し、画面に「Hello world」というメッセージをポストしてテストします。

```python
from mcpi import minecraft

mc = minecraft.Minecraft.create()

mc.postToChat("Hello world")
```

コマンドをPythonウィンドウに直接入力する場合は、各行の後に `Enter`を打ちます。ファイルの場合は `Ctrl + S 'で保存し、` F5`で実行してください。コードが実行されると、ゲームの画面にメッセージが表示されます。

![](images/mcpi-idle.png)

Minecraftウィンドウで「Hello world」が表示されたら、次のステップに進むとよいでしょう。
