# 儿童日常照片转自然拼读贴纸技能

一个用于将儿童日常照片转化为教育性自然拼读贴纸的AI技能。该设计不仅包含了专业的图生图提示词生成逻辑，还融入了教育价值（提取拼读规律）和互动价值（亲子互动玩法），成品可直接用于淘宝定制。

## 🌟 功能特点

- 📸 **照片转贴纸**：将孩子的日常照片一键转化为可爱的自然拼读贴纸
- 🔤 **教育价值**：自动提取单词拼读规律，帮助孩子学习自然拼读
- 🎨 **专业设计**：采用可爱的2D儿童绘本插画风格，色彩明亮活泼
- 👨‍👩‍👧 **亲子互动**：提供多种亲子互动玩法，让学习更有趣
- 🛒 **定制输出**：生成的设计可直接用于淘宝等平台定制实体贴纸
- 📐 **标准比例**：3:4比例设计，适合各种展示和打印需求

## 🖼️ 效果展示

### 示例：从日常照片到自然拼读贴纸

**原图（孩子跑步的日常照片）**
![原图](https://trae-api-cn.mchost.guru/api/ide/v1/text_to_image?prompt=A%20little%20girl%20running%20outdoors%2C%20light%20blue%20clothes%2C%20pigtails%2C%20happy%20expression%2C%20real%20photograph&image_size=portrait_4_3)

**成品（RUN自然拼读贴纸）**
![成品](https://trae-api-cn.mchost.guru/api/ide/v1/text_to_image?prompt=Cute%20educational%20phonics%20sticker%20design%2C%20letter%20R%20at%20top%2C%20little%20girl%20running%20in%20center%2C%20word%20RUN%20at%20bottom%2C%20colorful%20cartoon%20style%2C%20sticker%20border&image_size=portrait_4_3)

## 🚀 使用方法

### 输入参数

- `core_word`: 核心词汇（必填），如 "run", "apple", "ball"
- `target_letter`: 首字母/目标音素（必填），如 "R", "A", "B"
- `subject_description`: 人物特征和动作描述（英文，必填）
- `main_subject`: 主体描述（英文，必填）

### 输出结果

- `prompt`: 生成贴纸设计的完整提示词
- `image_size`: 推荐的图片尺寸（portrait_4_3）

### 使用示例

```json
{
  "core_word": "run",
  "target_letter": "R",
  "subject_description": "A cute little girl with pigtails, wearing blue overalls and striped shirt, running happily",
  "main_subject": "A girl running"
}
```

## 📚 教育价值

### 拼读规律提取

- **首字母发音**：突出目标字母的发音特点
- **音节分解**：帮助孩子理解单词的音节结构
- **视觉联想**：通过生动的图像建立单词与含义的联系

### 亲子互动玩法

1. **贴纸拼图**：将多个贴纸组合成故事场景
2. **单词接龙**：用贴纸玩单词接龙游戏
3. **情景表演**：根据贴纸内容进行角色扮演
4. **拼写比赛**：使用贴纸进行拼写练习

## 🎨 设计规范

- **视觉风格**: 可爱的2D儿童绘本插画风格
- **布局**: 3:4比例，顶部目标字母，中间插图，底部核心词汇
- **颜色**: 柔和的pastel背景，明亮的糖果色主体
- **字体**: 粗体、圆润、气泡状的儿童友好字体
- **边框**: 厚白色描边，营造贴纸效果
- **细节**: 加入小星星、气泡等装饰元素增加趣味性

## 🔧 技术实现

### 图生图提示词生成逻辑

该技能通过以下步骤生成高质量的图生图提示词：

1. **人物特征提取**：从输入描述中提取孩子的外貌特征
2. **动作场景构建**：根据词汇含义构建相应的动作场景
3. **教育元素融合**：融入自然拼读的教育元素
4. **风格统一化**：应用统一的视觉风格和设计规范

### 核心提示词结构

```
Create a cute educational phonics sticker design about the word "{{core_word}}".

=== CRITICAL STYLE REQUIREMENTS ===
【OVERALL CONCEPT】
- Cute 2D children's picture book illustration style
- High educational value with clear phonics focus
- Die-cut sticker style with thick white border

【LAYOUT】
- Aspect ratio: 3:4
- Top: Giant cute letter "{{target_letter}}"
- Middle: {{main_subject}} illustration
- Bottom: Bold word "{{core_word}}"

【VISUAL ELEMENTS】
- Subject details: {{subject_description}}
- Background: Soft pastel color
- Decorations: Little stars, bubbles, etc.
```

## 🛒 定制建议

### 淘宝定制流程

1. 使用本技能生成贴纸设计提示词
2. 将生成的图片保存到本地
3. 在淘宝搜索"贴纸定制"或"不干胶印刷"
4. 选择合适的商家，上传设计文件
5. 选择材质（推荐防水不干胶）
6. 确认数量和尺寸后下单

### 推荐材质

- **防水不干胶**：适合贴在水杯、笔记本等物品上
- **透明PVC**：适合贴在玻璃、手机壳等光滑表面
- **磁性贴纸**：适合贴在冰箱、白板等磁性表面

## 📦 安装方法

1. 克隆仓库：
```bash
git clone https://github.com/hjsjtu826/phonics-sticker-design.git
cd phonics-sticker-design
```

2. 将技能文件复制到您的AI助手技能目录

## 🤝 贡献

欢迎提交Issue和Pull Request！如果您有更好的设计建议或功能改进，欢迎参与贡献。

## 📄 许可证

MIT License

## 📧 联系方式

- 作者: 硅蜜
- 邮箱: jeanhu721@gmail.com