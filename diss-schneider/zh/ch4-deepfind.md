---
icon: magnifying-glass
---

# 4. Deep Find

### 概述

**Deep Find** 是集成在 DISS 中的 AI 聊天机器人，允许用户以自然语言查询已配置的知识源——工厂手册、程序、常见问题、政策、报告的存储库。Deep Find 分析已上传的文档并根据其内容综合回答。可以将多个文档附加到同一对话中，为 AI 提供更丰富的上下文。

<figure><img src=".gitbook/assets/DeepFind-Cover Welcome page.png" alt=""><figcaption></figcaption></figure>

## 使用时机

* 查找特定设备干预的程序。
* 验证质量或安全政策的先决条件或步骤。
* 识别机器上出现的错误代码并找到推荐的纠正措施。
* 在 Kata 调查期间在大型技术手册中找到正确的段落。

## 先决条件

* 必须在 DISS 中为您的工厂配置知识源。
* 相关文档（手册、程序、常见问题、错误代码参考）必须已上传到知识源。
* 必须在该知识源中明确启用 Deep Find。

{% hint style="info" %}
如果 Deep Find 在您的 DISS 工具栏中不可见，请联系您的 DISS 管理员，验证是否已为您的工厂配置了启用 Deep Find 的知识源。
{% endhint %}

## 使用方法

{% stepper %}
{% step %}
### 配置知识源

* 此步骤由具有**知识源管理员**范围的用户执行，必须在最终用户查询 Deep Find 之前完成。

<figure><img src=".gitbook/assets/diss_user-profile-details-with-knowledge-source-administrator-scope-highlighted.png" alt="突出显示知识源管理员范围的用户配置文件详情"><figcaption></figcaption></figure>

* 点击右上角的用户头像，从下拉菜单中选择**知识源**。在左侧面板中，点击 **+** 打开创建对话框。输入描述性名称并点击**创建**。

<figure><img src=".gitbook/assets/Knowledge Sources — profile dropdown showing the Knowledge Sources option.png" alt=""><figcaption></figcaption></figure>

* 选中知识源后，转到**文档**选项卡，点击**导入文件**上传相关文档（PDF 或兼容格式）。每个额外文件重复此操作。

<figure><img src=".gitbook/assets/knowledge-sources_documents-tab-with-import-file-button-and-uploaded-document-list.png" alt="带导入文件按钮和已上传文档列表的文档选项卡"><figcaption></figcaption></figure>

* 在**权限**选项卡中，分配允许查询此知识源的组织和用户组。

<figure><img src=".gitbook/assets/knowledge-sources_permissions-tab-with-organisation-and-group-configured.png" alt="已配置组织和组的权限选项卡"><figcaption></figcaption></figure>

* 在 **AI 代理**选项卡中，启用 **Deep Find AI Assistant** 切换开关，将此知识源连接到 Deep Find。

<figure><img src=".gitbook/assets/knowledge-sources_ai-agents-tab-with-deepfind-ai-assistant-enabled.png" alt="已启用 DeepFind AI Assistant 的 AI 代理选项卡"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 打开 Deep Find

* 在 DISS 工具栏中找到 **Deep Find Assistant** 图标，点击打开聊天界面。

<figure><img src=".gitbook/assets/deepfind_assistant-icon-in-the-toolbar.png" alt="工具栏中的 DeepFind Assistant 图标"><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/deepfind_chat-interface-opened-empty-state.png" alt="打开的 DeepFind 聊天界面（空状态）"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 提问

* 以自然语言输入问题——完整的句子比关键词搜索效果更好。对于故障排除，包括错误代码和症状的简短描述。

<figure><img src=".gitbook/assets/deepfind_typing-a-natural-language-question-with-error-code-example.png" alt="输入带错误代码示例的自然语言问题"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 阅读回答并跟进

* 阅读综合回答。Deep Find 在每个回答末尾引用来源文档和章节，以便验证信息来源。如有必要，提出后续问题以细化或扩展回答。

<figure><img src=".gitbook/assets/deepfind_synthesised-answer-and-follow-up-turn.png" alt="综合回答和后续对话轮次"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## 结果解读

Deep Find 根据在已配置知识源和附加到对话的文档中找到的最相关段落综合回答。回答遵循底层文档的访问策略：用户只能看到其有权访问的文档中的信息。

当 Deep Find 无法根据可用材料回答时，返回：_"抱歉，我无法帮助解决这个问题，因为它超出了我的知识范围。"_ 这意味着未找到相关文档，而不是该主题不存在。

## 提示与已知限制

{% hint style="info" %}
* 一次提一个问题——复合问题往往会得到部分回答。
* 如果回答不完整，用不同的关键词重新表述，或更具体地说明设备、流程或错误代码。
* 如果问题在范围内但未找到答案，请咨询 DISS 管理员，验证相关文档是否已上传且该知识源中已启用 Deep Find。
* Deep Find 不会编造内容：它只引用已配置知识源或附加文档中存在的材料。
{% endhint %}
