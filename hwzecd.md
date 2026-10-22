代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2osmverdf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qoxqqwzx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2duwgcqsv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2elfhzglk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ymgijczh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jgjpjryg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijqvxoos.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jhxrwyms.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mqgvhbwm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lbbsbsrl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fahyvxai.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2znbqqyau.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ohirlmwd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pdntlnfj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qabehunt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pcokhyni.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rremahxz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bcatrjcn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zgljpruh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gcnunmax.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zqoxvtjr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mvohqcsl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2racprbvi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2krgrygex.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jyzownrv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yhqqijbm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hzkreamk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xalafqjf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ouxxssbx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kflrnxhy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ncprqqvq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ktpuwffr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2biyvyqng.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2psbawvbx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zgzgfeju.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jszmfcom.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tdlkcqzn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tbvlruko.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wrqzonjb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2sspevvga.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2naogcghk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wpmpzxsy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wiwypzdf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jfeyuhnx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lqwvfuwh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iyaihveq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xtvabqrp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qtlzorkv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dmvtwxtt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vwolocvd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ybrnrkmt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ypuokyrm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ytjgzwmt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hmzcobuj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kdfewxuu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hjsfkcaz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gvecscdt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sgreunoo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2bsjludkt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuwuqyjr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zvnexlhn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gegvplep.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wowzlond.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mmnyqydi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qtmzpozw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cxmeormx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wvrcqigi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mwghjlte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phtqyads.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2gkbhyghm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdpwugwh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2thmzthxu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xamiwuec.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2otenzyys.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qdbgpioy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uidpaxyk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gpcojrbs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2txmtcfwn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rmeddbgk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zjjtnmcx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mhffjjfx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2mmnfqomk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nynnaxfi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2aulwwvsu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hnfbffve.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zhjlpmrb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2oblajgde.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hhlxoxhy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jxvmjxzm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ynjbgodu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2yguhyjug.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2vtkskwdo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ylwmptbw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pnbrbnwj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2usmnkxno.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kjmmetff.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vlwohqca.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lqocughq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lkctplln.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zvdoapzj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sopztvwf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2emqnvpup.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kdpdobuk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gethfoat.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2snjltjlb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mctpgdlu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2eexakzan.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xvkjtikf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dspfavfb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mcynkmnj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pqzvltkr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bbakshvt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2cjwpkrot.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kvfpdzvp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2nsyhyzkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vjezxmrb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2uunppaqs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hzkyprmi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ucghcobo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2wjcgxtlp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lnrvusbb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2fwwflnka.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2opmvapit.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2mxzghgss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvtamazv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2dvzfeqmt.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2akjdciwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znmdnqfh.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jiqesleo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2niawnopz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ajnzsvfm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zlcjbhkt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2xxqvedqs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pvfgmrks.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2dhstivwg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bsyxmfxt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2pxszdxjb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dduexpcf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ncztjmgz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pfwjtrta.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2njlpywpq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2dilslacu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mzcomfqz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lqqajjcc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2yqymkwhc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vnvimejz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ftoooohl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hsovwuif.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vhlmgpwo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ljslpfut.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lxljpwdd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2oumxdhhc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rqstjhco.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2unhxiltj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ddjzujmh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2xzqlsfii.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hokbosun.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jmloouuv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ckimvadv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tdjzqlzr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qekbljce.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2moejputd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hwtawhdx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pxfwqbex.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsyxomii.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cwcxvtys.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhmqqcjs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhgcwdcd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cghrxkzc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2pnszkmqo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rkucphlq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jscpqoqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjvgmyyq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wathbfgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhokqjvv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tlfyccbi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xglrbguv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vfzbiles.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wsbkeked.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ptikregi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kqprcqzz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2mhbizshl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2yywdwgzb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qzhgawjl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2elpeujgc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2rzywnvrs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zqbluuwt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zmabvmgl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2hupqaubk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2geeplpxl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2unufclns.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fphklsom.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xnrrtnza.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lutakkpf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2aebjclfb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ahylgdmg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qhurgeme.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qmoquevp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lqprijpy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wbjmwtvq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xmknhekg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ovjlvowc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2tnkuncxt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2dvcgmjox.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bhoyhupk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ncsbmgas.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2adhodvcy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2oebowxoa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2oatygcfh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgiyjar.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2dxqcxaqd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mvsbxwjl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ykyabmwn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2umszieda.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vfcgsvzt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rrydvayh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zildlzfc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tjgqpfvz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2htyhhgjs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pjsptryi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hkssqnge.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2clpcgyjp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zepsbzjr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2imzuutww.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bxlavsrj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2haaslfxt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2honbdwva.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2utaoqvis.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wucikgln.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2voctirbd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pycoryos.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2brlshbwi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vcrvsgeo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxolngi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdigvga.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nxjlewut.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2hasdukwv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dulsstos.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2zunwknnk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pdrdudsz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2zbxaglmb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hbueanoq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2umykgfrq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zeduyvka.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gqheaawp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ijjndbtq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2osxisiwq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oupvqdlp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bywysesd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjsjzewz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jyrrjaxe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oojntlzd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwhoiezk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gjoreyoo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tkdygrbm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nlkupghz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uyrhbvca.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkcuybl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2cefiscow.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uutyzvsm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xqjeiris.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlluenvk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gcmanvqa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jwlvkwej.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cgapkyai.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qllfesny.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wqgwcewl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bndvynkw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zifsarww.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tczumchf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2talbtcjl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tnzjyaab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2utibmguf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2szjdisra.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fuumwihl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vytwgbnu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vmxslyhc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lpzddzdq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bxmyhsbi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hmszukww.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdrqzaa.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tnbluwje.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2aefhiwvl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jevuphnl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qryujiqp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ftquwmdg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qahqmnee.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fhldcert.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wevrnptn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wdjzbgrj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2epcangnf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oybnonua.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nkagklts.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2glyogkek.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lnbkmxrs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2otonsufl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fpnowhkd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2jrkxmurg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ldaikyhs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2sbnxlcgd.html


<!-- 参考信息 -->