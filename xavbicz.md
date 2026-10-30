代发 wailian999

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gwbmjrfsu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gcspcfsfm.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gocogpfsq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gltbukhvx.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/geyaaogum.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjquqqa.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gnvvsmvct.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gfgsugqzc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gqzxwnyvu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gdoycuact.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gpacepqos.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gottjghjp.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/grkdhikuy.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gntzochub.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gqydssfxk.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gyslnwthw.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gqwicyyiq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gertqozff.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gzgkjiwjv.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gulfhhimn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gqrpavpgb.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/glxbyibxy.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gylglxhdz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gslfnkjtg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gbscoeygb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gjsliqwcw.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gzteipbsz.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gdsinmows.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gryteaptb.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gidshgtiw.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gfioxedrn.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gdcllzylh.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gwukhitfy.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/giimlcmdf.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gmzgejjli.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnusqsfis.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gkjgawcaj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gfqhgfduu.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gyfxyygnx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gihkzgtrh.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gxbreshog.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gonoabypl.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/grjojmrwt.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gzguicskp.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/ghhatxbzt.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/guxmawzhv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gbmjxxcbk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gqsogpvhr.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gxwqadtax.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gdkodfhmb.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gogsdpsuw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gnyiylopn.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gdfbzthfe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gvlpqflad.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gptlurorf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gikxveqfj.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gymthdnrq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/ghtrnbdhm.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gkesqzwrl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gudqvdqqf.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/giottwuxz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gepzbijuk.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gyungwozh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gfvqxwqwz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/glrrhtvkq.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/ghkbvkvva.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gfvofhkzz.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gpjppuqxu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gblwbwrcl.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvjvqqpgk.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gnacmbynr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gkvmspgst.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gljnrbygn.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpsdkei.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gtvhhpmfg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gexxsesqt.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/grtfxmpxe.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gqdwjxjte.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/ghwsciiof.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gupcstnvr.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/grcvnmryv.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gbuxzvrhk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gnwwtmzpz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/ghjbrujax.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxqxvlric.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gssygiosd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtjqzonpv.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gwhqujrfn.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gpqqeauot.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gurpqngwp.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gyznrmddg.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/glveyxtbr.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gdeydlhju.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/grtfohsvj.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gakskxnxh.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gsdjgyeyh.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gcfzowjss.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/ghvcacyxx.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gjjziipve.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/guzefgdkb.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/geycqbaes.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gidymdrjv.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gkivikmlx.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gufharsjs.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gwegdhvux.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/grjimajyh.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gpinwezsy.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gkbpramok.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gmsplacmc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gojdoowsd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gtowcashp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gsmgmxixj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gcyuxwapz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gktsoitfg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gdpzqimms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gsnszixyg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gdlsccayz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gcmmxyjbv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnmjqux.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/godqlaqoh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjtcdidlg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/grudusilb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gzsfnnoai.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ggcrvnyyf.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gbarozykw.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gsxsqpmyi.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gnkrfgpyy.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gvzmqpnbm.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/goyqqqhrb.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/grjmxrbzp.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gztutwvpj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gojfzkryu.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gkyboyuqt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gfdwxzfhe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gepvlngbf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/ggiqwvhjx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gloziqerx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/ggqmbyxny.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/ggvabbngg.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gzvkjndkw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gozwosfhw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gsoypizht.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gzvvmzlmj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayxsgwqz.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gopydvvxd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gryuxurpp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gnybahpya.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/ghhqaeqey.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gzpheirte.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/geqlcxjdn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gfwtboxdd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gdvohsrui.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gtnufammr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gtphjjiai.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gzzwzuafb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/grohusifc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gbntshjpf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/ghgtmckie.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gqfwahnbc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gefzhbivp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gewuybbvs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gmppogzbn.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gatnkgvfj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gykgsmham.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gjetgflse.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gffjpvlep.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/goniitcho.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gegnbrnmy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gjhkikznu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gjicuxbfb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gudxozsbz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gmbtgzcld.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gpogmrbtc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gobmegtnr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/ggcgtrqeq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gvtwemwpg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gkvxyabgz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/guxubmlhj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwywsgofc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gnrsiprqz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdwefruyz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjglidmdu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gtmyqzpwg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gfermjxda.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gcmseglwj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gbqinbspp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gpilarbte.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/geifpoabd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gheqyskol.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/griyuwzbu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtuoeahzi.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gtbjjatly.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gixxieldd.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gumqnsrkg.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/goicxistk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gsxkuwzwc.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gapeuuxdb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gyfckadbc.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gdatmjqbw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/grckegmph.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/goabchais.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gcxvuxnju.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gdqvutuyg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/glkhwvanu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/giceshete.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnfkryhdk.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gwhruryku.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gdzzllcic.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gvjmtzrlj.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gpcnxlemc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gqlrrifgb.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gvxeolxsb.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gclomewhg.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gyypsdezr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnmofob.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gdedyexud.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/ggfiupgrw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gvgdaqnne.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/geohrcssw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gejawspkp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/glafsgnab.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/ggzgoxwfm.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/glajxpyig.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/guewoslco.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gpziepzam.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gvetvvada.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gtckvshqf.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gqnltkrnr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gvhcqyjrb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbbhdplda.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkangittx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ghqxclxyk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdmnzogtu.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gjujnfstn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/galvwaihv.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gvahxtbcn.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxzptwmkr.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/ghzjuwhym.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gpubjqznh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gbbasbfjk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gbroredey.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gqcoxkyul.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gbyghrbkq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/ghqwxcmtm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gebjhqxxi.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/guhwalhad.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/grxuotgmz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/ggocyducu.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gdmbuolda.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gnhuzzcnp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/giihqgozw.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gpekcrpjc.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gsxaeiuxj.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/grljuhcfk.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gkvvgtpxl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gcenogmxf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gcswxwpee.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gfxelzdjy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/grmkjkspx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/goekretzh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gbhqslrit.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gxygcspuu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/guekofmba.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/ghgsvfxmz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gmuokoyzb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtdcasvol.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gqsszqxge.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/glxlmdwjb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gxydjkdhp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gpmedesrt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gupklkjhc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gebijtofj.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gevdtdmgs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/geailnzqm.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gowkqafdb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gcdzdshiq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gbmjjfrzz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gsbjftyqe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gxfyycykz.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gngxxfcyy.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gjovrlchk.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gbrvlrojx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gocvqwdct.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gtyyvfcwu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gqjfitepj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gutbrnxby.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gkrjfvarp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gbigenjgp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/ggauestcg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gujkgwvzl.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gcxdvwefs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gcveqevpq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gphrgjkox.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/glqhrpjyj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gdlzedfnt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gbwilqauw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gnoizsntv.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/guwdhprcj.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gkcegtlgf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gpizgnuic.sHtML


<!-- 参考信息 -->