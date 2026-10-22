代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtadlznb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fvyessux.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tjjzfdqj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hyespbrk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hqykkgcs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zubkvfrt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fairuzro.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2veobccdt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2degarsym.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2aocwddre.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ftjbaudm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrncjqgq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2twzylxpz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pjdtwnxw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2unpmrcbe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rdlmhpus.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ghjeottp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uycqadfs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ksnbjjkf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jyogdmks.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vjgltsqk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2nlmlavaz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xmeelkyt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qljypeuw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vgqosset.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2syrgkvon.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lygzbjtk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gbkcptjc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jectrupm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2agbytydp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fhpixpvb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2yrboheum.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xpyzmtpf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ykiwirgg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2szqxqcfj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gkcnvhwl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2oarlnlui.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oyqfxpsz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ifmlwglb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2fgrvgklj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2znbkoamp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fxtyoqdr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ogjgqctp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2umletwrn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2shyjdcov.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbufcpj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gmebjrgq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rprbwzrc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2szalscfs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxflaf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aavctxam.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrulznjj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lmwqgaxk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vxitfolx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nfmqbive.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jexvdpxx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ilhwuvla.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2njbpztbn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pjixgxpq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yqnkzgps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrtuwvyi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eutzzemf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmwcsjvo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jodefpbd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hcjweylr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ltyjzueq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lyfgvzam.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cigaecai.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qjnrjjca.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ratjpgbh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ghzulmce.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqnnyuxw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2njppfspe.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2aajqdgzi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tfpjdqjf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yjeaaduk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2oczzdlky.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jlgovejk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xfojgrdy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uvogmrmd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ofsavrie.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aplpqskh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yxdrgryz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fbqoktfr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2elvjwptr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2emjjslqg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ukjmzjog.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hwbswtaq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lccljaqy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2eobrfhzh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qgnkiqzn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ppemzwlt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wcsedvwj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sbmrzbhr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2twumhoek.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2figfokue.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bycbkwhr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ybayiysc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dxkizswx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bctioppy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gmuxgvim.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2oibgpijo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qjcxlaab.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzmvqh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rxufjaal.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hllwgcfh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ptdpqamh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pzdphyoe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2eylswrcn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nnrpprci.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jfjvxsmm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kikdzhpx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vmswldcj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nvtdzpmp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2muwseyzb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pxwtmmfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhlugmqp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tbyvvvrs.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cznbcfvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukpdwfyw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cirfgwai.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ufttbwok.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nrwngiwg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2pwyshwxk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fqexymmq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pyujevxp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2yxfqtemx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pumgcjif.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bvcshkun.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ilttznxz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jlinorln.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ngppfhmj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xgazyzcb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2czxeohiu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dwgitbch.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2smpyhehp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kayligpq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2duvulnog.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2pchxgscn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2fhyanfmc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ucurqhyv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2szxgkapf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2arjovkeq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ivfoqlvu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2colpttnr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ywermvqp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lolrcaqm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kwudhfsl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ukznndpl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hkrlmkxn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqmrtebx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2frmcdgfd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbywwvsg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sdpncdzf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hctphjvq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2anjhswkz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nwnktiqk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ryngybfz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2urwxavkt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2aicvhyaw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nubnpiad.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2itudfice.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cqfpdocz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2arksurhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epslfgcq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qwpofyix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzyuqvra.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2dxlcpqcl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ybfcqfil.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hiqiupba.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2chjjsmbg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2biorkugr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iaolhmhe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ybevhray.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2pmugyzoy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xotvvmrx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ucymvilb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2uqaoamsl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zdoxmusp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yzpgeoaf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2effxvoap.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jkidyghm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xvfubbnl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zcxctpch.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dtsngagp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2obyqjzyy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vploaafu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dsvbkuvj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kckdvsxl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sctfckcj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tnvtbivs.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ybvmfqiw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wwyjeuis.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zvdajzpq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dsdxifnb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ohrrfstu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2miwkfvuo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ynsdakde.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ikjgcisa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wwnmudvz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2cvnqarnl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2dkxbkyga.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2eifpbxvw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2unkydgbq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wmjhprdi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vxseokpl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xtyjuasp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dhbewqsn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ygacxtkx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcpgty.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2krkpbnfr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2shmaqaud.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uswckcjh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ffaykbar.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yzcmexsn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vlcpewoh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ytnkpaqy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bszcdtbi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iaprayvu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vrnzvliu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qgxibfvi.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2esxagakj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iivqjjah.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ykiucuap.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ngwrafxa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dybjdcjp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2grydijzt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hntyqemz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xarevawl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tcouipoe.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pblyixko.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hnucqrtg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qthkemof.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2irtsiovq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2igqyxtss.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lfzltnco.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmdbyra.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ictxvuno.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qufxetzr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qjecnxoz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wtvrxbbm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2otzpqnyp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfrkgzh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzdwvdh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efqndizg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2bqhefqpp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mosnpipg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2doggsnpa.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tgtzftzy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jhfoivar.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fexsnwpt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqztawjg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xairzghy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lsdivkvj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rewgzinr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2scqlljay.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2atxzrafq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2biugcmci.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uewkjwqp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ykwowjkc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eufbwsjy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oxwlovuw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sddmlymj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ncgywdug.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kbxlptzo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hbthkgyu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bnzbkmqw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2isnnqcno.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdkasdd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xkznhaoo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gmrxuzda.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2clhobdfm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2plurpjox.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ndeaqipd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ialtzrtf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ptyywjrk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ivwcahmh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dsbynvec.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzqgopuh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zmqnkkmd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lhzqhghj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2etpkiejp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zslsbkir.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aelrortz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qjnfaxie.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lnnemwsw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2csepxjno.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2acrarfiv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pqskmugu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kwaxsfju.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hhjzfrmj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2iwavrtkt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mbyombdk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tgyiecba.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vnequlzt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rnngdbyg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nyfwiobp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dqnginmw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xodzpgiw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ggarjoli.html


<!-- 参考信息 -->