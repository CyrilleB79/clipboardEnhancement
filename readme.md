# 剪贴板朗读增强

这是一款用于 NVDA 屏幕阅读器的功能增强插件，本插件主要对剪贴板和刚听到的内容（即 NVDA 最后一次朗读的内容）做了增强支持，包括拷贝、追加、粘贴、英文单词解释以及按相应单位导航等功能。

除此之外，还具备一件打开网址，公农历信息查看，剪贴板内容变化提示等特性。


## 兼容性
- 兼容 NVDA 2019.3 及以上；

下表列出了相关功能的默认快捷键，您可以在 NVDA 的“按键与手势”对话框内更改这些默认快捷键。

## 快捷键表

记忆技巧：

1. 笔记本方案使用基本组合键加四个箭头实现成对的功能；
2. 台式机方案使用基本组合键加数字小键盘区域实现相应功能；
3. 台式机方案小键盘区域与 NVDA 文本查看命令的快捷键高度类似，即小键盘区域的7、9为上/下一行； 4、6为上/下一词句； 1、3为上/下一字。

**提示： 下表可用 NVDA 的表格导航命令 CTRL + Alt +箭头查阅**

| 名称 | 台式机方案 | 笔记本方案 |
| --- | --- | --- |
| 编辑文档标记开始点 | windows+小键盘 4 | NVDA+alt+[ |
| 编辑文档标记结束点 | windows+小键盘 6 | NVDA+alt+] |
| 编辑文档的当前光标位置 | windows+小键盘 5 | NVDA+alt+\ |
| 编辑文档的字数统计 | windows+小键盘删除 | NVDA+alt+= |
| 查询选中单词或词组 | 未分配 | 未分配 |
| 刚听到内容的上一个字 | ctrl+windows+小键盘 1 | NVDA+windows+左光标 |
| 刚听到内容的当前字（连按两次解释） | ctrl+windows+小键盘 2 | NVDA+windows+. |
| 刚听到内容的下一个字 | ctrl+windows+小键盘 3 | NVDA+windows+右光标 |
| 刚听到内容的上一个词句 | ctrl+windows+小键盘 4 | NVDA+windows+shift+左光标 |
| 刚听到内容的当前词句（解释英文单词） | ctrl+windows+小键盘 5 | NVDA+windows+shift+. |
| 刚听到内容的下一个词句 | ctrl+windows+小键盘 6 | NVDA+windows+shift+右光标 |
| 拷贝刚听到的内容到剪贴板 | NVDA+c | NVDA+c |
| 粘贴刚听到的内容到当前光标位置 | NVDA+`（反撇号，位于 Tab 键上方） | NVDA+`（反撇号，位于 Tab 键上方） |
| 追加刚听到的内容到剪贴板 | NVDA+Alt+d | NVDA+Alt+d |
| 追加已选择的内容到剪贴板 | NVDA+Alt+a | NVDA+Alt+a |
| 重复朗读刚听到的内容 | 未分配 | 未分配 |
| 剪贴板第一行 | ctrl+小键盘 斜杠 | NVDA+alt+shift+上光标 |
| 剪贴板最后一行 | ctrl+小键盘 星号 | NVDA+alt+shift+下光标 |
| 剪贴板向上十行 | ctrl+小键盘 加号 | NVDA+alt+shift+上翻页 |
| 剪贴板向下十行 | ctrl+小键盘 减号 | NVDA+alt+shift+下翻页 |
| 剪贴板上一行 | ctrl+小键盘 7 | NVDA+alt+上光标 |
| 从剪贴板当前行向下朗读 | ctrl+小键盘 8 | NVDA+alt+l |
| 剪贴板下一行 | ctrl+小键盘 9 | NVDA+alt+下光标 |
| 剪贴板上一个词句 | ctrl+小键盘 4 | NVDA+alt+shift+左光标 |
| 剪贴板当前词句（解释英文单词） | ctrl+小键盘 5 | NVDA+alt+shift+. |
| 剪贴板下一个词句 | ctrl+小键盘 6 | NVDA+alt+shift+右光标 |
| 剪贴板上一个字 | ctrl+小键盘 1 | NVDA+alt+左光标 |
| 剪贴板当前字（连按两次解释） | ctrl+小键盘 2 | NVDA+alt+. |
| 剪贴板下一个字 | ctrl+小键盘 3 | NVDA+alt+右光标 |
| 剪贴板综述 | ctrl+数字键盘删除 | NVDA+alt+' |
| 打开剪贴板编辑器 | NVDA+E | NVDA+E |
| 读出农历日期（连按两次读出本月节气） | NVDA+f11 | NVDA+f11 |
| 读出时间（连按两次读出日期） | NVDA+f12 | NVDA+f12 |
| 打开刚听到内容（或剪贴板）中的网址 | ctrl+数字键盘 回车 | NVDA+alt+回车 |

## 贡献者
- 大可 （主要开发者）；
- Eureka （协助开发者）；
- 永远的星光 （代码贡献者）；
- 好奇的 01 （代码贡献者）；

## V2.3.0 更新日志
1. NVDA-2022.1 的兼容性更新；
2. “追加刚听到的内容到剪贴板”的快捷键更改为 NVDA +Alt +D（台式机与笔记本键盘布局一致）；
    - 原快捷键（NVDA+D）在 NVDA-2022.1 中用于读出详细信息摘要。


