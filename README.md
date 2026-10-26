# Transformer 结构学习可视化

这是一个面向初学者的 Transformer / LLM 结构交互式学习资料。页面使用一套可以手算的 mini decoder-only 模型，把输入、RMSNorm、QKV 投影、因果注意力、第一次残差、MLP、第二次残差和 LM Head 串起来。

## 页面内容

- 完整模型总览：从 batch token IDs 到下一个词的 logits
- 单层 Transformer Block：点击模块后跳转到内部计算页面
- 多层 Block：查看层间形状和每层输出
- 推理模式：逐 token 生成与 KV cache
- 慢速自动播放、暂停和继续播放；可用“上一步 / 下一步”手动查看，同步更新文字说明和示例结果
- 数据并行和 MoE 的结构示意
- 所有主干张量都使用具体形状和小数值例子

## 打开方式

直接打开 `index.html` 即可使用。也可以把仓库启用 GitHub Pages，选择默认分支的根目录作为发布源。

页面中的参数是教学用的简化示例：结构对应真实 Transformer，权重和数值经过缩小，方便手算和观察数据流。

