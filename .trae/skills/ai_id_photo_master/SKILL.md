---
name: "ai_id_photo_master"
description: "将用户的日常随手自拍一键转化为符合标准、专业且自然的精美证件照。自动输出图生图提示词并调用生图模型，解决背景杂乱、光影不佳、服装不正式等问题，适用于简历、签证、工作牌等核心场景。"
---

# AI极简证件照大师

这个技能用于将用户的日常随手自拍一键转化为符合标准、专业且自然的精美证件照。自动输出图生图提示词并调用生图模型，解决背景杂乱、光影不佳、服装不正式等问题，适用于简历、签证、工作牌等核心场景。

## 功能特点

- 🎯 智能识别面部特征，保留个人辨识度
- 🎨 自动优化光影，消除不良光线影响
- 👔 智能穿搭替换，将休闲服饰替换为正式服装
- 🖼️ 背景净化重构，替换为标准证件照底色
- 📏 符合证件照标准尺寸和比例要求
- 🎓 适用于多种场景：求职简历、护照签证、驾照、员工牌等

## 使用方法

### 输入参数

- `background_color`: 背景颜色（必填，可选：white/blue/red/grey）
- `clothing_style`: 服装风格（必填，如：black_suit_white_shirt/white_shirt/light_blue_business）
- `usage_scenario`: 使用场景（必填，如：resume/passport/driver_license/employee_card）
- `subject_features`: 人物特征描述（英文，必填，如：A 25-year-old Asian female with long hair）
- `hair_style`: 发型描述（英文，必填，如：neat tied-up hair/short tidy hair）

### 输出结果

- `prompt`: 生成证件照的完整提示词
- `image_size`: 推荐的图片尺寸

## 设计规范

- **视觉风格**: 超写实摄影风格，专业影棚肖像照
- **布局**: 3:4比例，胸部以上半身特写，头部居中
- **背景**: 纯色背景（白/蓝/红/灰）
- **光影**: 专业影棚平光/蝴蝶光，面部光线均匀柔和
- **服装**: 正式商务服装，合身无褶皱
- **表情**: 自然、礼貌、自信，直视镜头

## 文件结构

- `skill.json`: 技能描述文件，包含核心模板和配置
- `SKILL.md`: 使用说明文档

## 许可证

MIT License