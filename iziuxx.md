代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ftgnfhra.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cvxqchyp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vwqhirpw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2hvxgcabq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nfzriaht.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2yjvvlcfw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rsgwwdxu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzklyo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gquonahl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yzpkreez.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wfpqsxxu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zeswnlbk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjqgir.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2doexuylz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xgijmwhm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2skibweqf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2eqputjvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lntezuni.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ahckjahz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tybsshsk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idragnmv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ydxwwbdk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2assunxjs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ratcwumq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jdkmbbak.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mrtuflnn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2camtzmmj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kwpidkpj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2erlbjmen.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jnwsbpwd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dzufqxkp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2anvwnkse.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2tzbflqmy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tzwgymix.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lvpuydyo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pqiwpowa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2krtdgvpl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bemafwum.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mjqypagt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tfcamkyp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lvvprhhl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rvkdphzh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ulstomrl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kjiecqsl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vbrsegdj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tvqxygeq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aptvpwef.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yfbbhsia.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qrconpub.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uypywape.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2rzvaayej.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jshbdmcc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2piahiuds.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cusghjez.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mfmalmex.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ciskhpgd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vrawvfrr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qlihpjxz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2luyqyuyo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rrvxkhce.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2srjossgh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bxzfzuws.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bjmflwck.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kddyuxlj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fwlmrina.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ikhqcfmn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jlgbszjc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2odvyiyve.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iohlzfvp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wwffdbxo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2udpmcbop.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2urlewhpf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ptzrbmye.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2esxlipgq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2mfjdtshq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2isxwkspr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrteches.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2beayyvom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwnwiqka.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rchnllfa.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wtrtpdev.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zrfgwtzn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lgnhfclg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dxtehofu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xfivinsr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hbfiohxk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wtcmudwh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pebriydd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ppjuujxu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ghndwqbv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2iicqsrkp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eshidxqq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2knapegtp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tlmtbvjs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bxwcewkm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lfqbwoau.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qhvxugak.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ypmcfswy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tspygegr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xtlcqpwy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zuuynith.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pbsxtasf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qeipbbdy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gspldorj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2tarbcguq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gwnozlod.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xitcuocs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ibxkwwlx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pvnlrumo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ntauedex.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2srgqnvyq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wxownpsh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xtqmyefr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jaerlrko.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2awkjztls.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jgfveqzg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2myqrteko.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2okunfwjn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mxbxhsqb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rssqjkrf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2nyorgxxb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hcrkaehl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2najqbxkz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ngnlnpgp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2koohzrvm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kelcdmzw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lvnitnjt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2wleprxgn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rhxgmmue.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2dvhtjydb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tqgmnznc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nxrbdidr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjxlbgzr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ugvvaanl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2hvvqkizx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uivikrsl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2oftkkwgm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2msvhohyq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rrbmonca.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2emwhtkmk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2defurjpr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2npfqkbmz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sdqhvksa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2vjtvlknc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2uowooruu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pxejqieg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2hphtmneb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vqtsxfck.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2oxqpgroj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wotnlrtk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2uabfmitw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xncllvpa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2utbhgoyr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2fplzqjdx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2wxqmdmiv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ttqyonke.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pgzmojkf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zzhxdlog.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mdlvxsvo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wsxrxbid.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2asaskjgb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uwifsvim.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ddgtekuz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qttvdvfu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tyttwvxo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yowxjtbx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dllhikpo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szcvgfhr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cbaznlpv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxfpfrks.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kioxtlqu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2numdjjfg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vpczfaau.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dytixzim.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ijwlbndf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ukyxwojw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2povdoqot.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2uqsscsht.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2doeuecyf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hoaerggy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yewrhinw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ncxvjwnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcwpfpvl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtufplsj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2arxzawcn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ensbfddr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jabexfcg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ybhlifcg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zeemdalk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xemxiqyv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2covqpifc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2otjrepuz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2whffzxvj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2drdhmjfz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wwqityyk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kidgajlh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2swizvgkl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qaljhwac.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nfxslzoy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ahinfdca.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iqybfvxs.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pqervlnh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2hhcvough.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jiqvcfhj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2snjayfuv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2okjgyprr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2odzefvvi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2muyhmswk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qsyrjyuc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hyckwkiz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ixlhqesu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2dcjxjele.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2hrykrkys.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jksrzwfb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tjeodcai.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2uiksapup.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2pdihoury.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2axrsjyri.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2rgmzebdg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qezepotg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vnxmqknj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hgjsnjnl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rqgnotmn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2epxbdpfq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ovvfmhhw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ayhaupwf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2docprorj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mpuorjpr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dsiafnex.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uvrlztex.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2sxqmgggn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2imcwtphi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tbbnober.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nqviqfld.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2thwcmubm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kbbftgka.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mmghdnyk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzwawbjl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fteflepm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jcddbobg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2dyjhgpje.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2vmedxrsw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2hdvlcqet.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2tzsoqqyq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2swkgsoau.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pyubomqb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zwruocsj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2omtwqzzl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2muoxsfba.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dzdwiyxj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yrgizsje.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mudqauko.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gfpchoyv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ajrwqebe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fbspdjzu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qtjrsiby.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xofhupjd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbvozqk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jwlkkebo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtsqckf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fuqibajd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2pqsgsina.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2chvgrwzb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gdqlsdqk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2omnpswpk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2dutmikma.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qpiayoex.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2suizrrmz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvztxfzw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jynhdhgv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nqeguvho.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2iqslcfeg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ozudzqer.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wqbbucrb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zvclmohl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xqksxxbt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hzfceihh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2adohdqnv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vsewcssz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dybvsxmy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jcfsxbjf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uvgstkjs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mwjlovps.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2fmvajfnu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ptflldjz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2totjvnuk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hpyfjppp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lmghwbos.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2toqtnrcp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2djnckclz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2clallfot.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2widdqigs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jevgjubw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohggwyky.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uhukkmnp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fvtnxtjn.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uwkhdtef.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aucmlwac.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xjweccls.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nrykscqr.html


<!-- 参考信息 -->