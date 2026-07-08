# Tasks

- [x] Task 1: 创建 `index.html` 基础骨架与样式
  - [x] SubTask 1.1: 编写 HTML 结构（上传区、筛选区、表格区、文案区、复制按钮）
  - [x] SubTask 1.2: 编写简洁的 CSS 样式（响应式、清晰分隔、按钮态）
  - [x] SubTask 1.3: 通过 CDN 引入 SheetJS（xlsx.full.min.js）

- [x] Task 2: 实现 Excel 解析与数据展示
  - [x] SubTask 2.1: 监听文件选择/拖拽事件，调用 `XLSX.read` 解析
  - [x] SubTask 2.2: 校验表头，缺失必要列时给出提示
  - [x] SubTask 2.3: 将行数据渲染为 HTML 表格并显示行数

- [x] Task 3: 实现直属领导筛选
  - [x] SubTask 3.1: 从数据中提取去重的「直属领导」列表
  - [x] SubTask 3.2: 提供下拉多选控件（默认全选），联动表格与文案区

- [x] Task 4: 实现当月报工情况文案生成
  - [x] SubTask 4.1: 区分「0 次」与「>0 次」人员
  - [x] SubTask 4.2: 按 `7月份报工情况: ...。` 模板拼接，自动从「查询日期」取月份

- [x] Task 5: 实现今日未报工提醒文案生成
  - [x] SubTask 5.1: 过滤 `当天报工(件数) = 0` 的人员
  - [x] SubTask 5.2: 按 `7月8日报工情况: ...。` 模板拼接，日期从「查询日期」取

- [x] Task 6: 实现一键复制
  - [x] SubTask 6.1: 调用 `navigator.clipboard.writeText`，失败时回退 `execCommand('copy')`
  - [x] SubTask 6.2: 文案为空时禁用复制按钮

# Task Dependencies
- Task 2 依赖 Task 1
- Task 3 依赖 Task 2
- Task 4、Task 5 依赖 Task 3
- Task 6 依赖 Task 4、Task 5
