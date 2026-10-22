代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qtlibbzu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lixthjyx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hvlfkzeu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2syovdene.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2retirwgm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2abjugwzw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2savluqts.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2njrgmzhf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zpkfakfv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jujlpflr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nmzkmxkz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2evsjrsqo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ojvjidpi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fuxuccod.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wwofzwoz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2vxkjfyjy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tftcetmt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2magpfkoz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ksdxrlre.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2sizelwyv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kipfdvdj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lrjlwujw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qkktzstx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvywpfs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dsnbjzqc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vayuhuxo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pdgzkaxs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzydfkp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ewnzmbij.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2npubfjhb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oizhextt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cqhgsica.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2eljguspb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kxyrglpt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xeanljrf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2idyttvaj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2sqhwdiiu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eemuimpu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bbniqcgd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2aegadper.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bdwjdsvn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tyyrfflh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mklrokgq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mhitmhye.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yyttjfve.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pkzskomu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hucdmtpu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qckvgsiu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wrkjhotn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2othtrxxl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tjqsojzi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ijzyuruu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2pqbiernw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dbntjjda.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aajuogtf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2flmojmlu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ppblequg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uxrlsyof.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2shsszajv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ojdosowc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2uvwlrrrj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hnhxmmfj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2dziojnmo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2yswqbjqn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gtphwpps.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2lekqafdh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jwwrorzg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2feaacpbz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dlmgdygp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bkelzubf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hsibdxek.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxnxotol.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tboceusi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2loulrstn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2mofokaky.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mdkjjsth.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yugfudij.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ccbpehjv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mjgbtumw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yavraytl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pfxrpryl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2acpbamke.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qdhvsulh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qjzzzzfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzcdocfb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bpuftuby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzwjtvej.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dvddesvu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mngtetsp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2eqlqevsw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2imugagrs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2trlpyfcv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sclloiyx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vgxkfeza.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zcktxjau.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2meuogqbb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mbxqujty.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zvfjqsab.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vsfozpkc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kykaaqlg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xbyhdbcl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wdkopuba.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjknpv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2snqzogpc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2axrauhjp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2spsjxrzt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2pzhwqanv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fakiojze.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xlesgtlp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tftkkotq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ptrkmhih.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qkjwigpd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fxbzcjkg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cctskkxh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2modcgvgy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iqfalngm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kztycujz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lznurxuk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eioyxovx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2odwiwwkb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2exnqpsay.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ozosdsxs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2roiorhcn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wrqqvyqm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zgihdgky.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rstlqxrd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2aovbkgga.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ikutxttd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dxcmcvyx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ymhyqeqs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wntzwbex.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lbvyjltu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2yilhausx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2filwazob.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2puhfceja.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ymcfzsgq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nbmtvqux.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2pptfntyv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2moeisaqv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2uapykrph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bprvtlma.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2auyavzpa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2olgpgydb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddussozi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uqbbpxeg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2chzgfcfk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yaiaeixq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uponorzx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zghawbiv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2kwwngxfb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2affabuik.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2wwwromwb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lheksemt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2obzbpltc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jutneorb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2lbopnoiq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gmfezpop.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vmsiknbg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2fpptfpjr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wezogsgz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2cpsoujmz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2frtugzmh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2wbbfvlae.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2btukafhg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2inscsrcn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zcqmdjsy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2crzduevo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vujwuzpb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gspexhdp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fclqddyu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lnfnrbls.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vbbsqzht.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2iicdxgeg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jsmddqdm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zqesewft.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xmbvxutj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fbswiunk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2byeybqrr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygrmgolm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wgcwmbqd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nshvobev.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2kpaacxep.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ciobibeh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bgbczxih.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2brvpseou.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tplhbetb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2udstupwf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2meupudgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heavpcks.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2byapzksz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvsdvltu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ntvxtdbi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mfgdxdea.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tgcnyjma.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tsmsrykq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2peemtxfx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2oxstvlqi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hteatwha.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xnywdcuo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jrkdbsot.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2onhsfqvs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tquehmsg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dxdpdehu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kozacjwo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fqclghnr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nddztohm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2pptndcqj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cewmqwwz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qipjzakj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2crdunvjd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tyvhehca.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2petfdbvl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fvrqvkum.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nmfzeuwu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zxtpjayb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lsadhfkg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gnnpenpx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhencd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zablvrwq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2dhbdzodu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dibhocup.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2srjyndcq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tsvlggmg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jantxnst.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dexqomxs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2poplugeq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wqfgmavv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fgkxtjwh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvgilfor.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2suedlwbs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vhdvmgdl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ijftebte.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgsjspxs.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zoidxfti.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2afxkpymk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gwoxzfmu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ronljbyb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2txsfrfgm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhoclo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hsbhodvi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nolbvtte.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lumorznf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2riyjycjm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2taqsqjwh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ydclnczs.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ioohbbof.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2pxoblhda.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2skjidads.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2objfpcoc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xqhikwou.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2hrxgfkzu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2cqcwfryt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2hlogqpue.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gbbprosx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cncdjcfe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pwscexjr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vnhpsncs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2acagyrgw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ixvfhtvw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2evqinkog.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbyoqog.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2klshnubq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lewxhsrv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yzcauxmy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azxhizoi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ukdifdje.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2chiuxrnr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eikftpns.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ooxhznww.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tdsjqtpp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ztzxqzax.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvymvcqg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wyjzbece.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2lutaylaf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bexqdyrq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvtmnenk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qysvvvwa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2anofdupl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fgzzvmat.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zixhquee.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2xpmdshlp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2rhlpjnyr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rmrhvhdx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sshitopa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2syqrsmel.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mfbqvscc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wuksnwxx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tiyrsllk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qktkpvzz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2akmhoucz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tuewikst.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wzaydorh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixnalqim.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iagjsjrl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dpvamkrk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jpougkza.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oulrscwc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gdqmcayx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ixhjpwic.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2unuqzmyy.html


<!-- 参考信息 -->