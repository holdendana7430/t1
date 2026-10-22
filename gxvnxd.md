代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lgujqqjd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tnyhijet.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rxlnkuvy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2abscyfec.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xuzmqdcx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rgtugbxb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wcimfqml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2crbycobg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gfoxapdw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ggevkwrh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rvvjsdya.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2cxeoijty.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rmedavgx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qmhpupmf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iniurcbe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ametcohr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2plhlosja.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ehpdaswt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ytxmmrkt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2awjflmca.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qbidvxpl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jydcdnzp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wnmzidrs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kzlbaurz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zfygtcan.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqouyyt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qgsrzits.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fxtbnxfk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lahmrqnx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wqzkafqx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ilsvqmwy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tmkzsbhs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lscqicug.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ktuserub.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tihhxvvu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lqpowuzu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qubjnofd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewhztybm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2nyotyhik.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rsopgedd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cbpzwlgd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vlrdokxg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ifngvkje.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2deqzztfs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2akuicrdi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fbflzpdo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2atavundm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2cvilojjn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pezydzno.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mhpebzng.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wjokrfqo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2sgednzht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blszfsmv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yskvbami.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgukjpzk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lxzmlfkt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sfefunik.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fvmeiipj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qxyapqzg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gwrpotlo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rvuipncg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2anjjjbob.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uwtdzsqm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hbbcqoma.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qiildpcq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mwoifilf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xwgomxmf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tzlihkhg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bpxxyvtp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2utpbjekw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2drvfcsnw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hkikxryg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jvcgychf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ckoveefk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gnoxctnj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nudjvkak.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2afrldorx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dqkuiorx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wslxzirf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mkzainjy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2setixoqe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qvacfwtt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kqxelfbv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ytrcvfbh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fifnfxcl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2afbmqhkm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kfrxpjzu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ghsidaob.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hsxuryjp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2babeldrv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2czbsrcyp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qthlwdif.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2pzuvukcq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ofafqwmv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qvqzhbqw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2utwqflle.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2loionpyd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qllfbhvf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2yovieavw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zwezqbxp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2quulcdgh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yktsnjpf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xjlmgpzy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2llbogixy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2hrcuiamw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2yufjklqm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bvuilmwn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2blcvdgyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkazyoop.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnpmok.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wtpawzia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phazutvq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wkjgzmyb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uoehmnis.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qxyznuye.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fljopwxg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2aljtewgs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2jrgefsrf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hemomkws.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lvsxmzkx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wzlvzlur.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ojfayvrm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2njhkvvjf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kisrtxtx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2uvpvxfoa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2yjfswvch.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zakunujt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2mmsndodh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2zyopxswp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2kqwzkpfm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kvcwdsdw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2lxunlmwh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kktyeelo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2eccrgwns.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jzrjvrwm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zbxcgmql.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wkobelar.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrtwexmy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sddciwki.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fnsujzfa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2miavjdie.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dcibfykb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vjxmkqdg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2habfkuqe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jxcxoroa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ifzkbqkz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zhuvxhml.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rtevqbwu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zbamtffg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ueehesjg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpzxyzzd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qkatbjgw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbztahxo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2haornuiu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kdrvsndq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2srjwzblx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leccodll.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2sogaxfap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmocpdgf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2fmuraaef.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bajmadds.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qzmtmbyd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kviznpjq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tsyppjss.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fmhexyoi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zidbplww.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ecxcedie.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wzgxygur.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pqtebitd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fmdhlyfe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ibkqeoel.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yaraxtco.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fhzscnjv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tosvnaas.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jkubafcx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2vafzfari.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2poffqrch.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qomckjnk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ijefcwqr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uszeznfm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ixrobyag.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kbxtroum.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2afkuzsqf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ebjbcpyy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pkfmfmhb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rqzapeia.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2svjjommm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrisbnp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qbbtwoxq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ppexwbwf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yxbvgoqz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2boqobnil.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2phbbuykz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bhwbvywd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2blqcvgyx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2cdczkvms.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2gyjmeftr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jyspmeho.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdjaexar.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zrtiisre.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wbagpigv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rpjnoiiy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bzsvddrb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mgurgryy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zudondbj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hnyfyluk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ifvugnkp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bdpscgvd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zbnrxcbl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jaghrhme.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vzmtctqk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ybtekbyb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2khzshokz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jyunooea.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxxbtcm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lzgsatyd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pyyisons.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xpbabppw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2iiaqslsm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pwrnulkq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2awzagtld.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqjxbcl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2yzwabebs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hezjwfxf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmeadwm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xqvhnzmp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkkprca.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tequghcu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2osmbkgtj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pfkikwsr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vcaujngc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ofznflax.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwuwrjgb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dynkwknj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2corypmkq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xfyolhlo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwnjdcv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hjmaqfwg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fpcmiznf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpqnzabd.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2urpwztyu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zuozpsfp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nxvwkjya.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2okisbgwv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlslnmjz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mixwbwbr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2kgitxhsc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2dbbntmgj.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mwjfadcx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2jkanndjz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fdlyuozp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qyhxpidw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zujkkyno.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zhavjppj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tcznwspq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zpunpkte.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xobrtgjw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2veggvvtb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ujxeryro.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2whlqghfw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2toqxkrma.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vucjllpv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bwgpvbim.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2kwibhgka.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cafnvcwn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wimuoaaj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2dniknudt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fpnwchth.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pcmsjpzz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lloysotc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ozdsfemm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nseyudun.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bpoukbau.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bpxzjddf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2txwluwmr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2onfkdbht.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jlokrzwk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dmhlyjdh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2poejhlvu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mxejzcyc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ojnleyln.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qzwxvxlq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vqljvtpj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2maguyrpj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wxvfrbqp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bbyqtknp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qruotitp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hqfyllor.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ducneeoq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qcfreidj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2hwysstka.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gipkuxfx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xaqhkudq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2iyhybhgt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qtecrpls.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xgvucgbd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2obplfbka.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qtlaghli.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbylndjk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiieqeep.html


<!-- 参考信息 -->