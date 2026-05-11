# ar-hokuriku-fish

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

An AR/VR web application showcasing marine life from Japan's Hokuriku region using high-quality, animated 3D models.

The demo displays a realistic 3D model of an Alaskan Pink Shrimp, known in Japan as *Hokkoku Akaebi*. The model is animated and floats in the view, accompanied by a descriptive label in Japanese.

## Features

-   **Web-Based AR/VR:** View animated 3D sea creatures in a web browser, compatible with desktop, mobile, and VR/AR headsets.
-   **High-Quality Animated Models:** Utilizes detailed, animated GLB models for a lifelike experience.
-   **Dynamic Text Labels:** On-screen labels are generated dynamically using HTML Canvas to provide information about the species.
-   **Desktop Controls:** Includes mouse and keyboard controls for easy navigation on a PC.
-   **Extensible:** Easily configured to display other included models like the Snow Crab and Yellowtail.

## How to Run

Because web browsers have security restrictions for loading local files, you'll need to use a local web server to run this project.

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/user/ar-hokuriku-fish.git
    cd ar-hokuriku-fish
    ```

2.  **Start a local server:**
    If you have Python 3, you can run:
    ```sh
    python -m http.server
    ```
    Alternatively, use a tool like the [Live Server extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer).

3.  **Open in your browser:**
    Navigate to `http://localhost:8000` (or the URL provided by your local server).

## Customization

By default, only the Alaskan Pink Shrimp is displayed. You can enable the Snow Crab and Five-ray Yellowtail models by editing the `fns` array in `index.html`:

```javascript
// index.html

// Uncomment the lines for the models you want to display
const fns = [
  "cc0____snow_crab_chionoecetes_opilio.glb", // 18M
  "cc0___alaskan_pink_shrimp_p._eous.glb", // 28M
  "cc0___five-ray_yellowtail_s._quinqueradiata.glb", // 49M
];
```

## Included 3D Models

The repository includes the following 3D models in GLB format:

-   `cc0___alaskan_pink_shrimp_p._eous.glb` (28 MB)
-   `cc0____snow_crab_chionoecetes_opilio.glb` (18 MB)
-   `cc0___five-ray_yellowtail_s._quinqueradiata.glb` (49 MB)

## Credits and Source Models

This project uses the following CC0-licensed 3D models from ffish.asia / floraZia.com.

-   [CC0 ホッコクアカエビ 🦐 Alaskan Pink Shrimp, P. eous - Download Free 3D model by ffish.asia / floraZia.com (@ffishAsia-and-floraZia) [7bf0947]](https://sketchfab.com/3d-models/cc0-alaskan-pink-shrimp-p-eous-7bf09478c7f94b419f1b90261c538e65)
-   [CC0 ブリ 🐟 Five-ray Yellowtail, S. quinqueradiata - Download Free 3D model by ffish.asia / floraZia.com (@ffishAsia-and-floraZia) [e27d30b]](https://sketchfab.com/3d-models/cc0-five-ray-yellowtail-s-quinqueradiata-e27d30bd4d7347238e428a8e36d9fde4)
-   [CC0 ズワイガニ 🦀 ♂ Snow Crab, Chionoecetes opilio - Download Free 3D model by ffish.asia / floraZia.com (@ffishAsia-and-floraZia) [c6495be]](https://sketchfab.com/3d-models/cc0-snow-crab-chionoecetes-opilio-c6495becaa2a4dec8148dd09fcd010ff#download)
