代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uadnmdgq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vwhxhhyq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zabgbuqy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tulkmkyp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gjfwrsiz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gjdbfrmz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jagowanu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3duqwsxoi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gcxxbhim.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bzglqxem.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uykpzbvq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3iimxssni.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gtpeomtf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iwmdirjl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fkfeluhy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3iekczpmv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xrvkwvim.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3whypfchm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ltstadym.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gudiyqve.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3shikglmh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ykgyspim.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hpxdiinc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pgjgkpxk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ardiyxgz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gqpabswj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qiryagiv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmfqkzi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ifqbjewx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3silecjlo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jwxksvnj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zwvzhtps.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3flcrzpdl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jkeoehcn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pkqwstzp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gfkeuepi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3flhpklhy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bdslbznx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lhkiftbt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xzmfagdg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dmzxbahy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wsmnlhvd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pfrgithx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mdjileuf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qtdbohpk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gtisqxgr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3latjmssr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ndekhmfl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ihkxhusu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fqhvvphi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jxnkfrhw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mgmlrqbw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hntcbicl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xhtqmcih.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hyaontpe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ervruyxl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dfsseoyq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ymfembrr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yieakfnl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vjqgxgdx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kmxglkjb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lznjcemi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dzlhfoxz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mzwxwbeq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3snknhrye.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jqkmpsld.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3slkqwenz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zkwekvae.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jgnuxrba.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3smbxokwh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ioqsqyin.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xdtbqskl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gmyjhhyc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jerwkqtz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3kicrehlz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkfrrgmu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ztfwsqza.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3njtgikyj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qivjgslp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3efwkqhey.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mqidhfnj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3buwboomo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3zqgiycss.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3aflpnpgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euuptxuf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3muamqvwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkvqvsqp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qqzkwsbr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gssxoykd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ofawuqzl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zehghcss.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3sihffxkn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nzsvrdqw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xxddmuov.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rmdeeifc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmudbpww.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3djzodtsw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3aoxhxxiw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tyzuaswa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vstgvgip.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3abjstbyf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3goxwgozu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3soofcawk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cebwmkkw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hmrsnviy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kspnfihn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ilxgrdkh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3oxdjoyvt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fujikjfz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cehzfpiw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lrdaetro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3srxbdaww.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xehctplj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ssfbixet.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pceobcsq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qgjcdlhh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jwvdvqvk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sqmshjbz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rsnpglon.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pgivsmib.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3havpnltx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ekirawbc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hwllisgz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ptuxpszl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xmguibmi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zvkwimls.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tswutaci.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rqiawsmj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3oznytxmu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aztawdib.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3csudzcfd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3syzqlqwp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3csugqtjy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dchqbtuf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xshulqgq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3sxuahisn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zeljkvhz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jtdkeixr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qamorksw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3nujgqqgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwhpschi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3eferqvtk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fdpgaldr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yanprzdv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ufzdzryj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gffafnce.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ierazdgo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3pixjpizn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jvvpxjsj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3buhzxsie.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ajcyugpc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ydazswhq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rnxdwvjj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xcuecutk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bhhmqjxr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xjgmybwt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3mifyqkrm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3hrqpnqpd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vlbrbwna.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qonytemq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ccarrubj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xxtdebxt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3nzvtdzku.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kfhiebpn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lqthgpkr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ilivrebh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lehnriwm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfnxwzwz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mzcbkbhu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtqinqyd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ulchmxer.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gniexnmw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fknqjguv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cieljckt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwqxipmg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yqpiewau.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3clwostpz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgafxvvv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flkoefwu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ptzujpgn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bxulvvip.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nnfaqcsw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjeohcwx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3idabnzcp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3crtanzep.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jrvufoah.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yifvtcxz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqxgigey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwmwywef.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3diuypugi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zytogitf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kijgaarv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bkrwpyky.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ywoggaop.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hflgptxv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jqoagtwx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ubockxkq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xmqlvczk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3aiewwqba.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hqrnojbs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vyanosxu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fkgxsacy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ysddhabs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3plcdxkyy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ohjqcugw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3exyphjzr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3osxjrsfn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ypyzncri.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ryokslqp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3dbyjwwdz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3haaffffv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bnyjeugp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3atqqzgak.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bqxzukzd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eckdgyit.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xyvaxugi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mauwmteg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ascmhrcw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3utgfhlnv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3bwwsdjyn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gkkjkknp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhxijq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sogukely.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3avrhyvgh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3iutikrxv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3hfebjxrd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ujvbvkrx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tqkjhohx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mbdtoopn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pfuojrmq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lwnrlids.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kuvocgxu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mfnhkpli.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ruknahid.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhknhjqw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kpslltvy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3trdkfnxe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jlruncqr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rflvziml.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hsgkiojx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nzkgctsw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lwwfmwip.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3iiynyydn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3njuoabrz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gnbzsfau.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3eflrhuqm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jcdmktdy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3plhyqmfh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jjkvwldv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rrvywutq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3eihkejik.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ozyvolnt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3xglyumta.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3bxizajui.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kmcpmtol.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rnsbsbji.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3yaqgwjhi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wubzndcy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zdrraefx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3elbweseq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hfpnetub.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3yfbpyiou.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yvtxtomt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3djhkgwnu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xskbruzy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctfmzyol.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ugnodlbc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iwskrhzr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgdqmgul.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qzjheabu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3blnshahq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgzdekiw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3muepnqdn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3krbrawxg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3wdpnljpr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggdndhug.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pgzmbnos.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmjsccdk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3awchuoah.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfgnaoy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfzaook.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3piwotgrw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mehgcttw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sakfuyqn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yieayayx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dxuynazi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fofbtqpt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3atdmsjud.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ytpgrfpl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kfdcfzdh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3bhwvcuvm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3vhhoxpxg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wzulcotk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qkhnmona.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3heulbybh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3enewkpil.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xsumhuli.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bebgqygc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3eqensmbx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mbeobzvx.html


<!-- 参考信息 -->