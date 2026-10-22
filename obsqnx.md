代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mkqtyykw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ajmqhsym.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ahhokrve.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zdnpgdse.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fxwohgwj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jurbnieh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2sysljene.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jdshjjry.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jjzooolk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sgegczpk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2imuruqco.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdghqpds.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2syvjhblx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jlebqxpt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rfqfeibe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vsvrzngd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ewsizovn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jsrurjrh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2uumctzsk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2owlwxeoz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xqenenre.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2omzqwnap.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rpahkqvk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2evsqvruc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2opbdvvmc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gzoewksw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2umxbfhqs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qtebcuma.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rghbnfvj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zvsilldi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sxzvvghg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2awltsuib.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hyfsitdp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ojidpkcb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jmapdwlg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ozcsrewp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2pfzgxinm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ebokozru.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mewufvpq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ltjwfabg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jlesjlda.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2otititcc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nuxjztom.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qnvncajo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vsxdmhfh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gdtfmxyu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pvtmddjd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qslzcmzw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2padpgcez.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rtyimdyo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wjmstthz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tunskmso.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fpqpsmvh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frjdwvah.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kovyxftx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oopsbvao.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2brasibad.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2egdowstl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vkythfzm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqaegcdi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2clubsree.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qlccueep.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jlcanrtj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hlmfakre.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fxjtpyia.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ezbqbtmx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ypykwerz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wzwxwphe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpzpiudu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2drrawzjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkukxdki.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gcquwpjh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ttgivksf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2znpsbkeu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uhwattbg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jdrlixha.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qirvnkzs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2erzrldnr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qteubwzy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jzueghcr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mmpyssma.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2aicfmezw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dlknxopx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2dccnybsw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hkxpslqt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rdtkcpej.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2uzasmdzy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2upfvuena.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hbqxwinw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wraiepdf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2gjuftjvh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2iyqrxqir.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uwjgjxnn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ptpatlxc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xtqycibe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ekjpsrnc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2rpfvvuan.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ixeezrww.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dtjqjcph.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xiffacld.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eokaqxyg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fagdtyhv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zrmdrqvk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tflrmbrn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ozuvuxhu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rudzrknz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2sdcnujkl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ykbklsju.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2pxaxbmqs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qkqppyqk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xssfmfwi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fbnlzxgy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cimedwmm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hvzpgtgo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mppdhwyn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mvcxnwkq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2addrhotr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2epquvnfo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xvoqyhjb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pupqghiv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gbfxujsk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2vsfkrbtd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2beqvicrj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2yoxqgpol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqfcjbth.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nnvnsdrz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2uetbjpcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhojkyvp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2silpkagp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jiqzmmdy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2klolgsaj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ubijthor.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2oxcefowz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2srzkiakk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ubanhgvo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lhgnibpc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2zwtenfkz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pccqumyl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bttdtbbg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2azufawyp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dgiwkujm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2fsjyuujm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yjafombo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2viqgbpts.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2seuenzky.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vldvwafw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jkqrqhpg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2zpolnzuj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wxqdlhmd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2brnfjnsh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cwbrswln.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qxabrsag.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yoiorpkq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rwqpnpbt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wgpctyqx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aavghdpn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tlucirpj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnaotoni.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bysgxhft.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vcewfhoa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chhfprpa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xsqxqbhg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vswuixsw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uphmmidu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wyykuyaf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pckiomww.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2syaacbss.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqymzfni.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pldxmnqu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vodjkglc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zoaauaia.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eumtvyxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbeebshp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rocarovl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgpdoibn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yefcwkjj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2osnkiiar.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2djugbzqz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fuakymlb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2nsolhbcl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gmigpvqb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ljeetluu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nivfpevj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xzzvdual.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hxlphktt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vzfmvxrp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2igoljvlk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ovehzsqh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ddxfqabs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2okpoahdt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2awmkvgep.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xqcqlodj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zhoxvowm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ehuyssxf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2cqcpsfec.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aqakloxn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vcyxqquh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zotmnfyd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fmktlhkl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nmkvoylu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pcybapbr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dmqdbhwv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qcprouer.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ywvwqjcz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jmvvqyyn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2amceeill.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tpzixlba.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lxlnrurv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ceryqvnq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2cztgvigp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2iskdwgbf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aeggpcwo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntxcsoin.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qrsiuocx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fvdzcihi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qujclkpn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vbrkggst.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ixebflgm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sorbdyfb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zxtoytix.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pthxehmg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2khrbtttl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gsfdrpyr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wbfnfirj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hhhpdoxn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2otsaqefl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mksikgpd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2whirlefc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yxegnray.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwyzxukd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fvujlrvr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2iwvfklcx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zztptfvx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qbquhflg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2afwzuntm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dhdooysg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yfgknmyj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ualewwiy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2amcjqnkm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qjmadxhr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2aconjkba.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aaylfdmf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2sciircke.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2onoebnbg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fvjjceud.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2xrqgyipg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nckgpuzj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kjxorbid.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubojksxz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ytqrpkzn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ptnqzcvq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jztjmzhx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhqsozdl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2urjjmmml.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2tasmwboz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwhimjl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2djksfmlk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ljkuhmew.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2sdbunopx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hwftbscj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xqvqymwa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxecmwds.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2pxgukkuc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2abmewyfv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkwyeca.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gfhduepr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fbpqyzhn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lhhjkmep.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2txjeetgv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dcdhjlvf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lbdsiakq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jzaaxmmz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ydhtikzh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tttxvdzy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ejjnhnym.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vkmologv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2avuweyzo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2whvapcmf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2piheiyvh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlfjrfc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ffhxidhp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dxspdqne.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hddbocar.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2izlghgxu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2damhfrzg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhrlgcud.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yswzudfo.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hvsddbvj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2axezrcll.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2plgxqxia.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2crbnwxhm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yhnczsti.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nqcvvpbx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rxlmufxg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wneaymkl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2icxyfdkz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gyhathgx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zsdvxgpy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fwtchhqh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2gfjymlne.html


<!-- 参考信息 -->