## V2.3.0 更新日志
1. 改用 nvwave 模块以解决切换声卡后音效不跟随问题；
2. 增加了剪贴板编辑器输入焦点跟随快捷键导航位置的功能；
3. 增加了“查询选中单词或词组”的功能，默认未分配快捷键。
4. 改进并优化了词典数据库的解析方式；
5. 修复了剪贴板监控在 MS Word 和 Windows 云剪贴板中会偶尔失灵的问题；
6. 修复了使用 NVDA +Ctrl +F3 重新载入插件后可能引起的销毁错误；
7. 在 Word 启用 UIA 接口的情况下不再尝试获取光标位置和字数统计信息，而推荐使用 NVDA 本身的‘朗读状态栏’功能；
8. 优化“追加已选文字到剪贴板”和“粘贴刚听到的内容”功能；
9. 进一步丰富本地词典数据库，具体涵盖以下词条：
    - 四六级、考研、雅思、托福等考试大纲词；
    - 常用短语及专有名词；
    - 《麦克米伦高阶美语词典》高频词；
    - GSLThe General Service List 英语常用词；
    - 美国当代语料库（COCA）20000高频词；


## V2.1.0 更新日志
1. 完善 NVDA+f11 的农历信息获取：
    - 按依次获取农历日期，包含天干地支、大小月、生肖等信息；
    - 连按两次获取节气信息，包含节气的对应公历日期。
2. 完善 NVDA+f12 的公历信息获取：
    - 按依次获取时间（精确到秒）;
    - 连按两次获取日期信息，包含星期几，全年已过天数，星座等信息。

## V2.0.2 更新日志
1. 修复某些情况下获取农历信息失败的错误；
2. 完善帮助文档和插件本身帮助信息。

## V2.0.1 更新日志
- 修复在剪贴板编辑器内无法打开“正则替换”对话框的问题。

## V2.0 更新日志
*本版代码全部重写。*

1. 剪贴板监控改为再插件内部实现，基于此全面优化剪贴板的详细访问逻辑：
    - 当剪贴板内是文件时，按综述剪贴板的快捷键，可以朗读相关的文件数量及大小等信息。
    - 当剪贴板内是文件时，按逐行访问的快捷键，可以依次听取文件名称和路径，并且会给出音效提示，以与剪贴板内文本相区分。
    - 当剪贴板内是位图数据时，会提示为“图片”。
2. 访问剪贴板，移动到首尾以及逐字词跨行时，增加音效提示；
3. 访问刚听到的内容，移动到首尾时，增加音效提示；
4. 增加使用 NVDA + Alt + A 将所选文本追加到剪贴板的功能；
5. 兼容 NVDA 2021.1 ；
6. 在逐字导航刚听到的内容或剪贴板内容过程中，使词句位置跟随；
7. 为剪贴板编辑器的“查找”、“替换”对话框内的按钮添加了加速键；
8. 在不支持编辑文档字数统计，不支持编辑文档选择开始 / 结束点以及不支持查看编辑文档当前位置等场景下给出提示；
9. 增加粘贴刚听到的内容到当前光标位置 NVDA + `（反撇号，即位于 Tab 上方的键），以下场景可能很有用；
    - 可以随心所欲的粘贴剪贴板导航中的文本单位（行、字、词等）；
    - 可以在对象导航与系统焦点分离时粘贴对象导航中的文本到当前光标位置（用于阅读摘抄等场景）
10. 更换了全新的本地词典数据库，将词条数目增加到 10 万以上，使单词释义更加丰富，更加准确；
11. 剪贴板编辑器默认将以最大化显示；
12. 尝试修复混合使用逐字词访问剪贴板，偶尔出现位置错乱的情况；
13. CTRL+numpad8，改为从剪贴板当前行向下朗读；
14. 优化NVDA+F12朗读时间日期的详细程度；
15. 修复了农历节气计算错误的 Bug；
16. 修复当剪贴板编辑器内无内容时“更新”和“更新并关闭”无效的 Bug ；
    - 提示： 当剪贴板内是文件时，执行“更新”或“更新并关闭”即为清空剪贴板。
17. 其他的一些细节优化。

---

## V1.2.5 更新日志
1. 修正剪贴板监控程序的调用方式，避免进程驻留。
2. 重写剪贴板监控，解决文件大小统计错误的问题；
    - PS： 感谢小康老师编写的剪贴板监控程序。

## V1.2.2 更新日志
1. 修正在某些日期获取不到农历节气信息；
2. 剪贴板内移动字词时可跨行移动。

## V1.2 更新日志
1. 增加对连续英文单词的拆分支持，比如： "GetWindowLong" 使用上/下一个词句浏览可拆分为 "Get"、"Window"、"Long"；
2. 快捷键浏览剪贴板时可记忆焦点位置；
3. 增强打开URL的能力，增加了对于 "nvdaremote://"（NVDA 远程链接协议）的支持。
4. 集成了沉浮老师的剪贴板监控程序。

## V1.0 更新日志
1. 增加对剪贴板内容更详细的访问：
    - 上、下、当前词句（解释英文单词）；
    - 上、下、当前字（连按两次解释）；
2. 增加打开URL功能（代码来自好奇的 01）。
3. 词句切换后将逐字移动的焦点放置在词句的开始处，便于拼读。
4. 重新设计了默认快捷键：
    - 增加笔记本方案；
    - 避免占用 NVDA 本身快捷键；
5. 可在插件管理器点“帮助”按钮查看使用说明。
