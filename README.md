# Family / AI · 2026 研究图谱 v5

面向 DRS 课程论文调研的交互式文献资料库：AI 支持家庭跨代际社交、儿童与青少年、设计原型、技术、研究方法及证据边界。包含研究方向地图、设计机会地图、Research Gap 与 Research Questions。

## 结构
- `index.html` — 可公开访问的网页首页。包含旧版核心功能和 84 篇基础论文的 JSON 文献矩阵。
- `assets/atlas-addon.css` — v5 研究地图的样式。
- `assets/atlas-addon.js` — 六大主题、机会地图、三个 RQ 及两篇 HCI 文献增补与交互。
- `.nojekyll` — 使 GitHub Pages 直接发布静态资源。

## 如何部署（首次）
1. 使用 GitHub **Lya-banana** 账号创建**公开**仓库 `drs-ai-family-atlas`，不需要预先创建 README（避免和本项目重复）。
2. 将本目录下 `index.html`、`assets/`、`.nojekyll`、`README.md` 全部上传到仓库的 `main` 分支，保持目录结构。
3. 打开 `Settings` → `Pages`，在 `Build and deployment` 下选择 `Deploy from a branch`，分支 `main`、目录 `/(root)`，保存。
4. Pages 成功部署后访问 `https://lya-banana.github.io/drs-ai-family-atlas/`。

## 后续怎么更新
- 更新地图规则、机会点、RQ：编辑 `assets/atlas-addon.js`。
- 更新视觉：编辑 `assets/atlas-addon.css`。
- 更新原有 84 篇底表：编辑 `index.html` 内的 `<script id="data" type="application/json">` 文献 JSON；也可以让自动化助手在 GitHub 仓库提交修改。
- 更新后 GitHub Pages 将根据已配置的发布源重新发布，无须另行使用升级器或 API。

## 研究可信度声明
- 共 86 篇：旧版 84 篇 + v5 新增 FamilyDittos、家庭生成式 AI 代理隐私研究 2 篇；动态加载时按 DOI 去重。
- DRS 主会、IASDR、Nordes、CHI / DIS / IDC / CSCW 等 HCI 分开统计。收录的 B/C 档包括非 AI、非家庭实证的邻近研究，不能算作 AI 跨代社交的直接验证。
- 主题聚类、争议与 Research Gap 属于文献二次分析及假设，不等于原作者的实证结论，也不构成系统性综述。详见页面研究说明与各论文的证据等级。
- 网站纯静态，文献不要求个人登录，无模型 API 费用；公开仓库中的内容和提交历史任何人都可以访问，请勿提交隐私数据或密钥。

本项目静态站点地址与旧的 `chatgpt.site` 属于两个不同托管系统，发布到 GitHub 不会自动改写旧网址。