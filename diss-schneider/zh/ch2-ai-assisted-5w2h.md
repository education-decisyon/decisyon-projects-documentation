---
icon: star-half-stroke
---

# 2. AI辅助5W2H

### 概述

**AI-Assisted 5W2H** 是一个质量评估小部件，用于分析 Kata 问题陈述的完整性和清晰度。它根据 5W2H 框架——**谁、什么、为什么、何时、何地、如何、多少**——对用户在当前状态和目标状态字段中输入的文本进行评分，并返回总体质量评分和每个维度的反馈。目标是在团队和工厂之间标准化质量检查，消除不一致和主观的审查。

<figure><img src=".gitbook/assets/5W2H Cover - Welcome page.png" alt=""><figcaption></figcaption></figure>

## 使用时机

* 在起草新 Kata 的**当前状态**或**目标状态**时，确保问题陈述足够精确且可操作。
* 在辅导会议期间，直接从用户文本中提取证据支持对话。
* 随着时间推移，通过稳定的数字评分追踪团队间问题陈述质量的演变。

## 先决条件

* **5W2H** 小部件必须在需要运行的 Kata 字段中启用（通常是当前状态和目标状态）。
* 用户必须具有编辑相关 Kata 的权限。

## 使用方法

{% stepper %}
{% step %}
### 导航至 Kata QRCI

* 导航至 **Digitized Idea & SIM System → Kata QRCI**。仪表板显示所有现有 Kata，可按日期范围、状态和 KPI 筛选。点击右上角的**添加**打开新建 Kata 表单。

<figure><img src=".gitbook/assets/kata-qrci_dashboard-with-kata-list-and-add-button-highlighted.png" alt="Kata QRCI 仪表板，添加按钮已高亮显示"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写 Kata 标题

在添加表单中，配置上下文字段：

* **生产区域**和**生产线**（来自工厂层级结构）；
* **标题**（简洁的问题陈述）；
* **负责人**和**教练**（均为必填项）；
* **来源**（问题来源类别，如停机时间、效率、维护问题）和 **KPI**（如 OEE）；
* **创建日期**自动填充为当前日期。

<figure><img src=".gitbook/assets/Kata QRCI — Add form with header fields filled in.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写当前状态 (5W2H) 和目标

* 在**当前状态**和**目标 (5W2H)** 字段中，按照 5W2H 框架清晰且可测量地描述当前情况和期望的最终状态：**谁、什么、为什么、何时、何地、如何、多少。**

<figure><img src=".gitbook/assets/5w2h_kata-form-with-current-state-target-state-fields.png" alt="包含当前状态和目标状态字段的 Kata 表单"><figcaption></figcaption></figure>

* 输入时，小部件的内联指示器显示当前质量评分和字符数。

<figure><img src=".gitbook/assets/5w2h_inline-quality-badge-updating-live-as-the-user-types.png" alt="用户输入时实时更新的内联质量徽章" width="473"><figcaption></figcaption></figure>

* 点击内联指示器以打开详细弹出窗口。

<figure><img src=".gitbook/assets/5w2h_clicking-the-badge-opens-the-detailed-popup.png" alt="点击徽章打开详细弹出窗口" width="563"><figcaption></figcaption></figure>

* 查看圆形评分、定性标签和 AI 建议的**重点关注：**区域。

<figure><img src=".gitbook/assets/5w2h_detailed-popup-with-circular-score-and-focus-on-area.png" alt="包含圆形评分和重点关注区域的详细弹出窗口" width="563"><figcaption></figcaption></figure>

* 在文本中添加缺失的信息；保存字段时评分会更新。

<figure><img src=".gitbook/assets/5w2h_score-recalculated-after-adding-missing-information.png" alt="添加缺失信息后重新计算的评分"><figcaption></figcaption></figure>

* 点击**保存**创建 Kata。

<figure><img src=".gitbook/assets/kata-qrci_add-form-with-current-status-5w2h-and-target-fields-filled-in.png" alt="已填写当前状态和目标 (5W2H) 字段的表单"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 打开 Kata 以激活 5W2H 小部件

* 新 Kata 出现在 **Kata QRCI** 列表中。打开它：**AI-Assisted 5W2H** 小部件现在在当前状态和目标状态字段中处于活动状态，并开始评估输入的文本。

<figure><img src=".gitbook/assets/kata-qrci_newly-created-kata-visible-in-the-list-ready-to-open.png" alt="新 Kata 在列表中可见，准备打开"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 结果解读

### 7 个维度

每个问题陈述都按照相同的固定维度集进行评估，顺序如下：**谁、什么、为什么、何时、何地、如何、多少**。

### 每维度评分

每个维度根据文本中对其处理的完整性和具体程度获得交通灯颜色和数字评分。

### 总体质量评分

总分是 7 个维度评分之和（最高 14 分），表示为 14 的百分比，得到 0 到 100 的质量评分。

### 摘要表

对于每个维度，小部件显示四列：

| 列     | 描述                                                        |
| ------ | ----------------------------------------------------------- |
| 问题   | 正在评估的 5W2H 维度                                        |
| 评估   | 维度评分和交通灯颜色                                        |
| 摘录   | AI 用于评估该维度的文本部分                                 |
| 建议   | 需要添加或澄清的内容（当维度缺失或模糊时显示）              |

## 提示与已知限制

{% hint style="info" %}
* 用户保持完全控制：AI 建议仅供参考——最终文本始终由用户编写和保存
* 评分基于当前字段的文本计算——独立填写当前状态和目标状态以获得可靠的按字段反馈
* 小部件奖励具体性：日期、名称、生产线、KPI 和可测量数量能快速提升评分
* 翻译是一种展示功能：评分基于原始文本计算
* 两个具有相同总评分的问题陈述可能具有非常不同的维度分布——使用摘要表而非仅使用总百分比来决定改进方向
* AI-Assisted 5W2H 是一个指导工具：持续低分是团队需要问题表述方面辅导的信号
{% endhint %}
