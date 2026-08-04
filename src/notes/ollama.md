# mac本地大模型ollama命令

一、基础完整流程（日常标准操作）

1. 确认后台服务开启（只需开机执行一次）

```zsh
brew services start ollama
```
关闭服务：
```zsh
brew services stop ollama
```
2. 进入交互式对话（最常用）
```zsh
ollama run qwen3:8b
```
出现 >>> 就可以持续聊天

• /bye 退出对话，释放模型内存

• /help 查看终端内置指令

3. 单次提问（不进入持续对话，用完立刻释放）
```zsh
ollama run qwen3:8b "大一医学生如何联系导师进课题组"
```
---

二、高频日常终端命令整理

📦 模型管理
查看本地所有已下载模型
```zsh
ollama list
```

下载模型
```zsh
ollama pull qwen3:8b
```
删除模型（释放硬盘）
```zsh
ollama rm qwen3:8b
```
查看模型参数信息
```zsh
ollama show qwen3:8b
```
⚙️ 运行监控
查看当前正在加载运行的模型
```zsh
ollama ps
```
停止正在运行的模型，立刻回收内存
```zsh
ollama stop qwen3:8b
```

---

三、两种启动模式区别（重点区分，避免混乱）

1. brew services start ollama
✅ 后台常驻服务，关闭终端服务依然运行，推荐日常使用

2. ollama serve
前台运行服务，关掉终端窗口服务直接终止，仅用于调试，不要日常用

四、适合你16G Mac：带内存优化临时启动

如果你不想用brew常驻，前台启动带上优化参数：
OLLAMA_FLASH_ATTENTION="1" OLLAMA_KV_CACHE_TYPE="q8_0" ollama serve
五、实用小技巧

1. 不要长期挂着模型占用内存
不用AI时执行：
ollama stop qwen3:8b
2. 想直接把回答保存成文本
ollama run qwen3:8b "总结噬菌体癌症治疗进展" > answer.txt
六、最简日常工作流（直接照抄使用）
开机首次执行
```zsh
brew services start ollama
```
开启对话
```zsh
ollama run qwen3:8b
```
使用完毕退出对话
>/bye

# 长时间不用，释放模型内存
```zsh
ollama stop qwen3:8b
```

1. 所有模型文件默认存放路径（Mac Apple Silicon）
~/.ollama/models

2. 如果局域网平板/手机访问本机AI，我可以给你局域网开放配置指令；

3. OpenWebUI下载模型 ≡ ollama pull，图形界面操作不需要敲命令。

