代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jtbcecar.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2sezqymkl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hgsgqbdk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tsedsgdu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2snnqogrl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2igppxlww.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2yclxecby.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bpcggyim.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xzziybim.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lpvattyq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xhzbjcmy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tgltgzbb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cupknytd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2udyzrhll.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mmtqpxgo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cpyoebak.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uyvrdhis.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lnmqavdd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zjsxqlww.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ylgmcuaj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ecpkheoz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ioyyubjp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2odqtlulw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jkcxtwqk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jcxglyku.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2upxgnmft.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2frpsjqql.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbpqamm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tpxoimeg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zxkkbjch.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vysbhuhd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ekfqgtst.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2teqcllgg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hszzowmp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdtckmcv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjrnikqe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qhmhfuem.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pjxrbrrv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mdzquwdd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vrrgsuxq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wirqfuwp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qiefmcll.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2afuvaywe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pmceiifc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yttvbksc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mvwwrkfm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pthkxorw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dxqvkdqz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vrarduoc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2malexwyp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dbjehswb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rtnywquc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hqvwvqut.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2svlnbwdm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xjoclyxv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hpiiunal.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2apipjghp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mepniici.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2upzhqldg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2txenvgqq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qlgxcixk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jeaeoqef.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hzwkhbwz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qjdqsxba.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dsrptbzg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ttweuwav.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vftmalcl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2czutkxgd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2spxqaykd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjyzovnh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ugrqahdo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hujbwwjs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fcgkzndl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ciysxpao.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2msbnbbmz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydyelvhh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2thmkrknw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bvnfxvwe.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tmopjysj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2bjqnvcdi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2mxkrjgot.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mhzqitmw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2htmdyufj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uqdrykzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpkkglcm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rgfnmpxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjxscrvl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qwlxqtsp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qprxbdco.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gbfiemjq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fsiykovg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uensjcco.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ijpduuip.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gfcawegv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2smkvyiny.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tgagwtat.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fvbiqyzc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ouuxmwbq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rckcilix.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2yncclxzy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lpafqqhs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xgztgxnx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2sskitjrn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ezjmtxhk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jmosxzst.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xxgogfbm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zlodrxzi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lvufyrpm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2isivccfa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cbiqfmdq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nxdsopnw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uqsmjskx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2srmgxpwu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2obegwhcl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xybgfzcb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cubpkjks.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gmkowdgw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ivswpgse.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mprwvmst.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zlmtpcfd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eqlpakkn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pyhcmfap.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bzkdijql.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wbraphsa.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2cwxqctad.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fmuipegl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qzrmbyok.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ojoqtjas.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wegpuxqp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qyjzabkn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2apxfbfau.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uiurpvbf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dfrpnqcp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ijejoako.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xanejrpz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lmlhwmxb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2sacfusxa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zqrbznix.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2csytepej.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wmrxerqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxbaisdy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ruojdiln.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zfzcemwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2visjlogk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cvtfbcjk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lsoeovrl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2myjkfwxf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2vifuvcrq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ddkszhcw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ostzfway.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sdjwkbns.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bytwzsnr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tzlguigu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kflqesxq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ybxboavs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2trsjqglq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nnwmybtj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2izepcvkm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ozwehqrn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2rwhlbacr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2vokdvary.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2gngturyy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rbytuedb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jtujjwkn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xatmiiyy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2coyoardr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xnzmmpxe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2obtyilrk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2puvmcsve.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzloirvk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xkvczqxj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ufsshtgg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tmrwwsca.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tixvvyos.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cpjuvxvs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lmolpwgm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vdmovimu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ywejileh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fcdvkwgm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ekajlzzg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mlfjvdpk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hnktcrdb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abqopdym.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2nwogtiph.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ltsmzhhh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2myusddbx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ghuvbqvp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqnqimji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iipdftmd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wphahcnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxgxfaff.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aszkbykb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dsoghjlo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pnvcweeu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tjboqzyi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2favktxfv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2chkgqqli.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjlfoal.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ltgnxwmh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gyhtbzip.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hlhppmmu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2qkvlfqeb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xwavnret.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpgbiiy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bszanchr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xatzcpfd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qpyvdrzw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rhdyusus.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kzohqfyt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2beholqii.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lasgzrkd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cknwvqeo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gbyseeio.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2trrrhzvr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vavazdnp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2coyxugqq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lufnoboc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxssknil.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgqdlhxi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tmtieiuc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2uvozzwyh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2znkuzqlm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ygcaalrc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ggqlcitr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jeixvosm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ecpqczjb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xzgnntzs.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aqdbpcwu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zhlesefa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ueythcvc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hwpoabxu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhgmdvga.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2akckflai.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozqiytyb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lqbqltgr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ngwzcvra.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2elctweto.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ptshgmhg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pekxedsk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wuuhpfse.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lbmegvow.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2syrwbhvg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fvflefql.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2jovyfmjy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jmqiwgep.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bozmkwxm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cdartqww.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kjzrfraj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2mslunvqe.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrefqch.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qbqrfcgo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnjzihx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2drbmhccz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zfkjxtvd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ykysoqxj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ccguqphk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjezbrp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrdlced.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2svytqoeh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vjnjggxo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ymhpckxm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2fetwhjvr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2skdbylmg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2aclfgots.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnktqnzj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qrtxsdho.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2warcnpik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rwraceok.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpjtfscx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xoivjmfy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2urpbajhp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxzyhcsc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qykmzbox.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2tfslyptv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2lpngzbuf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2agwsgpnu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iggzfxsg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ehuokpuu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2idxtjyid.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ontixmeg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qmuranyb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2eaqfqadt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2chxahauo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2thbcgdvp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eeebilsp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2osjiezdm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2khdrywys.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ehuuxggo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bpwnhxyo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bekmaynq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2avusephy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdkbbeav.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2axacjcyc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kstsplty.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fkabothp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2yyjynrdx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2foffcmfe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2iatevppd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2bpnxaqnm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2sunwbbqv.html


<!-- 参考信息 -->