---
icon: chart-line
---

# 6. 会议洞察

### 概述

会议洞察 是一个 AI 代理，处理 会议感知 已捕获的会议。会议感知 专注于单个录制，而 会议洞察 同时分析多个会议记录，以识别整个档案中的模式、重复问题和汇总行动。它将单个 SIM 会议记录流转化为工厂或区域级的运营智慧。

<figure><img src=".gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png" alt=""><figcaption></figcaption></figure>

## 使用时机

* 回答"哪些问题一直在重复出现？"——会议洞察 识别所选时期 SIM 会议中的重复主题。
* 从许多会议（如上个月所有 SIM 1 会议）生成合并的行动列表，无需逐一打开。
* 提取不同生产日期和生产区域的趋势和模式，支持管理评审和持续改进方向。
* 使用任何支持语言的自然语言问题调查会议档案中的主题。

## 先决条件

* DISS 环境中必须至少存在一个由 会议感知 产生的会议记录。
* 用户必须能访问会议概览档案。
* 用户必须对分析中包含的会议具有读取权限。

## 使用方法

{% stepper %}
{% step %}
### 导航至会议概览档案

* 在 DISS 中导航至**会议概览**档案。

<figure><img src=".gitbook/assets/meeting-insight_overview-meeting-archive-page.png" alt="会议概览档案页面"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 筛选会议档案

* 使用日期或组织级别筛选器隔离与分析范围相关的会议。

<figure><img src=".gitbook/assets/meeting-insight_date-and-level-filters-on-the-archive.png" alt="档案上的日期和级别筛选器"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择要分析的会议

* 使用每行左侧的复选框选择多个会议，以定义分析数据集。

<figure><img src=".gitbook/assets/meeting-insight_meetings-selected-via-checkboxes.png" alt="通过复选框选择的会议"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动 会议洞察

* 点击**汇总记录**对所选会议启动 Insight 代理。代理打开一个对话窗口，可以与所有选定转录的合并数据集进行交互。

<figure><img src=".gitbook/assets/meeting-insight_summarize-notes-button.png" alt="汇总记录按钮"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 管理活动选择

* 使用侧边面板查看或取消选择特定会议而不关闭对话，保持对分析范围的完全控制。

<figure><img src=".gitbook/assets/meeting-insight_managing-the-active-selection-from-the-dialog.png" alt="从对话框管理活动选择"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 提取行动列表

* 点击**提取行动列表**将所选会话的所有行动汇总到一个列表中。

<figure><img src=".gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png" alt="跨会议汇总的行动项目列表"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 提出自然语言问题

* 在输入字段中以自然语言提问，在转录中定位特定的操作细节——根本原因、重复障碍、负责人。

<figure><img src=".gitbook/assets/meeting-insight_natural-language-query-on-the-selected-meetings.png" alt="对所选会议的自然语言查询"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导出并收藏结果

* 将常用查询添加书签以便更快地重用，并将生成的摘要或行动列表复制到外部文档用于报告。

<figure><img src=".gitbook/assets/meeting-insight_bookmarking-a-query-and-exporting-the-results.png" alt="为查询添加书签并导出结果"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 结果解读

| 结果             | 描述                                                                                                                           |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| 行动列表         | 所选会议会话中识别的所有行动的合并去重列表，包含描述、推断的负责人和来源会议。                                                 |
| 自然语言回答     | 基于所选会议完整转录内容综合的 AI 回答，引用来源会议和会话。                                                                   |
| 收藏查询         | 从侧边面板保存并可重用的常用查询，加速每周趋势检查或管理评审等重复分析。                                                       |

{% hint style="info" %}
结果仅供参考。会议负责人仍然负责通过行动功能将重复模式转化为具体的应对措施。
{% endhint %}

## 提示与已知限制

{% hint style="info" %}
* 洞察质量随底层 会议感知 会议记录的质量而提升：鼓励在会议期间进行清晰录制并明确提及负责人和日期。
* 在启动代理前使用筛选器——分析有针对性的数据集（如一个 SIM 级别和一个月）比分析整个档案产生更精确的洞察。
* 在 SIM 会议本身期间的实时 AI 参与不是此版本的一部分：会议洞察 目前对已录制的会议记录进行操作。
* 洞察仅供参考：负责人负责通过行动或 Kata 将重复模式转化为具体的应对措施。
{% endhint %}
