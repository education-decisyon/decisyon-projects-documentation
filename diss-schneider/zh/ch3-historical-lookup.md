---
icon: clock-rotate-left
---

# 3. 历史查询

### 概述

**Historical Lookup** 是一个 AI 功能，基于当前正在处理的 Kata QRCI，搜索同一工厂的已关闭 Kata 并返回最相似的结果。对于每个历史 Kata，用户可以查看 AI 对匹配原因的解释，并有选择性地导入用于解决过去问题的行动，从而加快对重复性问题的响应速度。

<figure><img src=".gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png" alt=""><figcaption></figcaption></figure>

## 使用时机

* 当工厂中的问题看起来很熟悉，但团队不记得何时、何地以及如何解决过时。
* 在保存新 Kata 之前，检查是否已处理过相同问题，避免重复工作。
* 在根本原因分析过程中，了解同事如何在类似案例中表述当前状态和目标状态。

## 先决条件

* 当前 Kata 必须定义了工厂：只有在配置了工厂后，Historical Lookup 才会激活。
* 搜索范围内必须至少存在一个状态为**已关闭**的 Kata，AI 才能找到匹配项。
* 用户必须对搜索范围内的历史 Kata 具有读取权限。

## 使用方法

{% stepper %}
{% step %}
### 打开 Kata 仪表板

* 在 DISS 中打开 **Kata 仪表板**。

<figure><img src=".gitbook/assets/historical-lookup_kata-dashboard-with-the-ai-tools-column-visible.png" alt="显示 AI 工具列的 Kata 仪表板"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动 Historical Lookup

* 在 **Kata** 列中，点击正在处理的已打开 Kata 旁边的 **Kata 相似度图标**。

<figure><img src=".gitbook/assets/historical-lookup_icon-highlighted-on-a-kata-row.png" alt="Kata 行上高亮显示的相似度图标"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 等待 AI 搜索完成

* **AI Historical Lookup** 模态框打开，搜索自动开始——不需要额外输入。等待加载消息（"正在加载相似 Kata…"）完成。

<figure><img src=".gitbook/assets/historical-lookup_modal-in-loading-state.png" alt="处于加载状态的 Historical Lookup 模态框"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 查看相似 Kata

* 查看返回的最多 5 个已关闭 Kata，按相似度评分降序排列。

<figure><img src=".gitbook/assets/historical-lookup_list-of-matches-with-similarity-scores.png" alt="带相似度评分的匹配列表"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 详细分析每个匹配项

* 对于每个匹配项，展开 **AI 分析**折叠面板，阅读"**匹配原因**"和"**需考虑的差异**"。

<figure><img src=".gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png" alt="展开的 AI 分析折叠面板"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 选择性行动复制

每个历史匹配项都有一个**可重用行动**选择器。展开后，该 Kata 的行动会加载，每个行动旁边会出现一个复选框。可以：

* 逐一选择单个行动；
* 在一个历史 Kata 中使用**全选 / 取消全选**；
* 在同一会话中合并来自多个 Kata 的选择——总计数始终可见。

选择至少一个行动后，**导入 N 个行动**按钮出现在底部。点击它将所选行动复制到当前 Kata。对于每个导入的行动：

* 从来源复制**标题**和**描述**；
* 状态重置为已打开；
* 默认截止日期为今天 + 7 天；新负责人设置新日期。

完成后，模态框自动关闭，出现确认消息，当前 Kata 的行动表更新以显示新记录。

{% stepper %}
{% step %}
### 加载历史行动

* 在某个匹配项中，点击**可重用行动**加载该 Kata 的历史行动。

<figure><img src=".gitbook/assets/selective-action-copy_view-actions-toggle-expanded-for-a-match.png" alt="为匹配项展开的可重用行动切换"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择要导入的行动

* 使用复选框选择单个行动，或使用**全选 / 取消全选**对整个 Kata 进行操作。

<figure><img src=".gitbook/assets/Selective Action Copy — checkboxes and Select All - Deselect All controls.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 合并来自多个 Kata 的选择

* 可选择对其他匹配项重复操作：选择在同一会话的多个 Kata 中保持不变。

<figure><img src=".gitbook/assets/selective-action-copy_multi-kata-selection-with-total-counter-visible.png" alt="显示总计数器的多 Kata 选择"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入所选行动

* 点击模态框底部的**导入 N 个行动**。

<figure><img src=".gitbook/assets/Selective Action Copy — Import N Actions button.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认并验证导入的行动

* 模态框关闭，出现确认，当前 Kata 的行动表更新为新记录（状态 = 已打开，截止日期 = 当前日期）。

<figure><img src=".gitbook/assets/selective-action-copy_current-kata-actions-table-refreshed-with-imported-records.png" alt="当前 Kata 行动表已更新为导入记录"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 结果解读

| 字段         | 描述                                                                                                                                              |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| 相似度评分   | 一个百分比 (0–100)，表示已关闭 Kata 与已打开 Kata 的匹配程度。高于 70 的分数表示强主题重叠；低于 40 是为了完整性而显示的弱匹配。                |
| 匹配原因     | AI 生成的对两个 Kata 之间共同元素的简洁解释。                                                                                                     |
| 需考虑的差异 | 历史案例与当前案例区别的简要摘要。                                                                                                                |
| 可重用行动   | 历史 Kata 的完整行动列表，准备好进行选择性导入。                                                                                                  |

## 提示与已知限制

{% hint style="info" %}
* 默认情况下，Historical Lookup 仅在当前工厂内搜索。启用多工厂范围后，来源工厂在每个结果上都有清晰标注。
* 只考虑**已关闭**的 Kata；进行中的 Kata 被排除在外。
* 相同或几乎相同的 Kata 不会被隐藏——它们以非常高的相似度出现，让您决定是否导入其行动。
* 导入的行动总是重新开始（状态 = 已打开，截止日期 = 默认今天 + 7 天）：新负责人承担截止日期所有权。
* 区域、生产线、来源和 KPI 筛选器不是严格筛选器——AI 将其用作语义上下文，这意味着来自不同生产线的相关匹配项仍可能被建议。
{% endhint %}
