代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3htssjvuw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oecatnxz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fcxvkfte.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ixzejnbd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qqxupxyn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nwekfagf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wehqscpc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3iszvdyed.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jhuyvwlo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cdrlbxjh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bcyzijyt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cdffbxtf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dlahfazi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3lvkrvcum.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vzpkwhki.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3tikoxkkl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jhhohtig.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3bmhmnyhc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cedlqjrg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgwgnfk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nvdoegwf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gsrawdgd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rklyelcw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3logvcbpd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kuracdje.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qgxthhlf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bccoxinj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfynhbif.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3devsyatk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gwflzljt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkzjdnyw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pityynyt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pojdjdjg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qyokhmcc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3omfambjx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ayvpltbp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3fogngheb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vkiukuoj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xjbdozzb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uiaqejwm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kzyqvfgn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cbjaqsqm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3aynjixcl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hosresck.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ohohbxub.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hnziuric.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3cwkppuhf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3irxmheer.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3sadsvhkf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwdqpfq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cecegmmh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3onrkeagw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3aydmrsnh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rknbhnbe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3siuzgjiz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lbqfemvg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ozfxuigp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrapcce.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kdizbswb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jvwhshin.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dovtthff.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dhtyxsze.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zhzprfbg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nzhbjcrs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lfiwyvzt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hufokqxc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hzhoylki.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wybqbjsu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jgbzdzsl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rlligwkn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3grlzpunm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ducyogig.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vcgrjmkj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yrbinhvk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tmfkfemz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kkuroklm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dhbziwxo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ofqbxxik.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ifaidyaq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kpkumhyt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3obygouad.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ksjggvsy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3byohykdd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xbadjoga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3piqzonja.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3reulklkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpzpcsxp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gxzlygge.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3phqkxeww.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3avqevnne.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jdrkelnd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3clxvyhzy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3waeaygbu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vdkrfofj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sjnztxce.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cpeiqnuw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ehathzfx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gstlzyot.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3flkvvykw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3fatqpqaa.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3shiqmpje.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qiyfxixc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3fiznpnnu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wzkuzqex.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3frefqdwx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cokhcgjh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ggqqvglm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hckzifil.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pcrjebpa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nrskessi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3duyfjbec.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tnnmionu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kcenkiao.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3whkpfmle.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ycmtxuqr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vllqfddh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kygqttmk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3foqecdym.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3muwoyimj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qcvvaxnj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rlcsucrn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3cdpipsdh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gmlvjsig.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxqwmcua.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3waslpbcs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3flkelrtu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qdtymrik.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3galrhsnm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ottjonfe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3knjuvrxp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xgpnpffu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fmltxggc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lqtmutnp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3llfjjhif.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3pwtchzjs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rftvrzyp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3coxhuova.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bbszwcbc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tpergxyl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3pcoiijbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohnfhhfu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3pmkkmwpz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3khkxcnqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwgwpdoa.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lvzxyjxd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xgciyxzw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3annbafed.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3onxjazol.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3igmbojhy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3arezfbbq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3oiluirkf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3oerzcsss.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3djkwqcbu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3aunfaazf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vtsfrhni.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lpyszafd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hosjrmla.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3eafejqjh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rvuzfgin.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zrpwwivm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ysnnlbce.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3gnmqbsqc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ivmuemcv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3xeefxnne.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3djqlspss.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3fazmifqw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3msqrvdji.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fkkqakhz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqphbemi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvvjsfvj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mcxhqzvo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mxxdifuc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajtdxidd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3leclsgno.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3abfvsdaf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3plrofjta.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iymvernz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvkownbv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ltkxvyfk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uixcjirh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mdhungfr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gotzcndf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wvusjwjr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qgtxnjgs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tywbytcb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrdyoelj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rkgtqwgm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ouzplitj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wamynjtc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kbwjnxzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vngstxxj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3kljtpykq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxzfmtw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3sgvzjefv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3khcougme.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3btzmlnur.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3phddzpjx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3euifkssr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3euxjjbxp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nnohmdgs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mfhejvvj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ilajeoom.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ucydvshr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pnkorfsq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ialgvwdd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jpldyigr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zdvcrvuc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vcdqajna.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wlyelfko.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3uujqfxgi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dzhbmnbl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hkbdffqb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xkstynip.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pfkwubeq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ropoxsqj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wsjqodfq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dhstwicf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3axxehjob.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3oswvbdpa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3myfzyvyn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkszrqan.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xpdocpmt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jctpejwt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3fnxsabqm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3txmheumn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bhipvfeq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ttpauzmt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qjkxrbxa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhidpbum.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jqcpiikj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ismtdysa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lznfmqxv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fnjuhepl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ymyrjdwl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rbghxuum.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jcmafxac.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jqufpqzy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3stjdhnsz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wjqlfosu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3toknijoe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vjtlxlpj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gwcoxwro.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jyebrowz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zmlviaih.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lzfqyncu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elukmkso.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wthmrahp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbanrqz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jqskycbz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ejderhyl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vqwrgryp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3piweaonc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3thzoupsc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3huiyboet.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3udqgoodv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3seafavtl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtsysyf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fnowpefu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3oisiqovk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vaokexat.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ajfoxxde.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vqkcqmws.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xmtydqsf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uquutahv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lvwsfkfa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jarzdros.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwprjkkg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ziuallfh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ropgadev.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3pkgugvnb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3firxgnnz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3edieovol.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wruhtokh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3pogmwbyx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vywhujde.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vgpzvpjx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tjuujvhi.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ppohxtux.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ebeoawjy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3geecjvyl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3indiaqwn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ktylntyx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zwctqtxt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sfoqionf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lraeccrc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ltybvtri.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kdrbufst.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nonhsftk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yhifnzex.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kqmsheil.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ayflvbmv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3gogdmrpp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ugepvbfu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rqoioary.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rbyhjpyq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3zxgtuovk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wkxlnelz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3xhbftocu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3eoisfvqz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ixysnjmd.html


<!-- 参考信息 -->