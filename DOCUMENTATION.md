# AI 绘图提示词专家 Skill 介绍文档

---

## 1、Skill 简介

这是一个帮助 AI 绘图/视频创作者快速生成专业结构化提示词的 Skill，通过六维构建法将简单模糊的创意转化为高质量的 AI 绘图指令，适合需要频繁生成图片或视频场景的短剧创作者、设计师和内容运营使用。

---

## 2、使用场景

### 为什么想做它？
在使用 MidJourney、Stable Diffusion 等 AI 绘图工具时，经常遇到以下问题：
- 不知道如何描述才能让 AI 生成符合预期的图像
- 提示词过于简单导致生成结果质量低下
- 反复调整提示词浪费大量时间
- 不了解专业的光影、构图、风格术语

### 之前遇到的麻烦？
- 输出结果与预期相差甚远
- 需要反复尝试才能找到合适的提示词组合
- 缺乏专业的摄影和艺术知识
- Negative Prompt 需要手动添加，容易遗漏常见问题

### 做出来之后能省掉哪些动作？
- 省去学习专业摄影知识的时间
- 省去反复调试提示词的过程
- 省去手动编写 Negative Prompt 的步骤
- 一键生成符合专业标准的完整提示词

---

## 3、创作过程

### 核心设计思路

基于 Prompt Engineering 最佳实践，构建了十维技能体系：

| 技能模块 | 核心功能 |
|----------|----------|
| 结构化 Prompt 建模 | 六维构建法：主体+场景+风格+光影+材质+参数 |
| 视觉摄影与光影控制 | 专业灯光库（12种光效）和镜头库（12种镜头） |
| 艺术媒介与风格合成 | 多风格迁移（16种风格）和艺术家对标（12位艺术家） |
| 画质精修与负面工程 | 自动增益修正和逆向过滤（30+负面词） |
| MJ 技术参数调控 | 智能参数匹配（比例、风格化、混乱度） |
| 场景类型与情感匹配 | 12种场景类型适配矩阵 |
| 时代背景与地域文化适配 | 6个时代 + 6个地域文化特征 |
| 角色与人物细节库 | 年龄状态 + 情绪表达 |
| 环境与场景元素库 | 自然环境 + 城市环境 |
| 天气与时间特效 | 8种天气 + 7种时间特效 |

### 关键配置

**六维构建法执行逻辑：**
```
[核心主体] + [场景细节] + [艺术风格] + [光影构图] + [材质细节] + [技术参数]
```

**权重优化原则：**
- 遵循"首词优先"原则，将最重要的视觉锚点置于提示词前20%
- 自动添加画质增益词（Photorealistic、Highly Detailed、8K Resolution等）
- 自动生成 Negative Prompt 过滤常见 AI 错误

### 场景类型适配矩阵

| 场景类型 | 光影风格 | 镜头选择 | 推荐风格 |
|----------|----------|----------|----------|
| 情感特写 | 柔光/侧光/轮廓光 | 特写/中景 | 写实/动漫/水彩 |
| 动作场面 | 硬光/逆光/舞台灯光 | 全景/动态模糊 | 赛博朋克/写实/UE5 |
| 悬疑氛围 | 低光/阴影/烛光 | 俯拍/仰拍/特写 | 暗黑风格/超现实 |
| 浪漫场景 | 黄金时段/柔光/月光 | 中景/特写/全景 | 唯美/水彩/油画 |
| 科幻场景 | 霓虹灯/体积光/荧光 | 广角/低角度/远景 | UE5渲染/赛博朋克 |
| 历史场景 | 自然光/侧光/烛光 | 全景/中景 | 油画/写实/浮世绘 |
| 恐怖场景 | 低光/阴影/背光 | 特写/仰拍 | 暗黑风格/超现实 |
| 喜剧场景 | 明亮柔光/自然光 | 中景/全景 | 写实/动漫 |
| 史诗场景 | 体积光/逆光/自然光 | 远景/全景/低角度 | UE5渲染/油画 |
| 温馨日常 | 柔光/自然光/侧光 | 中景/特写 | 写实/水彩 |
| 战争场景 | 硬光/烟雾/逆光 | 全景/动态模糊 | 写实/UE5渲染 |
| 幻想场景 | 体积光/魔法光效 | 广角/低角度 | 动漫/超现实/宫崎骏风格 |

---

## 4、使用步骤

### 调用方式

1. **触发方式**：在 SOLO 中直接描述您的创意场景
2. **格式要求**：自然语言描述即可，无需特定格式

### 操作步骤

```
步骤 1：打开 SOLO，进入技能中心
步骤 2：启用「AI 绘图提示词专家」Skill
步骤 3：在聊天框中输入您的场景描述，例如：
        "一个小女孩在花园里跳舞"
步骤 4：Skill 自动解析并生成专业提示词
步骤 5：复制生成的完整指令到 AI 绘图工具中使用
```

### 输入输出示例

**输入：**
```
一个小女孩在花园里跳舞
```

