[EN](README.md) | 中文

# Star-Rail-Model-Importer (SRMI)

崩坏：星穹铁道导入自定义模型的工具和说明。

#### DISCLAIMER: 我强烈建议只使用私人服务器进行修改。在官方服务器会有被封号的高风险。我不赞成在官方服务器上使用这些工具和程序，如果你依然要在官服上使用，我对由此产生的任何后果不承担责任。

SRMI 是我对 3DMigoto/GIMI 修改后的一个版本，以便与星穹铁道兼容。请注意，这里的很多文件都是从 GIMI 移植过来的，我正在修复它们——其中很多文件可能有兼容性问题，而且可能有一些参考资料仍然指向 GIMI。

你可以随意使用或修改本库内的脚本，但如果你在你的项目中使用这里提供的程序，请注明出处。我将持续更新并修复这个页面，所以请经常回来查看。

故障排除指南: [看这里](Guides/CN_Troubleshooting.md)

星穹铁道的 mod 制作近期才开始, 相关指南仍在编写中。许多技术与 GIMI 相似，想要获得更多的修改帮助，请访问 AGMG 社区。(https://discord.gg/agmg)

导入模型文件在 [SR-Model-Importer-Assets](https://github.com/SilentNightSound/SR-Model-Importer-Assets)

## 安装说明 (3DMigoto)

1. 下载并解压 3dmigoto.zip。我提供了两个版本：

   - "3dmigoto-SRMI-for-development.zip" 是开发者版本，用于创作 mods，但比较慢。
   - "3dmigoto-SRMI-for-playing-mods.zip" 是给玩家的精简版本，它关闭了开发功能（没有绿色文本），速度更快。

2. 加载 3dmigoto，以管理员身份运行`3DMigotoLoader.exe`。注意，这个 exe 是由 python 编译的，所以 Windows 防火墙可能会标记它——如果你在运行 exe 时遇到问题，可能因为它被防火墙阻止了，我也提供了`3DMigotoLoader.py`，它有相同的代码（你将需要安装 psutil 和 pyinjector 依赖项来运行它。）

3. 如果到目前为止一切正常，3DMigoto 应该已被注入到游戏中，你应该可以在游戏中看到绿色文本（只有使用开发者版本才会显示，精简版不显示绿色文本）：

- 注意：加载器显示 “unable to verify if 3dmigoto was loaded” 并不意味着 3dmigoto 未能注入——如果绿色文本/mods 有显示，就没有问题。

4. 安装完成！你现在应该可以使用 3DMigoto 加载自定义 mods 并覆盖贴图和着色器了。想要添加 mods，就把它们放在 Mods 文件夹中（每个角色只能有一个 mod），并在游戏中按 F10 加载。

&nbsp;

## 安装说明 (3DMigoto Blender 插件)

要是你想自行修改游戏模型，你还需要配置 Blender 插件和环境。3DMigoto 插件只适用于 Blender 2.80 以上的版本

注意！如果使用 GIMI 插件，请卸载该版本，改用 SRMI 插件。它们的功能几乎相同，但 SRMI 插件有一个额外的导出选项，用于星穹铁道模型。

1. 下载并安装 Blender

2. 下载并安装修改过的 [3DMigoto 插件](https://github.com/SilentNightSound/SR-Model-Importer/releases)。前往 Edit -> Preferences -> Add-Ons -> Install，选择刚下载的 .py 文件以安装插件。

3. 如果操作正确，你应该会在插件列表中看到 3DMigoto，以及在导入和导出菜单中的新选项。

<img src="https://user-images.githubusercontent.com/107697535/174328624-ccb14ded-57b2-4ac7-b0a0-0de118119174.png" width="800"/>

<img src="https://user-images.githubusercontent.com/107697535/174329025-981a1a9f-7c56-4f44-804b-1b0394b8bd33.png" width="800"/>

&nbsp;

## 致谢

衷心感谢 DarkStarSword，bo3b，和 Chiri 的 3dmigoto!
