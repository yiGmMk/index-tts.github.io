# B站开源TTS

最近，基于大型语言模型（LLM）的文本到语音（TTS）系统由于其自然性高和强大的零声音克隆功能而逐渐成为行业中的主流。在这里，我们介绍了主要基于 XTTS 模型的 INDEXTTS 系统。我们增加了一些新颖的改进。具体而言，在中文场景中，我们采用了一种混合建模方法，该方法结合了角色和拼音，使多形字符和长尾字符的发音可控制。我们还对矢量量化（VQ）进行了比较分析，并使用有限量表量化（FSQ）进行了声音语音令牌的代码书利用。为了进一步增强语音克隆的效果和稳定性，我们引入了基于构象异构体的语音条件编码器，并用 BigVgan2 替换语音码解码器。与 XTT 相比，它在自然性，内容一致性和零声音克隆方面取得了重大改善。至于开源中流行的 TTS 系统，例如 Fish 语音，Cosyvoice2，FireredTTS 和 F5-TTS，Indextts 具有相对简单的训练过程，更可控制的用法和更快的推理速度。 此外，其性能超过了这些系统的性能。

![image](https://github.com/user-attachments/assets/5211e2db-0c0e-4b0a-ae47-f60dd798ce51)
![image](https://github.com/user-attachments/assets/223ef00e-90ed-42e7-89e7-f41b19012b1a)

