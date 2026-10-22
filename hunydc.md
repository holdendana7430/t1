代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2vnazorsg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2anzkasqm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2uqdwiffu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxayerbs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lbclgehf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2felcsejg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2thxoqzyy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xhsbgbzx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gkgqubox.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pyirdafq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oqzkpxzb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xbbbyvvv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zvcwaloc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hreiejlu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qiplsnds.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qacycxrb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aoaspxsr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zyplzgld.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2oecxvltk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mncqapuj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zzbclmvr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2anrtcgcv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fuhdnaqd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vaqawnkw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2prjchtas.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ppfeyvnw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lnqropti.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fefxbhnh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2kwmlgdtv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bslqzugm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2myypasmy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xssqqaee.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qcfeignc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ubpzzudb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nqtcfcgk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qazfrxxd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cpqffjnz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2abwyhdlt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gisfynoo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2rvjqagbv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ajrrkfrx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cvjihnkh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qgiusrff.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2alzrkanz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2afgtvdan.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2gfokmvwv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xwhpidjc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxqjpdem.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xdiwbhkk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jomcwcdb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2uxmnacsj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjctpwc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fapkgyhv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uhwapohv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fonrixww.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysfrzybz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hrodxijs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kztbzbit.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wenbbole.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2oddqzqkd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2aszebrhw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2eetdrnyq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2btlrlayy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2znahrtdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goirdggm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xeppulcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdkvgpqe.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2bmfqndeg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nwdcgjuj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2dbldqsim.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mgpaeekx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2romtdpez.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mqsekfkl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cdsmsuot.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wqzynocf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2komynane.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wjpmssiq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fclphsrq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2gvnuajte.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2aaegwydg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2drubssgh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2akghadyd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2epmdfqbe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zlpmhfaj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tcbhtuwx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ykvbqcel.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bobdrklj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2iprlrdlb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pcmyljmf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2snmteiyq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jzmfrxep.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qluvozyn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2potfvfif.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2llkbraqf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2duyumwqn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wtwowpey.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2luhygfew.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xvokfwrk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2waarypxf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tvygvgwh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xupxptyi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2poxmeago.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2sigbzggj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jphtgohz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lxtlkyfq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ihpmrzzw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vdmcmstv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yjzbwifk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cbsdhshb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zendwimk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qhngocvr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2asfgzbrf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tkomynot.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dpgugony.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ueajqpwl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rxotonwk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2oyqytxve.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2xrhnlzbd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fdtxjhkr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2cwseazqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhpfmrpz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yjdhrkbw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2alyqcybp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfucoifn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zqgsjuml.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2mtwnuozx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2omlxfjvr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ksiaqcpe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2svqnjtow.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zaferrjc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2jgvpvlnq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2wcunpiii.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2covvgwlz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wzjbuffp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2rxkwhpgk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zpdxldyi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xsqkifdd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2cjhukcwm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lmhysbgx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qrbglbzh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mltwhkjz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2kmteekbe.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lalmydvn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qqdiomfb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yziivrni.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kamolshl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pppmeife.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aivvaddm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ywlfnbvf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vqxnlkip.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cadvqbns.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgkwcobi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2useayeof.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etttvmju.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vkerjnzo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2duxxqdwi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vlfndpgk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bdzciikh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qectfbte.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hevumrir.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gvlfjmyg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hpndrhwt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbkodgoz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2adswkwru.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dfeddshy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fflsthlb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sphuqnjl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2umeeyitd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thxlherd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwxlznuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpvnakiv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2vfjlnnxu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2niwbkdtv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qxecrwcm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ahkfacfd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fctpzojb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vaojszhx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mdtfhikb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2lhowkmzy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oxuahnlh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2msngcnrt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bmoodgns.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zawqgszh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ksazupih.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2cdnenenz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hupizavr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2sfmrprtp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ygtxugip.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ghkhbhsy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ktzielvs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gfkckajl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gdamtrjx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rblxithe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nvqhotbf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xjblbwfi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gusltqhw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cjfprexu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lapqrbwa.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ztzcthpf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2msbhcvop.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gxdszfwq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mmgexnog.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bazzjkgp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rixswmag.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2bydkqell.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2dvnaubxg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2iuqodthm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2gapnzbjj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gsxfizau.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uomfvmjg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aqwmpqkf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cvovnofa.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qmuyztcw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bpwnxlrd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gavcsoov.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nrivnbpz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ixzqgrtt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nijweipo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dkwutkuy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2guvtdime.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2amnfglcs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dfwrfjdj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvzgzsg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kqcqvirv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xwcdftzl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vtkcalis.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2brzscoes.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2dxuoeefk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2flrmgnil.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2exzmkdpw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zwxzfvgv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yozqdqdr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2sveeedzd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lbgiifsb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2apcyxgxp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zvcizsfw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvuuelq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aotpiyzb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2crvehhwd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rpliuoph.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xwwqkbwx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hwxxdltc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvuerry.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2feopskxz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwxlcqy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qkrsdkev.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2elmoziva.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vdcfeemf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdciiowv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ljrajmpp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2xbqpsgel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2htyuwraw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2bewgkgla.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ootzcuqk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jzihdvqa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aakvurlq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vlultmvw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aqfvkcaq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qdhliomp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrxvbby.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2seuvrsqw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mhszwmus.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vraufnzf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kklrrxkh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cszrextq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pxghwtca.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qudhjpub.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2axhsyfth.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aplniqgr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fqpxxpdl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uvullzoz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ezhlyyjm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vmkitjtu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nxplqdmz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wmkjbahg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2okouhiue.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2jdgzynga.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pftltrfi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2igmlftty.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2nnlqlxor.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qfratmke.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2atrnvdym.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kmtpzzzj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rjxephgo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eieaosoh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rqwnejjx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nyonykpi.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2damyeyly.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gkufzwfk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zolsruou.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ipgawtvc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mmvpchwg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gssdfuth.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jorkgulx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ovrcgamv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2jdhetves.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lvkndtsh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lyorzamp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2owzoqcig.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wpwyrryd.html


<!-- 参考信息 -->