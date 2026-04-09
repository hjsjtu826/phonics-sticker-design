---
name: "phonics_sticker_design"
description: "Creates cute educational phonics sticker designs for Xiaohongshu. Invoke when user wants to generate phonics learning materials or sticker designs for children."
---

# 拼音贴纸设计技能

这个技能用于创建可爱的教育拼音贴纸设计，专为小红书平台优化，适合儿童拼音学习。

## 功能特点

- 🎨 生成符合小红书风格的拼音贴纸设计
- 📚 教育性强，适合儿童拼音学习
- 🎯 支持自定义核心词汇和人物特征
- 🎨 自动应用可爱的2D插画风格
- 📐 3:4比例，适合小红书平台展示

## 使用方法

### 输入参数

- `core_word`: 核心词汇（必填）
- `target_letter`: 首字母/目标音素（必填）
- `subject_description`: 人物特征和动作描述（英文，必填）
- `main_subject`: 主体描述（英文，必填）

### 输出结果

- `prompt`: 生成贴纸设计的完整提示词
- `image_size`: 推荐的图片尺寸（portrait_4_3）

## 使用示例

### 示例1：苹果贴纸

```json
{
  "core_word": "apple",
  "target_letter": "A",
  "subject_description": "A cute little girl with pigtails, wearing a red dress, happily holding a shiny red apple",
  "main_subject": "A happy girl holding an apple"
}
```

### 示例2：球贴纸

```json
{
  "core_word": "ball",
  "target_letter": "B",
  "subject_description": "A cute little boy with short hair, wearing a blue shirt, playing with a colorful bouncing ball",
  "main_subject": "A boy playing with a ball"
}
```

## 设计规范

- **视觉风格**: 可爱的2D儿童绘本插画风格
- **布局**: 3:4比例，顶部目标字母，中间插图，底部核心词汇
- **颜色**: 柔和的 pastel 背景，明亮的糖果色主体
- **字体**: 粗体、圆润、气泡状的儿童友好字体
- **边框**: 厚白色描边，营造贴纸效果

## 文件结构

- `skill.json`: 技能描述文件，包含核心模板和配置
- `config.yaml`: 技能配置文件，定义参数和执行逻辑
- `README.md`: 使用说明文档

## 许可证

MIT License