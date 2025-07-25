# Enigma_01 ビルドガイド  

ここではキーマップ編集の手順を説明します。総合案内は[こちら](https://github.com/nazuna293/Enigma_01)です。

## 目次
+ [キーマップ編集](#1-キーマップ編集)  
  + [KeymapEditor](#KeymapEditor)  
  + [ZMK Studio](#ZMK-Studio)  
+ [Enigma_01の起動](#2-Enigma_01の起動)

## キーマップ編集  

2つの方法を案内します。
複雑な編集はKeymapEditorが適していますが、初めての編集はZMK Studioがおすすめです。  

|項目|KeymapEditor<br>[編集手順](#KeymapEditor)|ZMK Studio<br>[編集手順](#ZMK-Studio)|  
|:-:|:-|:-|  
|事前準備|GitHubのアカウント登録<br>リポジトリのフォーク、登録|特になし|  
|編集方法|ブラウザ上でマウス操作→ファームウェアの書き出し、転送|ブラウザ上でマウス操作→ブラウザ上で上書き保存|  
|編集項目| マクロ等も編集できる|標準的な編集ができる|  

### KeymapEditor
#### GitHubリポジトリのフォーク  
ファームウェアはGitHub Actionsで書き出します。  
1. GitHubアカウントを持っていない場合は、事前に[アカウント登録](https://github.com/signup)をしてください。  
2. 準備できたらEnigma_01の[リポジトリ](https://github.com/nazuna293/zmk-config-Enigma_01)をフォークします。  

#### ファームウェアをEnigma_01へ
以下の手順で転送しましょう。
1. GitHub Actionsからファームウェアをダウンロード、解凍する
2. Enigma_01とパソコンをUSB-Cケーブルで接続します
3. 本体のリセットボタンを2回押します
4. フォルダに「XIAO SENSE」が表示されたらEnigma_01 rgbled_adapter.uf2を貼り付けます
5. 接続が解除、数秒後に復帰します
これでファームウェアの転送は完了しました。

### ZMK Studio  
#### ブラウザ上で接続
以下の手順で接続しましょう。
1. Enigma_01とパソコンをUSB-Cケーブルで接続します
2. ブラウザ上で[ZMK Studio](https://zmk.studio)を開きます
3. を選択します

#### キーマップの編集  
ブラウザ上で、

## デバイスと再接続  
### 有線接続の場合  
数秒待てば再接続されます。  

### 無線接続の場合  
ペアリング情報がリセットされているので、再ペアリングが必要です。
1. BT_SEL0でメインデバイスとペアリングする
2. BT_SEL1~SEL4でサブデバイスとペアリングする

**BT_CLR_ALL**でペアリング情報をクリアすることもできる
