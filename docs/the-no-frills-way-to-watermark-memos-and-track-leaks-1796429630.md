# 给备忘录加水印和追踪漏洞的简单方法

> 原文:[https://life hacker . com/the-no-free-frill-way-to-watermark-memos-and-track-leaks-1796429630](https://lifehacker.com/the-no-frills-way-to-watermark-memos-and-track-leaks-1796429630)

假设你需要向一群人发送一条私人消息，但你害怕其中一个人会将消息泄露到其他地方，而你不知道是谁。 [快进实验室有一个粗略的现成解决方案](http://blog.fastforwardlabs.com/2017/06/23/fingerprinting-documents-with-steganography.html) ，它将暴露任何公开复制和粘贴你的信息的人，而不让他们知道他们已经被抓了。

Watch

找出你的备忘录中可以在没有人注意的情况下改变的元素:你是使用双引号还是单引号；无论是写出像*三*这样的数字，还是使用像*三*这样的数字；无论在列表中使用分号还是逗号。差别越细微越好。如果你想变得更狡猾一点，你可以用 [类似的 Unicode 字符](http://unicode.org/cldr/utility/confusables.jsp?a=fast+forward+labs&r=None) 替换某些字母，但正如 FF Labs 指出的，如果消息被转换成纯文本，这些特殊字符可能会暴露出来。

现在，不要在一封电子邮件中抄送每个人，而是给每个收件人发送他们自己的密件。只要您的收件人习惯于通过密件抄送接收群发消息，他们就不会知道其中的区别。在每个密件抄送上，进行不同的细微更改。FF Labs 建议结合不同的变化，增加你可能的独特信息:一个收件人得到“三个”；一个得到“3”；一个得到‘三’；一个得 3 分。

现在，如果有人向公众透露你的信息，你可以对照你发出的电子邮件进行检查，找出泄密者。如果你的变化足够细微，他们可能永远不会知道你是如何发现的。