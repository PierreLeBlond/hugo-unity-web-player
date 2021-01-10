# hugo-unity-web-player
gohugo shortcode to embed a unity3d web player

/!\ Has been tested only on unity 2019 /!\

The shortcode is based on unity `index.html` file which is created along a
WebGL build.

### Installation

* Copy `layouts/shortcodes/unity.html` to your hugo project shortcodes folder.

* Instruction about building a Unity3D WebGL project can be found
[here](https://docs.unity3d.com/Manual/webgl-building.html). Once it's done
retrieve these files :
  - Put the content of the `Build` folder within your `static` folder, e.g. at
`static/unity/myGame`.
  - Put the `TemplateData` folder within your newly created
    folder, e.g. at `static/unity/myGame/TemplateData`.

### Usage

```go
{{< unity "/unity/toFixIt/Build/toFixIt.json" ".625" >}}
```

It require two parameters :
- The path to the build output
- The ratio between width and height of your unity project

