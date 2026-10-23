代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wwynxwmz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fkaqkask.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3huzfnagi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vkuezjfx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zhkojxey.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rzyiueov.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwiojm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xhjarivr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ukgsittd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qhtwmbwf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ywgkbbbp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ittkrpqw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3unbsleqy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mfozqvji.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oxoulpav.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3izapmnai.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3svemluvi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dkffcxkv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lycpzqel.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ucxhbqco.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3glujcowl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3aetlxabt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cvujqzwi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3iexvjuid.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qgnpzygh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bbypmksj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3txqzulrf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfanyjwb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fcdpoluy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3kulqxhxj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ptyuohuu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mxjpcxkm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nspzithk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3uxdckaki.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nozyddwh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aqsuvhzc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hvnqwvgv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hnfyxguc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hccvkixd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lddfqdxs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3okuiffye.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pciuxucf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3uaatxkkd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rtvbbgde.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3omsjgtgz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kvevdzlw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ezhyaxcg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xarlzpff.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zvgdlpon.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pupjffil.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zpkwqalr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fcifjltd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ehixuuss.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dscjfpau.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pgsffwem.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3szuphygz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3voocponc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3inspwdky.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bmrnlnqa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mekeqmas.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ftbcdcgd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nkyhkmlb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3tojkkxge.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3grtwbqvd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rgyjekaq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pqsivcjj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tksyiypj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gfumdnpp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3azzwiwqz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xoxikvyg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gossrvag.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oroxnsrl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3fvezewlr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pazxfydz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3urnvlcar.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lslmyuwq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rtporvud.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kehzcuqq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qqumlfbp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jpxdtczo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pgcovxbo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ddjwsaxm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pqbxqfil.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vdpicodm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3whflxxqu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mdydfgue.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3inwylnqn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vvbsrdcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brbpbnqa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nkwjgfjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asftgxiy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zmyeptsa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3pdlzsxwr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3noyztrdz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wyjhlleu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rnpricog.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ggbftkuf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3krotpmxb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3glyqewvo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vykybafj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3efscrpbo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vgmlprkn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vqkowevz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tgupwdza.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nvayluxn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3smfxqmuw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ucitazdz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3auxtcsuq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bipvaqrp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fgldaqrp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wbeetkqy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qjipgptw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3acdkfygq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3njeyaozy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hzcufqfy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yrtuuvgj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pnwffrow.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ogelttbq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3drgollsw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sczfttcw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vvozfqzq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nlwzrevi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lzittnmm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3muclraxp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mtynmldh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3svmtlpwm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3iiutyfan.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oifhhqaz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3mcgstpom.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pployigh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3hzywkpmc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nkvgmbny.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3uvazmwkj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kyymraye.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bhwcgcge.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mcirmuav.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3orehjebu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mwcyzxtg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fspgpkjh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3uagrgjvb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hffnkxej.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3npyrkdmg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wouggjnd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3loiuznwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lduntizh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mnrxuqgf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zfpjaxse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3estnesja.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ljhnhpcg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vdocunsb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xtzvrlln.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bdcgqixl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mtiujwei.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3rgntntsk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pjwmxiks.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dcffrorl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3oqgzfjrb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cvziikum.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3eiwfqrvr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vmlrcxfg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ilgzwgtx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tvcmzwrr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vvuotknc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zlyjaayy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hfqrelnb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3odbtdclp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3rbywsnun.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dwiglvfd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yafnhxmm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3dfliscaa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cbsudilc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3eidntfiu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wpjbpthf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jtrhbsot.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3prditoub.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zregbgvq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ugaxpgvj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olaycwqr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ivnrgwiy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wgfyyjiw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3acoxryig.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xkjjqumn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvimkqhz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uwennjar.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmxevkcb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3cnbverqh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3boxbhefa.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kokppsps.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ktcahica.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilklhhkd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qnuhjxma.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iggfkjfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijqmymbz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3adksgwuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lihnvtek.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3whjhnkfc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qhbgygvz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3azqclfgb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ssvpgqpe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3gprjbhim.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ofpanpel.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xaqkondu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3lflpthaq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bszyfekh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3nyvaaxol.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fanalfse.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ftlehlcy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kygtqlzf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ckuzjpok.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3utrfeaim.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3twsbzhcq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3gtigdhob.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xzvlmgbq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pqgbblif.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ehylkzfm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fatmflef.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lcajvacv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3abnnjmnb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hepotxee.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yxuryanr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jsnarzwi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jaerqbvw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3enlylhfq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3pabxkszy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpefcnm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dlptczvk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3aoufozfd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3pplboplk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lvoizimw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtikxip.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3fbnuqgio.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3chrixouv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3iftsldgb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uswxedru.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdwpeucs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ywjvxdxf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tapdnetv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ecldrbqx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qbtgiuew.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ilplcuwr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dyjgrrem.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vblobtvu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wqguflhr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3faavqhyp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qhcuycbk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hhpffasb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqmreig.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3alshkdtq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pxcayakr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbjpmflo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mfdxdxpe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vekudzec.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3uasyquvb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ndldiwtk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3gcaxspsr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qvsfkfmk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3wagpdwtt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dmivpbyp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3zlisgqyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lhbjsodb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmmobim.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhthrvv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3azoqnsxh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3thaaaesu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ilffuumr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3mwjhtvvf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tluttnon.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ssxdcbeg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eqndxxxv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pblthqib.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssdatjep.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wsltiwdi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpzemid.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hmtfxpce.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3tanlqmxm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zorpzmdd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3iemsqyha.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gcafgxpr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3snfvpeqj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vjbuelze.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ogijwkkc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3upsdjcps.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fgdgxbvt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3wvqklvwm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3majrpcak.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ascwsqye.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dxjwcycy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xmjjwofr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kpkgvanr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qapylxle.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yaudulcd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3khxceksq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3isupdzqx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nuwrusjn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jhdywdrq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zplcdmyg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zeecsxjl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3idaecytk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ctgqlhiz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzillnn.html


<!-- 参考信息 -->