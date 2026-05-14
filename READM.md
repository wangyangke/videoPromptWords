````markdown
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

基于 Prompt Engineering 最佳实践，构建了五维技能体系：

| 技能模块 | 核心功能 |
|----------|----------|
| 结构化 Prompt 建模 | 六维构建法：主体+场景+风格+光影+材质+参数 |
| 视觉摄影与光影控制 | 专业灯光库和镜头库 |
| 艺术媒介与风格合成 | 多风格迁移和艺术家对标 |
| 画质精修与负面工程 | 自动增益修正和逆向过滤 |
| MJ 技术参数调控 | 智能参数匹配 |

### 关键配置

**六维构建法执行逻辑：**
```
[核心主体] + [场景细节] + [艺术风格] + [光影构图] + [材质细节] + [技术参数]
```

**权重优化原则：**
- 遵循"首词优先"原则，将最重要的视觉锚点置于提示词前20%
- 自动添加画质增益词（Photorealistic、Highly Detailed、8K Resolution）
- 自动生成 Negative Prompt 过滤常见 AI 错误

### 情感分析增强配置

根据场景情感自动匹配光影和色彩：
- 悲伤：冷色调、低饱和度、柔和光线
- 喜悦：暖色调、高饱和度、明亮光线
- 愤怒：红色调、强烈对比、硬光
- 恐惧：深蓝色/紫色调、低光、阴影强烈
- 浪漫：粉色/金色调、柔光、散景效果

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
A cute little girl around 6-8 years old dancing joyfully in a beautiful flower garden, wearing a flowing pink dress that swirls as she twirls, surrounded by colorful blooming roses and lavender, butterflies fluttering around her, golden hour sunlight filtering through the trees creating dappled light patterns on the grass...

负面提示词：
extra limbs, distorted faces, blurry textures, low quality, pixelated, watermark...

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
A young boy around 8-10 years old swimming joyfully in a clear pond on a sunny summer day, splashing water with his hands, sunlight filtering through the water surface creating shimmering patterns on his skin, wet hair sticking to his forehead, bright blue swim trunks, ripples spreading across the pond, green lily pads floating nearby, trees and blue sky reflected in the water, golden hour sunlight casting warm glow, photorealistic style with ultra-detailed textures on water droplets and skin... --ar 16:9 --stylize 200 --v 6.0
Negative prompt: extra limbs, distorted faces, blurry textures, low quality, pixelated, watermark...
```

**效果对比：**
| 维度 | 使用前 | 使用后 |
|------|--------|--------|
| 细节丰富度 | 低 | 高 |
| 光影控制 | 无 | 专业灯光设置 |
| 构图指导 | 无 | 镜头参数配置 |
| 风格一致性 | 不确定 | 精准风格定义 |
| 画质保证 | 无 | 自动增益修正 |
| 错误过滤 | 无 | 自动负面过滤 |

---

## 6、Skill 链接

- **Skill 位置**：`/Users/admin/.trae-cn/skills/ai-prompt-engineer/`
- **核心文件**：[SKILL.md](file:///Users/admin/.trae-cn/skills/ai-prompt-engineer/SKILL.md)
- **说明文档**：[DOCUMENTATION.md](file:///Users/admin/.trae-cn/skills/ai-prompt-engineer/DOCUMENTATION.md)

---

## 7、总结与思考

### 收获与效率提升

通过使用这个 Skill，创作者可以获得以下提升：

1. **效率提升**：提示词生成时间从平均 5-10 分钟缩短到几秒钟
2. **质量提升**：生成图片的精准度和艺术质量显著提高
3. **知识门槛降低**：无需专业摄影和艺术知识也能生成专业级提示词
4. **一致性保障**：每次生成的提示词都遵循统一的专业标准

### 最满意的地方

1. **六维构建法**：系统性地将创意转化为结构化提示词
2. **情感分析增强**：根据场景情感自动匹配光影和色彩
3. **自动负面过滤**：智能排除常见 AI 生成错误
4. **短剧场景优化**：针对视频创作场景进行了专项优化

### 后续优化方向

1. **多语言支持**：增加中英文双语提示词生成
2. **风格模板库**：预设更多场景风格模板
3. **动态参数调整**：根据用户反馈智能调整参数
4. **视频分镜生成**：支持生成完整的视频分镜脚本
5. **用户自定义词库**：允许用户添加自定义的风格和词汇

### 体验建议

欢迎体验「AI 绘图提示词专家」Skill！建议尝试以下场景：

1. **情感特写**："一个孤独的老人坐在海边看日落"
2. **动作场面**："超级英雄在城市上空飞翔，身后是爆炸的火光"
3. **悬疑氛围**："深夜的废弃医院走廊，灯光闪烁"
4. **浪漫场景**："情侣在樱花树下牵手，花瓣飘落"

如果您有任何建议或改进想法，欢迎反馈！

---

*文档创建日期：2026年5月*

````

