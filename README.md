# 世博会记忆图谱 / EXPO Memory Archive

用于课堂发表的静态知识图谱与演示原型，围绕 1970 大阪、2005 爱知与 2025 大阪·关西世博会，连接主题、空间、参与者与档案资料。

节点与关系由人工整理，不包含 GraphRAG 索引、检索或生成能力。设计参考 Microsoft GraphRAG 可视化指南与 KG Visualization。

## 选择入口

| 文件 | 用途 |
| --- | --- |
| [index.html](index.html) | 互动图谱入口 |
| [presentation.html](presentation.html) | 课堂发表演示 |
| [dynamic-presentation.html](dynamic-presentation.html) | 分步呈现的动态演示，含讲稿与关系图交互 |
| `assets/` | 页面引用的本地图片 |

## 本地查看

下载或克隆仓库后，可直接用浏览器打开 HTML 文件。保留 `assets/` 与 HTML 的相对位置，避免图片丢失。

也可在仓库根目录启动静态服务（需要 Python 3）：

```bash
git clone https://github.com/SkkuFintechLiu/expo-archive-graph.git
cd expo-archive-graph
python3 -m http.server 8000 --bind 127.0.0.1
```

访问 [图谱首页](http://127.0.0.1:8000/) 或 [动态演示](http://127.0.0.1:8000/dynamic-presentation.html)。无需安装前端依赖或构建。

动态演示可使用页面按钮，或按以下快捷键：

| 按键 | 操作 |
| --- | --- |
| → / PageDown / 空格 | 展示下一步或下一页 |
| ← / PageUp | 返回上一步或上一页 |
| N | 展开或收起讲稿 |
| F | 切换全屏 |

## 修改内容

文字、关系与样式直接维护在相应 HTML 中。更换图片时同步更新引用路径、图注与来源链接；修改后检查三个入口，确认图片加载、翻页与节点说明正常。

## 资料与解释边界

资料仅用于学习，引用及图像的公开再利用须逐项核实。图中的连线表示整理者选择的资料与问题之间的联系，不代表因果关系。页面中的来源链接用于回到原资料核查，不能替代逐项授权确认。
