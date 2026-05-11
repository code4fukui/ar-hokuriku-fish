# ar-hokuriku-fish

日本北陸地方の海洋生物を、高品質なアニメーション付き3Dモデルで紹介するAR/VRウェブアプリケーションです。

デモでは、日本では「ホッコクアカエビ」として知られるAlaskan Pink Shrimpのリアルな3Dモデルを表示します。モデルはアニメーション付きで画面内に浮かび、日本語の説明ラベルが添えられます。

## 機能

- **ウェブベースのAR/VR:** デスクトップ、モバイル、VR/ARヘッドセットに対応し、ウェブブラウザ上でアニメーション付きの3D海洋生物を閲覧できます。
- **高品質なアニメーションモデル:** 詳細なアニメーション付きGLBモデルを使用し、リアルな体験を提供します。
- **動的なテキストラベル:** HTML Canvasを使用して画面上のラベルを動的に生成し、生物の情報を提供します。
- **デスクトップ操作:** PCでのナビゲーションを容易にする、マウスとキーボードによる操作機能を備えています。
- **拡張性:** ズワイガニやブリなど、同梱されている他のモデルも表示できるように簡単に設定を変更できます。

## 実行方法

ウェブブラウザにはローカルファイルの読み込みに関するセキュリティ制限があるため、このプロジェクトを実行するにはローカルウェブサーバーを使用する必要があります。

1. **リポジトリのクローン:**
    ```sh
    git clone https://github.com/user/ar-hokuriku-fish.git
    cd ar-hokuriku-fish
    ```

2. **ローカルサーバーの起動:**
    Python 3がインストールされている場合は、以下のコマンドを実行できます:
    ```sh
    python -m http.server
    ```
    または、[Live Server extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)などのツールを使用してください。

3. **ブラウザで開く:**
    `http://localhost:8000`（またはローカルサーバーが提供するURL）にアクセスします。

## カスタマイズ

デフォルトではホッコクアカエビのみが表示されます。`index.html`内の`fns`配列を編集することで、ズワイガニやブリのモデルを有効にできます。

```javascript
// index.html

// 表示したいモデルの行のコメントを解除してください
const fns = [
  "cc0____snow_crab_chionoecetes_opilio.glb", // 18M
  "cc0___alaskan_pink_shrimp_p._eous.glb", // 28M
  "cc0___five-ray_yellowtail_s._quinqueradiata.glb", // 49M
];
```

## 同梱されている3Dモデル

リポジトリには、GLB形式の以下の3Dモデルが含まれています:

- `cc0___alaskan_pink_shrimp_p._eous.glb` (28 MB)
- `cc0____snow_crab_chionoecetes_opilio.glb` (18 MB)
- `cc0___five-ray_yellowtail_s._quinqueradiata.glb` (49 MB)

## クレジットとソースモデル

このプロジェクトでは、ffish.asia / floraZia.com が提供する以下のCC0ライセンスの3Dモデルを使用しています。

- [CC0 ホッコクアカエビ 🦐 Alaskan Pink Shrimp, P. eous - Download Free 3D model by ffish.asia / floraZia.com (@ffishAsia-and-floraZia) [7bf0947]](https://sketchfab.com/3d-models/cc0-alaskan-pink-shrimp-p-eous-7bf09478c7f94b419f1b90261c538e65)
- [CC0 ブリ 🐟 Five-ray Yellowtail, S. quinqueradiata - Download Free 3D model by ffish.asia / floraZia.com (@ffishAsia-and-floraZia) [e27d30b]](https://sketchfab.com/3d-models/cc0-five-ray-yellowtail-s-quinqueradiata-e27d30bd4d7347238e428a8e36d9fde4)
- [CC0 ズワイガニ 🦀 ♂ Snow Crab, Chionoecetes opilio - Download Free 3D model by ffish.asia / floraZia.com (@ffishAsia-and-floraZia) [c6495be]](https://sketchfab.com/3d-models/cc0-snow-crab-chionoecetes-opilio-c6495becaa2a4dec8148dd09fcd010ff#download)

## ライセンス

3Dモデルは[CC0 1.0 Universal](http://creativecommons.org/publicdomain/zero/1.0/)ライセンスの下で提供されています。ソースコードはオープンソースです。
