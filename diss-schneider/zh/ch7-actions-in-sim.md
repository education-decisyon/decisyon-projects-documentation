---
icon: list-check
---

# 7. SIM中的行动

### 概述

DISS 中的**行动**功能是直接从 SIM Boards 记录、分配和跟踪纠正和改进活动的结构化方式。此处记录了两个互补的使用案例：**创建行动**——用完整的 SIM 上下文记录新行动——以及**编辑行动**——在团队通过每日 SIM 例程解决问题时保持现有行动的更新。

<figure><img src=".gitbook/assets/Action - Overview (1).png" alt=""><figcaption></figcaption></figure>

## 使用时机

* 在 SIM 会议期间发现生产线上的问题或机会时**创建行动**：安全/质量/交付/维护/生产/工程问题，有明确的负责人和截止日期。
* 在 SIM 会议之间**编辑行动**以保持行动的最新状态：状态进展、改进的描述、新附件、捕获的解决方案或添加到活动日志的备注。
* 使用 Actions in SIM 确保在 SIM Board 上识别的每个问题都成为可追溯和可分配的活动，而不是口头承诺。

## 先决条件

* 用户必须能访问启用了行动的 SIM Boards。
* 行动类别、生产区域和生产线必须在**工厂配置**中配置——它们填充创建行动表单中的类别、模块和生产线字段。
* 负责人或团队必须在 DISS 中存在才能分配给行动。

## 使用方法——创建行动

{% stepper %}
{% step %}
### 打开创建行动表单

* 从 SIM Board，打开**创建行动**表单。

<figure><img src=".gitbook/assets/create-action_entry-point-on-the-sim-board.png" alt="SIM Board 上的创建行动入口点"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 配置 SIM 上下文

配置 SIM 上下文：

* **类别**（安全、质量、交付、维护、生产、工程）；
* **模块**（预填充来源板的生产区域）；
* **生产线**。
* **来源 SIM 级别**和**目标 SIM 级别**从来源 SIM Board 自动选择；保存前请验证，因为保存后来源 SIM 级别变为不可变。

<figure><img src=".gitbook/assets/create-action_sim-context-bar-category.png" alt="带类别的创建行动 SIM 上下文栏"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写标题

* 填写标识问题的**标题**（最多 500 个字符）。

<figure><img src=".gitbook/assets/create-action_title-field.png" alt="创建行动标题字段"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 配置状态

* 将**状态**保留为"新建"，除非本地 SIM 流程需要不同的初始状态。

<figure><img src=".gitbook/assets/create-action_status-dropdown.png" alt="创建行动状态下拉菜单"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写描述

* 填写**描述**。使用粗体、斜体和列表以提高可读性。
* 可选择点击 **AI Enhance** 以提高清晰度；质量指示器在输入时提供实时反馈。

<figure><img src=".gitbook/assets/create-action_description-with-ai-enhance-and-quality-indicator.png" alt="带 AI Enhance 和质量指示器的描述"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 设置截止日期

* 选择**截止日期**——默认为今天 + 7 天。

<figure><img src=".gitbook/assets/create-action_due-date-picker.png" alt="创建行动截止日期选择器"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 设置优先级和严重性

* 设置**优先级**（轻微 / 次要 / 主要 / 严重 / 阻塞）
* 设置**严重性**（低 / 中 / 高 / 严重）

<figure><img src=".gitbook/assets/create-action_priority-and-severity-dropdowns.png" alt="优先级和严重性下拉菜单"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 分配发起人、团队和负责人

* 确认**发起人**（预填充为当前用户；仅在代表他人记录时更改）。
* 分配责任：**团队**和**负责人**中至少一个必须配置，以便行动在 SIM Board 上有明确的责任方。

<figure><img src=".gitbook/assets/create-action_team-and-owner-assignment.png" alt="团队和负责人分配"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 保存行动

* 点击**保存行动**。
* 绿色按钮仅在所有必填字段完成后激活。保存后，行动在 SIM Board 上可见。

<figure><img src=".gitbook/assets/create-action_save-action-button-active-and-action-visible-on-sim-board.png" alt="保存行动按钮激活且行动在 SIM Board 上可见"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 使用方法——编辑行动

编辑行动具有**自动保存**：每个字段在退出字段时单独确认。没有全局保存按钮——标题显示"所有更改已保存"作为确认。此行为允许在 SIM 会议期间快速进行更新，而不会中断其节奏。

{% stepper %}
{% step %}
### 从 SIM Board 打开行动

* 从 SIM Board，打开要更新的行动。

<figure><img src=".gitbook/assets/edit-action_opening-an-action-from-the-sim-board.png" alt="从 SIM Board 打开行动"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 更新输入面板字段

* 更新输入面板中的可编辑字段：**标题、状态、描述**（带 AI Enhance 和质量指示器）、**截止日期、优先级、严重性、发起人、团队、负责人、附件**。

<figure><img src=".gitbook/assets/edit-action_entry-panel-with-all-editable-fields.png" alt="带所有可编辑字段的输入面板"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 如有必要升级到更高 SIM 级别

* 如果行动需要升级，请更改上下文栏中的**目标 SIM 级别**（这是创建后上下文栏中唯一保持可编辑的字段）。

<figure><img src=".gitbook/assets/edit-action_target-tier-dropdown-in-the-context-bar.png" alt="上下文栏中的目标 SIM 级别下拉菜单"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 添加或修改解决方案和建议

* 在**解决方案和建议**面板中，输入或粘贴建议的解决方案，或点击 **AI Suggest** 自动生成按相关性排名的解决方案建议。

<figure><img src=".gitbook/assets/edit-action_solutions-proposals-with-ai-suggest.png" alt="带 AI Suggest 的解决方案和建议"><figcaption></figcaption></figure>

* 建议从上传到 **Deep Find 知识源**的文档中提取。

<figure><img src=".gitbook/assets/edit-action_solutions-proposals-from-deepfind-document.png" alt="从 DeepFind 知识源文档提取的解决方案和建议"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 向活动日志添加备注

* 在面板底部向**活动日志**添加备注；如有必要，通过回形针图标附加文件。活动日志是 SIM Board 上行动的完整历史记录。

<figure><img src=".gitbook/assets/edit-action_activity-log-with-note-input-and-paperclip.png" alt="带备注输入和回形针的活动日志"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 将行动设置为已完成

* 仅在行动真正结束时将**状态**设置为"已完成"："已完成"会锁定整个记录。

<figure><img src=".gitbook/assets/edit-action_status-set-to-done-locked-record.png" alt="状态设置为已完成——记录已锁定"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 结果解读

* 描述中的**质量指示器**——差 / 可接受 / 良好 / 优秀——表示文本是否包含足够的信息以便可操作
* **AI Enhance** 将文本改写以提高专业清晰度；始终在保存前检查结果。
* 解决方案中的 **AI Suggest** 按照与描述内容的相关性百分比对建议进行排名。
* 当状态更改、新团队/负责人分配、截止日期前 48 小时警告和逾期行动时，会发送电子邮件通知。

## 提示与已知限制

{% hint style="info" %}
* 不要在行动真正完成之前将状态设置为"已完成"：之后无法编辑。
* 如果团队和负责人都被移除，保存将失败——始终保持至少一个已分配。
* 自动保存在出错时会还原字段：如果出现保存错误消息，请检查网络连接。
* AI Enhance 和 AI Suggest 是辅助性的：负责人仍然负责最终文本和所选解决方案。
* SIM 级别之间的升级通过更改目标 SIM 级别而不是创建新行动来完成——这保留了原始问题活动日志的历史记录。
{% endhint %}
