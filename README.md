# 蓝色诺瓦学院 · 热力学课程 · 学生测试包

> v0.1 · 2026-06-10 建立 · 学生测试用 · 后续生成的新 HTML 直接放本目录

## 目录结构

```
蓝色诺瓦学院_热力学_学生测试包/
├── index.html                                                   # 主入口
├── README.md                                                    # 本文件
├── images/                                                      # 图片资源
│   └── molecular-kinetic-theory-fr-curve.jpg
│
├── basic-task-cards.html                                        # 热力学第一定律(基础)
├── advanced-task-cards.html                                     # 热力学第一定律 · 微观推导(进阶)
├── molecular-kinetic-theory-task-cards.html                     # 分子动理论(基础)
├── gas-liquid-solid-task-cards.html                             # 气体液体固体(基础)
├── second-law-basic-task-cards.html                             # 第二定律 · 基础(基础)
├── hess-law-task-cards.html                                     # 盖斯定律(基础)
├── carnot-cycle-task-cards.html                                 # 卡诺循环(进阶)
├── state-functions-task-cards.html                              # 状态函数(进阶)
├── entropy-meaning-task-cards.html                              # 熵的物理意义(进阶)
├── enthalpy-meaning-task-cards.html                             # 焓与焓变的意义(进阶)
├── gibbs-free-energy-basic-task-cards.html                      # 吉布斯自由能 · 基础(基础)
├── gibbs-free-energy-advanced-task-cards.html                   # 吉布斯自由能 · 进阶(进阶)
├── combustion-neutralization-heat-task-cards.html               # 燃烧热与中和热(基础)
├── bond-energy-reaction-enthalpy-task-cards.html                # 键能与反应焓变(基础)
│
├── hess-law-mock-check.html                                     # 盖斯定律 · 基础检测
├── molecular-kinetic-theory-mock-check.html                     # 分子动理论 · 基础检测
└── molecular-kinetic-theory-fluency-test.html                   # 分子动理论 · 熟练度检测
```

**扁平结构**: 所有 HTML 直接放在根目录, 互相用相对路径引用(如 `href="basic-task-cards.html"`)。图片放 `images/` 子目录。

## 板块清单(15 个)

### 基础链(高考必考, 必学 · 8 个)

按学习顺序:

1. **分子动理论** — `molecular-kinetic-theory-task-cards.html`(✅ 已配 mock-check + fluency-test)
2. **理想气体的状态方程**(原"气体液体固体") — `gas-liquid-solid-task-cards.html`(✅ 已配 mock-check + fluency-test)
3. **热力学第一定律** — `basic-task-cards.html`(✅ 已配 mock-check + fluency-test)
4. **第二定律 · 基础** — `second-law-basic-task-cards.html`(✅ 已配 mock-check + fluency-test)
5. **盖斯定律** — `hess-law-task-cards.html`(✅ 已配 mock-check + fluency-test)
6. **燃烧热与中和热** — `combustion-neutralization-heat-task-cards.html`
7. **键能与反应焓变** — `bond-energy-reaction-enthalpy-task-cards.html`
8. **吉布斯自由能 · 基础** — `gibbs-free-energy-basic-task-cards.html`

### 进阶链(深化, 可选 · 6 个)

1. **热力学第一定律 · 微观推导** — `advanced-task-cards.html`
2. **卡诺循环** — `carnot-cycle-task-cards.html`
3. **状态函数与非状态函数** — `state-functions-task-cards.html`
4. **熵的物理意义** — `entropy-meaning-task-cards.html`
5. **焓与焓变的意义** — `enthalpy-meaning-task-cards.html`
6. **吉布斯自由能 · 进阶** — `gibbs-free-energy-advanced-task-cards.html`

### 配套检测(12 个)

- **分子动理论 mock-check** — `molecular-kinetic-theory-mock-check.html`(基础检测)
- **分子动理论 fluency-test** — `molecular-kinetic-theory-fluency-test.html`(熟练度检测 · 题型同高考)
- **理想气体的状态方程 mock-check** — `gas-liquid-solid-mock-check.html`(基础检测)
- **理想气体的状态方程 fluency-test** — `gas-liquid-solid-fluency-test.html`(熟练度检测 · 题型同高考)
- **热力学第一定律 mock-check** — `basic-mock-check.html`(基础检测)
- **热力学第一定律 fluency-test** — `basic-fluency-test.html`(熟练度检测 · 题型同高考)
- **第二定律 · 基础 mock-check** — `second-law-basic-mock-check.html`(基础检测)
- **第二定律 · 基础 fluency-test** — `second-law-basic-fluency-test.html`(熟练度检测 · 题型同高考)
- **盖斯定律 mock-check** — `hess-law-mock-check.html`(基础检测)
- **盖斯定律 fluency-test** — `hess-law-fluency-test.html`(熟练度检测 · 题型同高考 · v0.1.4 首应用)
- **燃烧热与中和热 mock-check** — `combustion-neutralization-heat-mock-check.html`(基础检测)
- **燃烧热与中和热 fluency-test** — `combustion-neutralization-heat-fluency-test.html`(熟练度检测 · 题型同高考)

## 学生使用指引

1. 从 `index.html` 主入口进入, 按学习路径建议浏览
2. 每个板块是一份"学习任务卡", 含 3-5 张 Card、若干思考点、SVG 示意图、检查点
3. 学完任意基础板块后, 可以根据兴趣进入进阶链对应主题深化
4. 配套检测(目前只有盖斯定律)用于评估"是否真的掌握了基础结论"
5. 进度自动保存在浏览器 localStorage(不会丢失, 只在当前浏览器有效)

## 开发者: 后续添加新 HTML 的约定

1. **命名规范**: `{module-slug}-{type}.html`, type ∈ {task-cards / mock-check / fluency-test / oral-exam}
2. **直接放本目录根**: 不创建子目录(保持扁平结构, 相对路径简单)
3. **图片**: 放 `images/` 子目录, HTML 中用 `src="images/{filename}"`
4. **相对路径引用**: HTML 间用 `href="other-task-cards.html"`, 不用 `./` 或 `../`
5. **路径检查**: 添加后跑下面的检查脚本

```bash
# 路径完整性检查
cd ~/Desktop/蓝色诺瓦学院_热力学_学生测试包
python3 -c "
import re
from pathlib import Path
DST = Path('.')
htmls = list(DST.glob('*.html'))
existing = {f.name for f in htmls}
broken = []
for f in htmls:
    refs = re.findall(r'href=\"([^\"]+\.html)\"', f.read_text())
    for ref in refs:
        if ref not in existing:
            broken.append((f.name, ref))
print('❌ 断链:', broken) if broken else print('✅ OK')
"
```

6. **更新 index.html**: 新加的 HTML 在 index.html 中加一个 `.module-card` 入口

## 路径完整性(2026-06-10 建立时验证)

- 15 个 HTML 互相引用: ✅ 无断链
- 1 张图片引用: ✅ 路径正确

## 与开发主目录的关系

**开发主目录**(Skill 输出位置): `~/Desktop/热力学第一定律_AI自主学习课程/index-v2-github-pages/`

**本目录**(学生测试包): 是开发主目录中"新规范"15 个 HTML 的精选拷贝, 不含 5/20 招生展示版的过时 HTML。

后续 Skill 生成 HTML 默认输出到开发主目录, 然后用 `cp` 或 `rsync` 同步到本目录。或者直接修改 Skill 默认输出路径到本目录 — 由教师决定。
