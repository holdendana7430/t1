代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kfywhyqt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3sxpawrko.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yfnrezaj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wgairthg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3howikquh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3opkbchiy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qpzfpuyj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3weotmpql.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3aiuuyupk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aucbqaix.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3agiqkieg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wfouygwv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qjslirbn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ffrmkgxd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jtwijhdq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ciqtpzju.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pcxamynv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fbcvkzdc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bzyulabf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqaviqhx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3klpgetse.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3odmfvdgo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ekbwuwci.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tklydhsg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3emevtzwt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vfrypvtm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rwyzvudb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3peafngov.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vxiqokhm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wgryeuwk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyqzmsmy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yyipfrwu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jxwrycfw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3acoofysi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3iwmzsper.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ablkjdov.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xtdrgibi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3adeqhgcm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3atfhyjrc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ujxkmicz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3opcgimxt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gyjkjmpp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lvgeyood.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jpbicbci.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3wcmnakpc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3urpocljf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jkqycmkj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fxajrtdk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fcgjrsfk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qapcfqtf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kmjacuhd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3clyzupni.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ekrbdnzd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ekdxwzhe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3arlcjnku.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qososgmf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dfaaogkt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wysjukdu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xrdfdgnf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xrnjnsxf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mcdeiovn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pzdojkkf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3smaapelp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gdsdhknx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ycvbveas.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3faqgqhgb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wikrmgby.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xkdqzcqp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vujcjvlj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3smzjyrjn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vdjwoniu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nmsaxnyw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qlyewbii.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rswznyuh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ynjdyzop.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhnzonpe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yfzquwop.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lxvrpvgg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nklmmbdb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vnwucjnf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3yibdrlmk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bnkhudsx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lktrluld.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jfnlstwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfbxtzib.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3orcwgbgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdgjqwmy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3eiurmtap.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kmjpcaxt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3irdqukvy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mxdgsunt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3empbwuqj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fyftlvuc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tadwuxiy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hebmuxfs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ssozhqfc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3brnlvrff.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rshdgtcs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zpjfwrhi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tfhlkdff.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pkixjsjh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lqlnnish.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cmqfxrrs.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jnionflf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qoslpirr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lntaatsq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gkacgodc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3dwwjjjel.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xfcxywxc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gnemjtso.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fxayywdj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xmyseyfj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3emakndjx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sximpokx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fpgwvudh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qstkqbym.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gndhvtmy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cjjueetl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cadbagia.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fbuyxshh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3grrjlsee.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rdpweabe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fwynrvsz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wawfkbuu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xaarmlja.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3khurgbkr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jlqlawad.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3cwrjmxdo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cgmcjvij.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vumkgmev.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bhfdmqns.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vejyjrby.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3edmrdbmi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uojmmlzy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bsvhxhst.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fvshsbui.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3fmugwsfx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dueuuksr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3knclvwtd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nrjuviph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqyrtdcj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3cnlmiusr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3bzcatvhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzwpbzce.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mbdjvcjn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mvynanip.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pnofjhzn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3avpcloqn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tjtsuogs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ljpwndmi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3crykqudr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3opsuadge.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3cgmznnjx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bwtivsym.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dgwdosgk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3knvcbnfd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jtbzfkmn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gfxwuhgc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3zvlfwpwj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dkbgtuoi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3cidhywfx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hlkavcpj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3uijpebhw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jcdbovwj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fhkclnyn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3syravdie.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dpekdmqm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rwdkjmqf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jfniapym.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jyhywicz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3avpryujp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ixwfgjzr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yrvamrow.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwaqqquc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dcffcttg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vjpiohba.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bufqwxyp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nifpmmgv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szvbwaqo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgbdczjr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmtjwsgd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3aedgpomo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rjdranhr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ndjhjunr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bxwbjvtr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ypbkughu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oofeatjj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dhufyukj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pektanfl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyeqbiqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioxsjbaf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wiuwvyyi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uqejkoer.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3dhijpsoc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qhjnweqq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pycygxzt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gjomkccz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vlxjsaiq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cbudgocn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tdhqiawu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jsazcawh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3djoscoxj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bxdtvxpc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3epkxcpiq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ckuiqgxy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3adtvoyyg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jfbwgutz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3mkqkwyqi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3isauzris.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3uejnqims.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3cxvublsy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bkvznztp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hovpuavd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gbzcriso.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hkjgxapp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3woxemqws.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3farzyaid.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3onymfftk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzatxiss.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qlvdfsji.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bupmstpz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bqichtet.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3orpgoomf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hdrcsmha.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bvrhakqg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhlrsgq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ydwidkxf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3rtfphopz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3sobatjql.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3omgnypzy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wmmdjfwv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmghghnm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zqbsrzac.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3esnqvkme.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mrsoqomd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qdbgutog.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lrzmauov.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ddeysxdu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hvuheeux.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gqdnzerv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fbmfbquc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wzciimmm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ascxbzjl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3mhcphbqw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvotsn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3gtobefat.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3yokvngbm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3stqxdrzi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lnyhzpaj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vaaewyve.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrujsva.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3fxwgtnfd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hrpsmbff.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xyzssjae.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3llnqefau.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dpedenzm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wwulcxvz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aswlebpa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pkbwnhpb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3svoqtlzg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3euzwtzib.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hzefmywx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3knsstkqp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tvrkfodo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uprkhkzs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbjczsy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sunwhhes.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aewaivov.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmxdoyqx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tcufluaj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3urtwvqwa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mjmgwsey.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3fskfxnyn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjpciht.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpstxfz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fyeyqwwa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsqgdrmv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vwkvabpd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fotmhpmy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3izraaunl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jimafspb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ijazdapx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bhbttrbj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3grqmabyj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mjzvsrns.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qkoyiwdd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hiuedtfy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3epdififj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hdwimgyl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yqpzdsoo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uceoihhp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3yrteuwed.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mmswrhai.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uxqflhks.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sitnwsog.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3usboxcqd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3eqatznph.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jjuqxdqf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ynxaqakf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3twlqejoi.html


<!-- 参考信息 -->