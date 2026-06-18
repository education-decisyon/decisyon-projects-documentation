---
icon: microphone
---

# 5. Meeting Sense

### 概述

**Meeting Sense** 是集成在 DISS 中的会议录制和转录功能。它将 SIM 会议的口头对话转化为结构化数字数据：文字记录、执行摘要、提出的问题以及准备添加到 SIM 行动计划中的 AI 建议行动列表。会话自动与启动它的 SIM Board 的元数据（工厂、SIM 级别、生产区域）进行上下文关联，以便每个结果都已链接到正确的操作范围。

<figure><img src=".gitbook/assets/recording-widget-in-active-state-during-the-meeting-with-session-duration-and-audio-status-indicator.png" alt=""><figcaption></figcaption></figure>

## 使用时机

* 在 SIM 2 日常会议期间，团队讨论问题、根本原因和纠正措施，希望每个结果在 DISS 中都可追溯，无需手动记录笔记。
* 当 SIM 负责人希望对话被完整录制，以确保讨论和行动计划之间不会遗漏任何内容。
* 当团队在会议结束时需要出勤记录和一次性准备分配的结构化行动集。

## 先决条件

* 打开会议的 SIM Board 必须是 **SIM 2** Board（Meeting Sense 在此 SIM 级别启用）。
* 用于启动会议的设备上必须有可用的麦克风。
* 出勤角色必须为 SIM 2 Board 配置——可在**工厂配置 → 出勤 → SIM 2 出勤配置**中访问。
* 用户必须有权限在相关 SIM Board 上启动会议。

## 使用方法

{% stepper %}
{% step %}
### 打开 SIM Board 并开始会议

* 导航至举行会议的 SIM Board（**Digitized Idea & SIM System → SIM Boards → SIM 2**）。工厂、生产区域和日期自动填充。
* 点击右上角的**开始会议**打开会议初始化对话框。

<figure><img src=".gitbook/assets/sim-board-with-start-meeting-button-highlighted-in-the-top-right-corner.png" alt="突出显示开始会议按钮的 SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 初始化出勤和 SIM 负责人

在初始化对话框中：

* 定义每位参与者的状态（**准时、迟到、缺席**或**不需要**）；
* 分配 **SIM 负责人**（默认为当前用户，可通过下拉菜单更改）；
* 点击**开始会议**继续。

<figure><img src=".gitbook/assets/meeting-initialisation-dialog-attendance-statuses-and-sim-leader-selector.png" alt="包含出勤状态和 SIM 负责人选择器的会议初始化对话框"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择音频输入并开始录制

* 从可用音频输入列表中选择所需的麦克风并确认。如果未检测到麦克风，将显示错误消息，录制无法开始。

<figure><img src=".gitbook/assets/audio-input-device-selection-popup-with-a-microphone-confirmed.png" alt="已确认麦克风的音频输入设备选择弹出窗口"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 进行会议

在整个会议过程中清晰地发言，并表达之后创建行动所需的要素：

* 问题的**简短描述**；
* 相关**类别**（安全、质量、交付、维护、生产、工程）；
* **被分配人姓名**；
* 完成**目标**日期。

<figure><img src=".gitbook/assets/recording-widget-in-active-state-during-the-meeting-with-session-duration-and-audio-status-indicator.png" alt="录制小部件处于活动状态，显示会话持续时间和音频状态指示器"><figcaption></figcaption></figure>

{% hint style="info" %}
预定义的超时可防止会议因错误而保持打开状态：超时前两分钟会出现通知对话框，提供延长或手动停止会话的机会。
{% endhint %}
{% endstep %}

{% step %}
### 停止录制

* 会议结束后点击**停止**控件。系统开始在后台处理音频。生成转录时，可以切换到其他活动——团队不需要在会议页面等待。
* 转录和 AI 分析准备好后会出现通知。

<figure><img src=".gitbook/assets/recording-stopped-processing-indicator-and-confirmation-that-transcription-is-queued.png" alt="录制已停止，处理指示器和转录已排队的确认"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 从档案中打开会议

* 导航至**会议 → 会议概览**。
* 会议概览页面按时间顺序列出每个录制的会话，显示标题、SIM 级别、日期和 SIM 负责人。

<figure><img src=".gitbook/assets/overview-meeting-archive-with-the-list-of-recorded-sessions.png" alt="显示录制会话列表的会议概览档案"><figcaption></figcaption></figure>

* 点击会议以打开其详细视图。

<figure><img src=".gitbook/assets/meeting-detail-view_summary-identified-issues-ai-suggested-actions.png" alt="会议详细视图：摘要、已识别问题、AI 建议行动、持续时间、出勤记录"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 查看和编辑转录文本

* 点击**显示转录**显示字面文本，该文本保持完全可编辑。
* 纠正语音转文本引擎的任何误解，或添加未捕获的细节。
* 更新转录后，点击**生成会议记录**刷新 AI 摘要。

<figure><img src=".gitbook/assets/transcript-pane-with-show-transcription-opened-and-generate-meeting-notes-button.png" alt="显示转录已打开且带生成会议记录按钮的转录面板"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 结果解读

| 块               | 描述                                                                                              |
| ---------------- | ------------------------------------------------------------------------------------------------- |
| 摘要             | AI 生成的会议讨论叙述性概述，涵盖讨论的主要主题。                                                |
| 已识别问题       | 在会议期间识别的问题和异常情况的结构化列表，由 AI 从录制的对话中提取。                           |
| AI 建议行动      | 从对话中自动生成的行动建议，每个都有推断的描述、类别、负责人和截止日期。                          |
| 出勤记录         | 在会议开始时汇编的出勤列表，每位参与者都设置了状态。                                              |
| 持续时间         | 录制会议会话的总持续时间。                                                                        |

## 提示与已知限制

{% hint style="info" %}
* 清晰地发言并避免声音重叠：AI 提取质量随音频清晰度的提高而提升。
* 准确提及姓名和日期——"张三，周五前"比"他，本周末"等隐含引用产生更可靠的 AI 建议。
* 类别和负责人是行动创建的必填项：没有这些值的建议行动必须在验证表中完成后才能保存。
* Meeting Sense 是一个录制助手：SIM 负责人始终保持控制——行动只有在明确验证后才成为 SIM 计划的一部分，转录可以在创建任何行动之前编辑并重新汇总。
{% endhint %}
