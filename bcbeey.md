代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3psqvfibt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3aicydrgj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3azzdqftv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dfeyujlb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sfjmbyhb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pdrccuml.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jypexwwx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3joezyaoa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qwdnwuym.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yrwtrnfo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rbykhrsl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3igrfzaqr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tuwwezeg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ytmlibii.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mxtbntot.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uouqszqe.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ikssrczr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hqnvhdes.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3isnsktyf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ygrmlrpa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amuspvim.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xmsnjhtz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rbimeevt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3scfabxvi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aaabonhh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ramgatal.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uwtpjrcu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mradadym.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sqdxiorm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bteifner.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3oambxwum.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjawsdox.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3visamfxa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3drcgvjbe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rnwwcbwn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jrlrgcfj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tomxlucl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3iisfgtdx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kphjtcku.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qpxgpiev.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ocysywur.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zsiwgdwt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3iicxgghf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uxdghrir.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ixpkjtmq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3owrebzqc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rwaauwxc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3stqmeouq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qlxsjlrf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3atfybdmf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yluntmtm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ohffoyws.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lvodvpfq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3grzuhvzt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3evixlrxh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kkcqcmmo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rpyiwvec.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkzuxrb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tyzyhntq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3paygvsbx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ozdiwhkv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3znlicoyi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xuqlfuzi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ialekkpz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vgjqxoul.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3szbphyrk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cdnynyrg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dooilspa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3biyzffsp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tlcomhhv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3efaqdlou.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyulruoe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wjpkfbwh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gjtlvowx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xbgqaoru.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bqmnsjkw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jxmiecpz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wvnpdrht.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3xtluwclb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3eaotwjte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuswrpzp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3sfdvqyqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiszffrm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pdzoszzk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3klqwlkba.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3keznqzuo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ifqwmiqp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zlbzrckj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3myypwnbz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oxpythzv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xajsrbho.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3axpvoblq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nytqpzmm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wxwrgiht.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rmmcaoqn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gewgnicg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3aahcjbuq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pxmxrupa.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3aweftiix.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pjpkfvws.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3sodizhqo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gnietyno.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vfjxakva.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zbogulvy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gtxzwjiu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fcjgidjp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bcpluqsu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lpxgcxdk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mcenbmbu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fmhyqyyg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3toldhpms.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yvetfrjm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yxnbctyd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gnlocyrm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hlqwjzaz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3riwiubxx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jgqbnvcq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nndxjxtu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xicdfzxu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3edejjvzz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cwfzsdiq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3axqiezrx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uqnxdxll.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3cyqbnxdp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3iobzonsl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dachzcic.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jivpxpvg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3erofdihb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wrswcnzh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zxnwgtqb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ppqjxhki.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3nqspuaue.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tpkgynpq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3luqqhmii.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3srlihtiv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3igjkneub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krzmugel.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3neencjhe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qqjwfvhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guuveipb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wirmyzov.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lwicnxqi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qaihtkke.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3xerohanh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3sdehkweu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3yjalgwlt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3uwoswimx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nahvpmzw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3haaycawf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hykjsbdt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hricuxhi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gbhcgmsi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hfiopfjx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qknrqczo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jbncdmgw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3tecxltfr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3fbjbwrci.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dxmvfcus.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qunfpioa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3iycuazdx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mcljbkcd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3dcfdwfdh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jpnkhlep.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ppodjwls.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3inlkabnt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ueoidedq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pnluykyl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pnciyykz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrdzbsnq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3giahswts.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oxzytybd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnxsgzso.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3noupspqn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iqvsywxy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yeqdvlhv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjizfqod.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ujkxbwli.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3xdreszzl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qqxrovvn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itbrddwg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shtwbuay.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhxnoluk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3veswcczt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yfgeztwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aazumvmg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3siqyfwsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdwtsgsr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fedklexd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xlwjqwtd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mfnsyxdu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3clsoshno.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bqhnvjul.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aohcrpvb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3euyrxofh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bdhftxks.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cnkxplxh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jqgovgyv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kegpmjkp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zxotngfj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kpgcasmq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ndcvziyi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oyasjney.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3mtbwckqb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lyjbmwkt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fzylxbnh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3eprakbci.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3iytpdmbp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3npaadsox.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nnueriem.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mizhneef.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iibxhmcp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3boierhtu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xffplwpq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zetcmtvy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mjoayxni.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3esbfixtq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ekpukias.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kmvrtgyl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yztsjphi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vinkhcgx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mbakjlmp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3felxnjlz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ygdchvku.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tlqumlsm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xychdhgo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ybhabvcq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3labxkads.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yaeyflpq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fimzzsss.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3chmxznxs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sbdiuumq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nfokbrfh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jxefwqsc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gkrkeshk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yuedffzh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3znosinfy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3amhdlhdx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ggbfayco.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3pnfwbcwc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lmlxvawi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rarxpoah.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xfejjccg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3crwdffif.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ilkgalks.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xwnkeurj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kwlnbmjw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3idyndwxq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wezotpbt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3yoynqjjg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3vyguaxdv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uawgaszx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vevpaydq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfzvkmwp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ogymnbvp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3srxnffmn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uyxbbmst.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wmrpvznb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cudbyvwf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjmvvoq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aayfssrg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxlfqbc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xbwelant.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdthxudp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhetdpd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gitcplca.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lczuanxw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qyjqqnlf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iymnscgt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3snsvxywd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xlgntibo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dvsgdclr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3azrbmnbh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vtkchlnl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mnppfoni.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3uijjgdzr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3engdemag.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3chnmbeqo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3dkirhetj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xvolyude.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3esllrijz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ckfshwec.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rcdduyue.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rljsnqcv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3lavfnola.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ixoqnfmg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nphrjzrj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jblicfzx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bcakkttd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3frexhlfp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ycqxhvcu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qimfluzx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3sqdaudkv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3udlauxau.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3chakpdmq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3omvaehlu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ehenfchs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pyjscpnw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fdlnrcgi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3utjbuspm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3szkojupk.html


<!-- 参考信息 -->