**输出：**
```
正面提示词：
A cute little girl around 6-8 years old dancing joyfully in a beautiful flower garden, wearing a flowing pink dress that swirls as she twirls, surrounded by colorful blooming roses and lavender, butterflies fluttering around her, golden hour sunlight filtering through the trees creating dappled light patterns on the grass, dewdrops glistening on flower petals, her hair tied in pigtails with ribbons, bare feet on the soft green grass, joyful expression with sparkling eyes, photorealistic style with ultra-detailed textures on fabric and flowers, cinematic composition with shallow depth of field, Professional Lighting, Sharp Focus, Highly Detailed, 8K Resolution, Cinematic Quality, Ultra Realistic

负面提示词：
extra limbs, distorted faces, blurry textures, low quality, pixelated, watermark, text, signature, mutated, malformed, disfigured, unrealistic proportions, bad anatomy, duplicate, poorly drawn, ugly, cartoon style, anime style

完整MJ指令：
[正面提示词] --ar 16:9 --stylize 200 --v 6.0
Negative prompt: [负面提示词]
```

---

## 5、效果展示

### 使用前（原始描述）

```
一个小男孩在池塘里游泳
```

**问题分析：**
- 过于简单，缺乏细节描述
- AI 无法准确理解场景
- 生成结果可能不符合预期

### 使用后（专业提示词）

```
A young boy around 8-10 years old swimming joyfully in a clear pond on a sunny summer day, splashing water with his hands, sunlight filtering through the water surface creating shimmering patterns on his skin, wet hair sticking to his forehead, bright blue swim trunks, ripples spreading across the pond, green lily pads floating nearby, trees and blue sky reflected in the water, golden hour sunlight casting warm glow, photorealistic style with ultra-detailed textures on water droplets and skin, cinematic composition with shallow depth of field, Professional Lighting, Sharp Focus, Highly Detailed, 8K Resolution, Cinematic Quality, Ultra Realistic --ar 16:9 --stylize 200 --v 6.0
Negative prompt: extra limbs, distorted faces, blurry textures, low quality, pixelated, watermark, text, signature, mutated, malformed, disfigured, unrealistic proportions, bad anatomy, duplicate, poorly drawn, ugly, cartoon style, anime style
```

**效果对比：**
| 维度 | 使用前 | 使用后 |
|------|--------|--------|
| 细节丰富度 | 低 | 高 |
| 光影控制 | 无 | 专业灯光设置（Golden Hour） |
| 构图指导 | 无 | 镜头参数配置（Depth of Field） |
| 风格一致性 | 不确定 | 精准风格定义（Photorealistic） |
| 画质保证 | 无 | 自动增益修正（8K、Highly Detailed） |
| 错误过滤 | 无 | 自动负面过滤（30+负面词） |
| 情感表达 | 无 | 喜悦、活力 |
| 场景感 | 弱 | 强 |

---

## 6、Skill 链接

- **Skill 位置**：`/Users/admin/Desktop/trae-video-skill/`
- **核心文件**：[SKILL.md](file:///Users/admin/Desktop/trae-video-skill/SKILL.md)
- **说明文档**：[DOCUMENTATION.md](file:///Users/admin/Desktop/trae-video-skill/DOCUMENTATION.md)

---

## 7、总结与思考

### 收获与效率提升

通过使用这个 Skill，创作者可以获得以下提升：

1. **效率提升**：提示词生成时间从平均 5-10 分钟缩短到几秒钟
2. **质量提升**：生成图片的精准度和艺术质量显著提高
3. **知识门槛降低**：无需专业摄影和艺术知识也能生成专业级提示词
4. **一致性保障**：每次生成的提示词都遵循统一的专业标准
5. **场景覆盖广**：支持 12 种场景类型、6 个时代背景、6 个地域文化

### 最满意的地方

1. **十维技能体系**：系统性地覆盖了提示词生成的各个维度
2. **场景类型适配矩阵**：一键匹配最合适的光影、镜头和风格
3. **情感分析增强**：根据场景情感自动匹配光影和色彩
4. **自动负面过滤**：智能排除常见 AI 生成错误
5. **短剧场景优化**：针对视频创作场景进行了专项优化

### 后续优化方向

1. **多语言支持**：增加中英文双语提示词生成
2. **风格模板库**：预设更多场景风格模板
3. **动态参数调整**：根据用户反馈智能调整参数
4. **视频分镜生成**：支持生成完整的视频分镜脚本
5. **用户自定义词库**：允许用户添加自定义的风格和词汇
6. **实时预览功能**：根据提示词生成缩略图预览

### 体验建议

欢迎体验「AI 绘图提示词专家」Skill！建议尝试以下场景：

1. **情感特写**："一个孤独的老人坐在海边看日落"
2. **动作场面**："超级英雄在城市上空飞翔，身后是爆炸的火光"
3. **悬疑氛围**："深夜的废弃医院走廊，灯光闪烁"
4. **浪漫场景**："情侣在樱花树下牵手，花瓣飘落"
5. **科幻场景**："未来都市的雨夜，一个神秘人站在高楼边缘"
6. **历史场景**："中世纪城堡的宴会厅，骑士们围坐讨论"

如果您有任何建议或改进想法，欢迎反馈！

---

*文档创建日期：2026年5月*
