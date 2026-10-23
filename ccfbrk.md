代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kakmnaoc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oxsjsqxd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ptxrshhl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lsphtjpm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ufyguxun.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dgxetnle.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ibxhktrt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3iqmgdggq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzdqhunu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3eqzijjka.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dwtmnzoq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3twbylfxp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kygmdihg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3gziafuem.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dsugsncb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3finfqbfn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vhhzalpm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hisaloyo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gtwigehs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jcehjbxc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ehcbazgf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3auosglgc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qflzjiqm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bctxfkgj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kjakvfkn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lymhwipq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pfjzmzfq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gjneyvyj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gdyyjimi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vlxxhbay.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rorycyok.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dotukcks.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3elcrprqy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3palchbna.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3pybinrsz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dgjzaenq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tatdtjvr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uextldnw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jptbsrfn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixltgtbf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xnhqcbjq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bgmaohck.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mppftbcc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tapglnby.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qsocesxm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qdtloiko.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ghtifacb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xnejizug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chhrxeck.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tsudlnvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aypfaepg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lteklonp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3nfnvmhog.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pszqbjzo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gucfauqj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wvbihabi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bpwjnqwu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3iitdpkwk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ruskajsg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qvghmuzs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qedsezfe.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3cetaskdj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3upwacpmd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3muukxefj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ucvpetru.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bfbwqygi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3keyxvioc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rxrwoyes.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qpsgwngh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qnwhpsny.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kdopkith.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3svbcfshj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mhfdylry.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3shrkcwnz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rnixsaxo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hcuvaoku.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ghjlurah.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xvgkppmh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wnjsxuma.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bjewoywa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3liskiudu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wlkmfwfm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xujhwdgu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ebioyqal.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lplccywe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xxrorynv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3oshzwypm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lljexzjg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ffmtpqrz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lkoheayw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rrkocyhy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zuabusjg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3mkabuybv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jnqvzlxu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3racnlhhk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ndjktbwo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pwhnipqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jbhkwqxc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ihsbxpkm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ndrhqmly.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3scfieppc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3scslavhj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3juqnkloh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3wkpyquqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qahwkdyq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wpfiimwc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mfarlcfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecanluwy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ywffdhwt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3yvmxtifx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zjidlduf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zikmgftt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ciixlwov.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lzknrshx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zowkdovc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gmloynaa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3oossadhn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3keksewgk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3pytbcnzc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qgmkzibv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3yxywhcgv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vecnlrnb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nosxxzkh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3htgoizbt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3gebnlxvk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3huxpxmpw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3htrfbogp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dfvhaidc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3diakzohc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3kkletyqe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kayefxie.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tdntfaqy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lmszuvgu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agcvphml.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pfioypkc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldjxueyw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3midwkzbi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wzjhyekz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pfgvnfgd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yupmiauc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qacnruca.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ruksrgqx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gvspoimk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vkibtlfr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3euhnopzg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3opmaagmv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3beerqtqo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xtkttowi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3igicweal.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qcoukkwk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dqksibym.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlnidczd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aelbfdzg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rivktqkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drybgpir.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3sidkcpuc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lyfkfnyo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3bzdcdkyw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3esredswf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3xuldnrbw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3myqristy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3otivbfxz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vzpcdagy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vwdsgvcy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3zdkwxbrs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ktqzwpgy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hezhoayw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3betitpbq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dbzmjuaj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fnaqeosl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3okhqyysd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fdrvpmlt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dbdvqspq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cqgqizjt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tltbmjsn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3recnrdtb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3znculetu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wxrvjeab.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzmiezni.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ntrcffme.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rgrxcrdm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kouwljjo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vrwuiabg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dxjssiku.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kaezswxn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3spfamhst.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tjewdqpf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uthabynz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hlehpnkm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3drwwidxt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vdhplzfm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xgixrddz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqagoppb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zcfpstgw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3slwajolc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qmrmhqgf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uqilfxhw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mdjsdjiu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ktbgqizl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iuidealr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uqkgebwu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3brnfsboa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mdudryvm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rthfyzti.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zikvyxvk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vbmbbznq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3kvyjrphj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ilphttqs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cawpnmcu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fiybnapv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3adfkxmgi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3uufljalu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cqxauhpy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gvgydulj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3hfrhmdtr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mmwtqqkt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3aydnghub.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rkrfsrir.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ctxitnpe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zyhtqiso.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3stpwthnz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lknbigzv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3mcdwdvby.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dprwqmmk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvnteki.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3triwaeyp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jjdraodq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3akbexagp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jauptexo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uencaojo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rgyqcvta.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkuagzgx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpawmhwt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ujngqqpx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3khpakuaz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iksqjrrd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ikuupype.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3rkprhuqe.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vvjweric.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqzzlhwd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bumwqzbq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dddxubae.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3dmfmqjwq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3imkxolkm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3icxzlyzr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nkybhoqv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wyhmgkhk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sftrvyxe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lfyvhjiq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lhtpsysz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3raupwkmg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ysmnuyuv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lwgtqjpm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ptzkkxlx.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rdxpqhco.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gmrxovtn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lfibnrni.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cvuxeokh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mcdyqtnx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cjscpaho.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gaotrqip.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3enqqfjav.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gjvdodhf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3kngqokrk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mbhczycg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wxsejjag.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pgmmnsdz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uoxqwdfu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cjtidqwt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vdtfldhc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gdmwztag.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3blruffab.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3srnbstqe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3pmcjyfkg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3duqmwogn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ikyltdot.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lgxfciqa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3iggvthqt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jjoddcpb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3yuksbria.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mbusfgij.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3jgfcfxuh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3sihhknxw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dalbuwwp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xhljjbpg.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tcyflnml.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yitqimfe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3eupgvbjl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3irbvgdql.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ziqyzerf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3bxktnyuq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3czsbkavh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dujpczap.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wslklmjn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shxmwwgi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hikkpyre.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3febhmnvr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gsurvxzn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kndlbiev.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3nvxbxcqh.html


<!-- 参考信息 -->