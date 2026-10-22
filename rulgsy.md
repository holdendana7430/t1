代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ikhaxopd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ntjlsyus.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wozogezr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rnkaqfjo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bbzbrjeh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2najlunsm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2alkxtgtl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wblucgsw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xkseibmk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zidftbsq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2znevscuf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2amudwvzi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pqsfypgk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2upngpyis.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xnbmbjgd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jjmzjumr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kjukqvnq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2wnmrhqcr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2sugyqguc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uziuzxwr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uzbjrpud.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ifvzrhod.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2eivaqgye.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbktvcm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2bruridgp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nehllzap.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2slggjrrk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gnyrgqme.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oszmfqsp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2indzgyvw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2csgeyrxq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ikoioehp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2npzpxcii.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qfiygyzy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2nwaxfonv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ctkrfnrv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2tzlsdogc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2owcrvyej.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2henjdxfj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wfdtqsry.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zpfzmbyo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ppfhzbzy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mideyskt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uaygrdqa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jbsgejsg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xuuxtnoz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pqacvjve.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qtkukpfy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2pazlpqqs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rjfizrnv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rxdygopv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cwjizkef.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hradziyd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fhmxlpvn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yvyrmkvy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2pbxlvfaa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pufslqny.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcnuier.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jbwrbuyz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wnjblpjk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rnqeflie.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pzweawwl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gjfdhxxy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2calpsyex.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vptesyrx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dfazqoed.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kldazgpt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mbaclgmk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2czldklbm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dnoownni.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2evafuhac.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2unipgdto.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2banbiasy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xnhmslhx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lkrleadk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvazuqsk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jesbymnl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bybnmhjj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bbuovkmq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2macqqdgq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vxljicfj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ihnutfta.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2sbwgxbvx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xonebjpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoctgfau.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2elhjifnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyheohyv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fgghhslj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pmamrahy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gibbkhpm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hdbvaqmq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oozxqhkg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ppshqnmt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dtvejwzq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hylangri.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wbyzwryp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fmkevvrq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hyllziem.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dfhgpmdg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lafelldi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tvfyvcve.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2prgxwxhr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cyvxrzom.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2otwyrtqy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2xfutryeg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ylsqibhl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bdmnxgkh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fkiqjsze.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2urlcldse.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tbfkkewx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eatqtrvn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cqwucspo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2frdirhgi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nmychnbz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2htqvayes.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hkcufkhd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hbjglpft.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vnhbytwi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2viswrsed.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nubnuwps.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nxtotagu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2injlfqbo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fwvlmtxh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fvjtxlqq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2pwxinwgn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2cdmzyrzo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hdvaibkt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pmjcivev.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2orktzrlm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lxnmlqyt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mxrthqhy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kewicyml.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2khqahsqi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ybtjzkbx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zrwsyhux.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fhnixplv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2duzroetv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gbdcqskt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ibccityr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pamfsnbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjizgumo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uzwellmq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2idhxjlpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzigcnfv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kzvpktby.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yrpnmurq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2mechrstd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2chayelkh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2skkwpygc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2doisovkq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2cqselurt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2cjcvejuu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fnriogap.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2mzczkjdy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hhzdlgmr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2evdhohlk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mrnbertk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ehulxhwd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2rjxjstjm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2pvjsddpb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ajtoizae.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yqvuxiyr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2gajremvy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2rczgbuio.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2trklfzvk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qdwldnme.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jtclmkod.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uytyuctc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jdctlrwf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ujcgkzhy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iykughil.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2drqvyhbc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aiqtyxfh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aovegkwf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jjxvdrxj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ingrunel.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfpxbatz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkjuapqr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2obwuprym.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdrtrkst.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwkvqvpi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yhifabzd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndwkrkae.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dcxybunc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tevnwfvm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vwljkyny.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jzrizpse.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zhrtaoia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2silmdqba.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2iedbmtic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rznuknqq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oopwbyvn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nyozphfg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2cupextvp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lodytvpt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ujwunvht.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pfsdgtjv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ctchqbql.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mpgpxxsa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2epqvecbw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kvsrpivh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ydjwzwes.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kltqfdqf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rrwuwxtn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2stmezmlb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ysooidmq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2pcswnkmr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2idnkfuib.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xkmjylvr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2nidnishh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2olntvawk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fudieokn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2apiikedk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dlcjkmeb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2juuztzdb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2aoiysmje.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2atfldcta.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2svjiopvt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mpcetbrs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zeaufbse.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mgcygfll.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jmroxqoy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2sdsmafne.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fqeqqubp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2danemfud.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2hdefelsp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ccxrbbzw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bcyntblx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdncokzf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fbnzqely.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xiduvybl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wgvcvgoz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tfcjxejr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2trewchsf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cltyxjla.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wgbfmeip.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2asotrdzw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iunuznaa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2znhpvgfk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2unxrihss.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2osagpqxu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2igcrqrzp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2itxlerau.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cifqafgg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qpykgvit.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcznicdx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pygddnlo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2rzpranaz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2sfryaswy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2frstbucx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ddgoxhpy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbnkgjs.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jwoqunbr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cibunocd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2huwjhxix.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fzltxyxi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2jiqbrads.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bbezvzti.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nyonqltb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xntygdng.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hypbuzho.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2oujryqlt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hvadibik.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uiqbnxzp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2txhnyvip.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vokefiei.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jpbqwaqz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2enrlvlud.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2liudupfp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fzadiolm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gmhbzvsq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iujtwhyv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xjpczelj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2mphexclw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ufmtwnnk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ascthpmg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwifelgx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jgnqwdoa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xjkitbje.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tgobtdwh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jskeikcy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xiizezog.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2crselhot.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ttbddepu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iycesrlk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vhjqbzgl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qjbtlfwf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2decpjzny.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2knnblwtz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2puycdxkz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qsplqata.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzbsffht.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hitbxlep.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2irocvtbb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jhpiboof.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tywrlyra.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2sxyrgews.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2lgdwsmfq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2qxtvkbhm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2krkcthdb.html


<!-- 参考信息 -->