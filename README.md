# UE4_CustomGridShader
UE4向けグリッドシェーダー 

対応バージョン UE4.24.3  

<img width="597" alt="customgrid" src="https://user-images.githubusercontent.com/2414102/77856323-4c763280-7231-11ea-8683-430a0cec83d3.png">

# 概要
テクスチャ未使用のシェーダーのみのグリッドシェーダー  
ワールドの原点を中心に３種類のグリッドラインの線の色・太さ・間隔、背景カラーが設定可能です  
テストステージを作成する際などにご活用ください  

# 使い方

* プロジェクト一式Cloneした後、CustomGridフォルダを同じ階層のまま自分のプロジェクトにコピーするか、
[UE4] 他プロジェクトからアセットを移動させる方法  
https://historia.co.jp/archives/275/  
などでCustomGridフォルダ以下をお好きなプロジェクトに移動させてください

* デフォルトのグリッドからカスタムしたい場合は、CustomGrid/Materials/MT_CustomGrid からマテリアルインスタンスを作成しパラメータを変更してください
<img width="741" alt="materialinstance" src="https://user-images.githubusercontent.com/2414102/77820265-5f4f1100-7124-11ea-8c5c-0ff1008f88d9.png">

* あとはお好きなモデルにマテリアルを割り当てるとグリッドが表示されます

# シェーダーの各種パラメータ説明

| パラメータ | 説明 |
| ------------- | ------------- |
| BackgroundColor  | 背景色  |
| GridColorMidele  | 中くらいの細かさのグリッドの色設定 |
| GridColorNarrow  | 一番細かいグリッドの色設定。一番下に描かれる |
| GridColorWide    | 基準となるグリッドの色設定。一番上に描かれる |
|     |  |
| Blink  | 0以外を入れると点滅するようになります。Emissiveの値を0以上にする必要があります。 |
| Emissive    | Wide/Midele のグリッドのエミッシブカラーの調整用 |
| LineIntervalMiddle  | グリッドの間隔(中)。※単位はメートルです。 |
| LineIntervalNarrow  | グリッドの間隔(細) ※単位はメートルです。|
| LineIntervalWide  | グリッドの間隔(広) ※単位はメートルです。|
| LineSizeMiddle  | グリッド太さ(中) |
| LineSizeNarrow  | グリッド太さ(細) |
| LineSizeWide  | グリッド太さ(広) |
| Metallic  | 1.0に近づくほど金属っぽい表現になります |
| Roughness  | 1.0に近づくほどざらざらになります |

# ライセンス

MIT
