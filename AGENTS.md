# AGENTS.md

## 项目概览
"今天吃什么"随机吃饭选择器，纯静态 HTML 页面，支持本地双击打开。

## 技术栈
- 原生 HTML + CSS + JavaScript（无构建步骤）
- 静态文件服务（python http.server）

## 目录结构
```
.
├── index.html          # 主页面（所有样式和逻辑内联）
├── images/             # 店铺图片统一存放目录
│   ├── crab_baba.jpg   # 蟹爸爸
│   ├── xinfaxian.jpg   # 新发现
│   └── ...             # 其他店铺图片
├── .coze               # 沙箱配置
└── DESIGN.md           # 设计规范
```

## 维护指南
### 修改店铺数据
编辑 `index.html` 中的 `RESTAURANTS` 数组，每个对象包含：
- `name`: 店铺名称
- `image`: 图片文件名（对应 images/ 目录下的文件）

### 新增店铺
1. 将图片放入 `images/` 文件夹
2. 在 `RESTAURANTS` 数组中添加新对象

### 修改图片
替换 `images/` 目录下对应文件，保持文件名不变即可。
