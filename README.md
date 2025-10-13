# linalg-homework

欢迎使用这份专门为咱们线性代数课程定制的作业模板。

这份模板就是为了让课程作业的排版省心省力，看起来又专业又整洁。基本上，你只要填空就行了。

---

## 认识一下文件

你的项目里主要就这两个文件：

```
.
├── main.tex        # 📄 主文件 (老师出题、同学答题都在这儿)
├── config.tex      # ⚙️ 样式配置 (管着颜色、页眉页脚、格式，一般不用动)
└── README.md       # 📖 就是你现在看的这份说明啦
```

-   **`main.tex`**: 你大部分时间都会跟它打交道。
-   **`config.tex`**: 这是模板的“后台”，除非你想改改颜色或者字体，不然完全不用管它。

---

## 怎么用？

分两种角色，操作都非常简单。

### 👨‍🏫 **如果你是出题的老师或助教**

你的主要工作就是在 `main.tex` 里做两件事：

**第一步：改一下作业标题**

在 `main.tex` 文件最上面，找到这几行，改成这次作业的信息：

```latex
\newcommand{\CourseName}{线性代数·2025秋·第一章} % 比如改成“第二章”
\newcommand{\AssignmentTitle}{第一章 \quad 行列式} % 比如改成“第二章 \quad 矩阵”
\newcommand{\AssignmentDate}{2025年10月13日} % 改成作业截止日期
```

**第二步：换掉题目（最重要的一步！）**

往下翻，找到 `\section{综合练习}`。

你会看到一个很显眼的“**重要说明**”框。下面的所有题目**都只是为了演示格式的占位符**，请务（yi）必（ding）要把它们换成你这次要布置的实际作业题！

-   **想出选择题？** 照着这个格式来：
    ```latex
    \begin{exercise}
        ...你的题干...
        \begin{enumerate}[A.]
            \item 选项A
            \item 选项B
        \end{enumerate}
    \end{exercise}
    \noindent\textbf{答案：} (       )
    ```
-   **想出填空题？**
    ```latex
    \begin{exercise}
        ...你的题干... \underline{\hspace{3cm}}.
    \end{exercise}
    ```
-   **想出大题（计算/证明）？**
    ```latex
    \begin{exercise}
        ...你的题干...
    \end{exercise}
    \begin{hint}
        ...可以给学生一点提示...
    \end{hint}
    \noindent\textbf{解：}
    % 学生在这里写答案
    ```

那个 **[作答范例]** 是用来给学生展示怎么写步骤的，建议留着它。

### 🎓 **如果你是交作业的同学**

你的任务就更简单啦：

**第一步：填上你的大名**

在 `main.tex` 文件顶部，找到这几行，麻利地填好：

```latex
\newcommand{\StudentName}{你的姓名}
\newcommand{\StudentID}{你的学号}
\newcommand{\StudentClass}{你的班级}
```

**第二步：开始答题！**

直接在 `\section{综合练习}` 里找到老师布置的题目，在每道题下面对应的区域开写就行。

-   碰到计算大题，就在 `\noindent\textbf{解：}` 后面写下你的神仙操作。
-   不知道步骤怎么写好看？抬头看看那个 **[作答范例]**，照着学就行！

---

## 技术小贴士

-   **编译器**: **一定、必须、务必用 `XeLaTeX` 编译！**
    -   *为啥？* 因为模板里用了 `ctexart` 来处理中文，用 `XeLaTeX` 编译是最好的选择，可以避免各种字体和乱码问题。
    -   *在 Overleaf 上怎么设置？* 点击左上角 "Menu" -> "Compiler" -> 选 "XeLaTeX"。
-   **平台**: 在 Overleaf 这种在线平台用最省事，当然本地装了 TeX Live / MiKTeX 也没问题。

---

## 关于模板

-   **版本**: v1.0
-   **最后更新**: 2025年10月13日
-   **制作者**: [请在这里骄傲地写上你的名字或团队名]

祝大家用得开心！
