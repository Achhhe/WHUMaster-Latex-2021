# WHUMaster-Latex-2021
> 武汉大学研究生毕业论文latex模板

## 更新日志

### 2021.4

- 修改“攻读硕士期间科研成果”，可正常显示至目录
- 修改参考文献中会议格式："[C]. xxx"->"[C]//xxx"，与GB/T 774格式一致 【具体见.bst文件中修改说明】
- 参考文献中添加@misc{}，可引用电子文献[EB\OL] 【具体见.bst文件中修改说明】
- 添加word版本的英文封面【latex版英文封面不居中。。。逼死强迫症。。。。】
- 删除图表caption中多余冒号【'图1.1: '->‘图1.1 ’】



## 建议

### vscode+latex

毕业论文用vscode+latex写的，编译很快，自动补全，插件多，总之很香 【[点这里](https://achhhe.github.io/2021/05/02/vscode-latex/)】

### 分章节

善用`\input{xxx.tex}`

- 分章节编写，单独编译
- 图表也可

```
\chapter{绪论}

无论使用texstudio还是vscode，建议
\begin{itemize}
	\item 分章节写，input进来，可以只编译当前章节，其他注释掉，节约编译时间，不然当工程比较大时，统一编译很慢
	\item 不同图片、表格也写在单独tex中，input进来
\end{itemize}

input进来的好处是看起来清爽，而且注释方便

\section{研究背景及意义}


\input{fig-tab-tex/tab-rain12-rain1200-test1000.tex}

\input{fig-tab-tex/fig-unroll.tex}
```

