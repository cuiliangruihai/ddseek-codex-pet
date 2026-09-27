# ddseek · Codex 宠物

**ddseek** 是一只戴眼镜、穿薄荷绿衬衫、会指路的动画宠物。它沿用此前完成的角色设计，现以 `ddseek` 作为宠物 ID 和显示名称发布。

<p align="center">
  <img src="previews/contact-sheet.png" width="560" alt="ddseek 的动画精灵图总览">
</p>

## 预览

### 16 个注视方向

![ddseek 顺时针转动视线的动画](previews/direction-cycle.gif)

[打开或下载 16 方向 MP4 预览](previews/ddseek-demo.mp4) · [查看静态方向总览](previews/look-directions.png)

### 标准动画

| 待机 | 挥手 | 跳跃 |
|---|---|---|
| ![待机](previews/animations/idle.gif) | ![挥手](previews/animations/waving.gif) | ![跳跃](previews/animations/jumping.gif) |

全部动画：`idle`、`waving`、`waiting`、`review`、`failed`、`jumping`、`running`、`running-left`、`running-right`。GIF 文件在 [`previews/animations`](previews/animations/) 中。

## 精灵图规格

- Codex v2 宠物格式，`spriteVersionNumber: 2`
- 图集尺寸：1536 × 2288 像素，RGBA
- 布局：8 列 × 11 行，每格 192 × 208 像素
- 第 0–8 行：9 种标准动画
- 第 9–10 行：16 个顺时针注视方向

## 安装

在仓库目录运行以下命令，将配置和图集复制到当前 Codex 用户的宠物目录：

```sh
PET_DIR="${CODEX_HOME:-$HOME/.codex}/pets/ddseek"
mkdir -p "$PET_DIR"
cp pet.json spritesheet.webp "$PET_DIR/"
```

安装后，重启或刷新 Codex 的宠物选择界面以载入 `ddseek`。如果你的 Codex 环境使用自定义 `CODEX_HOME`，上面的命令会自动使用该位置。

## 让 Codex 帮你安装的提示词

复制下面这段，交给 Codex：

> 请帮我安装并配置 Codex 宠物 ddseek。仓库地址是 https://github.com/cuiliangruihai/ddseek-codex-pet 。请先检查仓库里的 `pet.json` 和 `spritesheet.webp`，确认宠物 ID 与显示名称是 `ddseek`，并使用 `spriteVersionNumber: 2`。然后根据我当前 Codex 环境实际使用的宠物目录，将这两个文件安装到 `pets/ddseek/`；如果同名目录已存在，请先备份再更新。最后核对文件和图集尺寸，并告诉我如何在 Codex 中刷新或启用这只宠物。不要更改其他宠物设置。

## 许可与署名

本仓库中的角色图稿、精灵图和预览采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)。转载时请注明：**“ddseek by @cuiliangruihai, licensed under CC BY 4.0.”** 如果修改后再发布，请说明改动。许可详情见 [`LICENSE`](LICENSE)。

该角色由 AI 辅助创作，参考了一张用户提供的照片。原始照片没有包含在仓库中。本许可仅覆盖贡献者有权授权的内容，不授予人物肖像、隐私或第三方权利。

---

# ddseek · Codex Pet

**ddseek** is an animated Codex pet: a cheerful bespectacled helper in a mint-green shirt, pointing the way.

## Preview

![ddseek animation contact sheet](previews/contact-sheet.png)

![ddseek looking through 16 directions](previews/direction-cycle.gif)

[Open or download the 16-direction MP4 preview](previews/ddseek-demo.mp4) · [Static direction sheet](previews/look-directions.png)

The v2 atlas is 1536 × 2288 pixels, RGBA, arranged as 8 columns by 11 rows. Rows 0–8 contain the nine standard animations. Rows 9–10 contain 16 clockwise look directions. Each cell is 192 × 208 pixels.

Install `pet.json` and `spritesheet.webp` into `${CODEX_HOME:-$HOME/.codex}/pets/ddseek/`. The Chinese section above includes copy-ready commands and a prompt for asking Codex to install the pet.

The artwork and previews are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit “ddseek by @cuiliangruihai” and note modifications. The original reference photo is not included; this license does not grant rights held by the subject or third parties.
