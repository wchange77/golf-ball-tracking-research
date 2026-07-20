# Golf 15 高尔夫追球研究门户

这是一个纯静态研究网页，不依赖 npm、CDN 或后端服务。

在线访问：<https://wchange77.github.io/golf-ball-tracking-research/>

## 打开方式

可直接打开 `index.html`。为确保浏览器对本地资源采用一致策略，建议在项目根目录启动本地服务器：

```bash
python3 -m http.server 8899 --bind 127.0.0.1
```

然后访问：

```text
http://127.0.0.1:8899/exportDoc/golf-ball-tracking-research/index.html
```

## 交互

- `/`：聚焦全局搜索。
- 左侧导航：定位研究地图、流程、模型、公式、训练、证据边界和来源。
- 模型与来源按钮：按类别筛选。
- 公式卡片：打开详细变量解释与工程用途。
- 右上角按钮：切换明暗主题。

研究正文与完整出处见 `高尔夫追球外部研究报告.md`。

## 证据边界

- 自动候选不是训练标签。
- TrackMan 数据只有经过人工确认后才作为强约束。
- 平滑、插值或贝塞尔曲线不能替代 RK4 + drag + Magnus 物理主线。
