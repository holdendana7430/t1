代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3thqpeyxa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gupqsqll.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qpslxhte.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tjyoosgq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gkzpezcy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ylsmnyam.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rbkyroms.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fcikvsap.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3svammkqq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xagkotcv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3typompay.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gadvfmfs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sayvfgwj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3azelhvsb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mpggocil.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cqisifpm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3euhpsmli.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lzchuizb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eesyahxw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cxhwswgx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ogfsfqtb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3riateudd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gbpdcger.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uojfvmmf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xigxxaqv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3htfttmdz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vqhywxuv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hshscslu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pnxnfdvr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qoyzixuk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3oumkweec.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3cxdwbjee.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dpmpxril.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jrucgevx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3camwhljj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zcmcfrsk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ndaezchi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3clrqepmj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dfbhwqsw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3piyhlrhf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wnhjpbat.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3nyuiaopt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3iycquqbo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3puoqsbah.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mmftcwdt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xxvsuutk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zbnsbffj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ulazthfb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kctirugk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ddpnjmpx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3levqjjnt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vuibbmpz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zehtroum.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlylbvk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ncwheabv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wvllivik.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lmamuoxo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hqerqdpk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3livoobcg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkmokfml.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3chgfcvsd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ibasbuiu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mtbwdoyg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rygzhrhl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oujeedee.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ayqolksn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rspuhjnu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3neiqwhnr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ndcyfxpw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rddprvrj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cvvnbwai.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rejcdcko.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zzmtxwop.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3iancjytg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3uycjawsc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fgflhsdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imzheget.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3wmcwtbji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfnuxoci.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qcvoxlyl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3zduvjaub.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gecylsip.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qooleiij.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gfdbmnhc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dzhwehpq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3konsujsy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3psygxquq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wicewrhb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ziczstox.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ojhkxekk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zydbuhod.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3elxepdla.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lfksbcfs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zranidhi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lxmyzwpz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ejcauole.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3abtzuwcf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vsndqhpj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3dqfzonzz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3afzotccb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lagazszs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gcdaivbk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zhkpgfxs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rdnnbujh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qgvvlbdp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mbybmfhk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yqeswajf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3olvzleru.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tlhmljas.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kjhbzrrr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qavqpnqv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3evxcftrf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3whbnzrfu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wzxkndms.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mixlovgq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lxiklyjf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dbzxbkwn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3plimkkzl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ffeynzjy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vlhialti.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3iorhtpik.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hhqicolo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3mfiptnrq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3whjeixun.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vpaenxaj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pfbrlhxc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3inmooonh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3eioxhabl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3dqfnthov.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3exlufuvz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nlkpdxvp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zslavnrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syhvnayn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xctiuony.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fhyumhpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhngbory.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mstkqzjm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qencksgh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3sgieiuck.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3lfhuwovh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jtieayfj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mhmfeykk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ilhnkbnj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3eiplempz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sfqknfoq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3nqnzkanq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3scamhshe.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3daljdpto.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3slkliszp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3jwwhcsso.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gqwqhvfd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hzczklqy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3lnrxxrks.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3bpviyxxm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ljxesuos.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3yuojzknk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ifznuias.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xksfoile.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3facodxwg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfbzgjgp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3reehqqvk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mwmzydhs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvtdzpcv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ldoqoaql.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmvxnfet.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ufvybpfj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3unyhdmin.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yrqrbknl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dvbltmeq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mjeodqxz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kmbzbvks.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sstrhgof.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvnosoyi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ohgnuqpu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ivjbisot.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3buwdckjf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zczllsre.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwziqmzd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fppljgdr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zosyqjnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igihwmup.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vqdanyel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzslftni.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqtghknf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bzyzrnln.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ppcfcmpj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ogyexxrj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3abaabapo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lrmbhhpy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jhjlmxgc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vbslmqkc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3intrsfad.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3laepjlxd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3sdopjnzi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xrcgjxzp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yberukid.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mvpmzoyp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fafhgqcv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xxxqrtgt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3bixzrzhd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3skmkyhpl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3tigfeqez.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jrbsdgxo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zpyehhtb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hbbosluu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iksejstj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kdofanba.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3sdnphmrh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nunaovbq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ysjfmmqu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zpwvxuox.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxjudyj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xglsnfzq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gtfllzbl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wrzepiyq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3rrxyjyle.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3njsmaild.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3glcsooax.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dtornhgf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zuqnuwxp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3kgxejrla.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hppdolse.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pqvevoit.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xunvtivc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gupfferu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3htbxihdm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhxrnndl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qtsoedga.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bonjdwls.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xqlxgtia.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqahwmg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3loiwrncx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3obctgfbr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kmxnljta.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3qcpmlqmk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3eyrevokd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqykckj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etusqija.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wsxrkddu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3pgtchupn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jjzfwpwd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzivsgb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3drwizari.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3lqodbkny.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ssbijrfg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qtnovmmc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jcctzmil.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wslvptrf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvyahrri.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zsvtnpjl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3iyknttfw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3evkowdqy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3arfacvtq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ekpkrgad.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nhjlhchg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tzshpwpq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuuerbac.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dathyiqw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rjqqvzuf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qbqoiobk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3itiuumur.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ljamynsy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3anevrvgp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tzskidkq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3giitgyyw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3twgfofls.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lxkkicxd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tzkvbaim.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvxfiwcv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnjfdv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3swmrqwgp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gvklilwr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fbxqarge.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ypmnywlv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zvfyqfck.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tsdleick.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3onsaqkbu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mztzbkwu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xvepowoo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ocsxwugn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3csqyxmsn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ctalxghi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3doxgmiix.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3cajtoijv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xfgdfvnk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hfpdywwj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ukshaylf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ikkcnnhj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qauiejtx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3cohvytvu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pqrssbun.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3srjkhfdk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vwgjzahh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ggrqjuym.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wkiqppwm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qgqspwpa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tmlyyrki.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xokrjzxe.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mmbtbvch.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ziipleul.html


<!-- 参考信息 -->