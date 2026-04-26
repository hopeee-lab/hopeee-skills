# GPT-Image-2 Prompt 助手

当用户想生成图片、寻找prompt模板、或需要GPT-Image-2的prompt参考时触发，触发词：生成图片、写prompt、帮我画、根据xxx生成一个xxx、类似xxx的图、prompt模板、图生文

从两个GitHub项目库中搜索对应的prompt模板

## 数据位置

- **库1（EvoLink）**：`https://github.com/EvoLinkAI/awesome-gpt-image-2-prompts`（中文 README：README_zh-CN.md）
- **库2（YouMind）**：`https://github.com/YouMind-OpenLab/awesome-gpt-image-2`（中文 README：README_zh.md，Web Gallery：youmind.com/gpt-image-2-prompts）

---

## 使用方式

### Step 1: 理解需求场景
确定用户想生成什么类型的图片，映射到以下类别，并确定优先搜索哪个库：

| 场景 | 类别关键词 | 优先库 |
|------|-----------|--------|
| 人像、照片、自拍、肖像 | portrait/人像 | 两库均有 |
| 海报、插画、平面设计 | poster/海报 | 两库均有 |
| 角色、人物、动漫、游戏角色 | character/角色 | 两库均有 |
| UI、截图、界面、社交媒体 | ui/UI | 两库均有 |
| 对比、测试、评测 | comparison/对比 | 库1 |
| 信息图、教学可视化 | infographic/信息图 | 库2 |
| YouTube封面、缩略图 | youtube-thumbnail | 库2 |
| 漫画、分镜 | comic/storyboard | 库2 |
| 产品营销、电商主图 | product-marketing/ecommerce | 库2 |
| 游戏资产 | game-asset | 库2 |
| App/Web 设计 | app-web-design | 库2 |
| 电影感、摄影 | cinematic/photography | 库2 |
| 3D渲染、等轴测图 | 3d-render/isometric | 库2 |
| Chibi、Q版 | chibi-q-style | 两库均有 |
| 像素艺术 | pixel-art | 库2 |
| 油画、水彩 | oil-painting/watercolor | 库2 |
| 水墨、中国风 | ink-chinese-style | 库2 |
| 复古、赛博朋克 | retro/cyberpunk | 库2 |
| 极简风 | minimalism | 库2 |
| 食物、饮料 | food-drink | 库2 |
| 动物、生物 | animal-creature | 库2 |
| 建筑、室内 | architecture-interior | 库2 |
| 风景、自然 | landscape-nature | 库2 |
| 城市、街道 | cityscape-street | 库2 |
| 文字、排版设计 | text-typography | 库2 |

### Step 2: 搜索案例
根据场景从对应库读取README，找到最匹配的案例：

**库1（EvoLink）关键词参考：**
- 人像类：便利店、霓虹、电影感、温泉、闪光灯、自拍、卧室、cosplay
- 海报类：城市、旅行、美食地图、中式、剪纸、手绘、任天堂
- 角色类：动漫、Persona5、Galgame、Chibi、角色表
- UI类：笔记本、手机截图、社交媒体、抖音、X页面
- 对比类：GPT vs Banana、文字渲染、细节

**库2（YouMind）关键词参考：**
- 可直接在 youmind.com/gpt-image-2-prompts 按分类筛选浏览
- Profile/Avatar、Social Media Post、Infographic、YouTube Thumbnail
- Anime/Manga、3D Render、Watercolor、Cyberpunk/Sci-Fi
- Portrait、Character、Product、Food/Drink、Architecture

### Step 3: 返回Prompt模板
从README中提取对应的prompt内容：
- **库1**：找到 "**提示词：**" 后面的内容
- **库2**：找到 "#### 📝 Prompt" 下方代码块内容
- 返回完整的prompt模板

---

## 输出格式

返回时包含：
1. 来源（库1 EvoLink / 库2 YouMind）+ 匹配到的最相似案例
2. 根据用户需求修改后的prompt
3. 可调整的部分说明

```markdown
## 案例：[案例名称] → 改成你的需求
**来源**：[库1 EvoLink / 库2 YouMind]

**Prompt：**
```
[修改后的完整prompt]
```

**使用建议：**
- [可调整的关键部分，如：地标、建筑、颜色、风格等]
- [参数调整建议：比例、构图、排版等]
```

### 输出示例

**用户需求**：生成一张广东佛山的城市宣传海报

**找到的相似案例**：广州城市海报

```markdown
## 案例：2026 广州春季城市海报 → 改成佛山
**来源**：库1 EvoLink

**Prompt：**
```
一张充满新春喜庆氛围但不失高雅格调的 2026 城市宣传海报。
双重曝光，构图延续了S型的流动感；
一条S形的河流贯穿画面，仿佛撕开纸面后露出的内部景象，河水以深浅不一的蓝色渲染，层次分明；
河流中叠加了佛山城市手绘图，国潮风格，景色尽收眼底，壮阔雄伟。
佛山的地标建筑（佛山祖庙、岭南天地、世纪莲体育中心、顺德欢乐海岸plus、珠江夜游、功夫小镇、顺德美食）。
云雾环绕，仙气缥缈，色彩丰富，结构复杂，细节丰富，大面积留白，画面清新脱俗。
左下角排版"SPRING 2026"和竖排宣传语，整体寓意"岭南之都，魅力佛山"。
```

**使用建议：**
- **地标**：换成佛山的（祖庙、岭南天地、世纪莲、顺德欢乐海岸等）
- **宣传语**：改成"岭南之都，魅力佛山"或其他
- **季节**：Spring 2026 → 看你需求
- **风格**：S型河流 + 国潮风 / 剪纸风
```
