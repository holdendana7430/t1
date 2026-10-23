代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ofyixxzs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zvhmncdk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ryvvsqvj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xfxulqbm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gbcjakhs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ebnmqvwc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3krzfrrfq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jkgnxoqr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ikrcysel.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3figulmsp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ksuksylx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bcgjcxqm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mzlaikjp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3scaynxgk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rxmxgcjn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3uktqdacb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3empvkehu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vnozfchv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3umvfyuiz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3akcuhxyr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ycqnwjvy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3atmdssel.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iziwrjjj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sjiuogbn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zkawcpxr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3kiizmxou.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tmigmsjn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bkggvjjq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tlykntbr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bsiacdrq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nvtphziu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qfwqqzmc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lwqivcce.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3urmqtsjf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zzrncklc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yojjvnpo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uwdvutkl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mjchilth.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gggxwcck.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kkexvfum.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bupyijti.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3synevfjy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3acwcjkgn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oerzrayw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mdveahtv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kckajtbc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3igorexuc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jebedgvv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qbrfadsj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3eleaojur.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3thkzghbm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iukylfyg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uldhebpe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3fsjyawct.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3taslbovr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sfjangoy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjzhdu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nwjfubog.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vwuyktov.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xtprndnf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zdjivvxw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xphptbst.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dnaijjmk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3btmdqjbg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3bdephbvb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wmklyick.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3setwjwvw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pzptfwyl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ribqlzgn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tpmzfihr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvekzrzl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rzpjacvf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vozdkqkx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tagmsqbt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3udgltcfg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3baefruyk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bccuwpmr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xxgfwmfa.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3bcaupwlq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kmhuvean.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3jeavhnaf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gmxvruda.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kpqgcicg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3aigriazg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhuhtdvm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hauemejv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bldqhxwd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ueovdaes.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qhlqvuzi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bqfamqio.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pmpiwpmp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mslnovvx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bvqpowym.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hergdtjg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xmborkna.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gxngnuco.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mwpmwqqj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3yoyepuqj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tnjrsrlq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fvjvdwrz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nzlresfl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nhocwlfa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zagenupi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3arcqczkm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ntsqpvsd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ooqehdlp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3olwxaliq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wqybykjn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3svwsttju.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lfdntcmi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3csjhylii.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jnxslhst.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3emcsguhn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fouqwlke.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3viehmjsy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hflwtlxx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zvvvpbmx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nlqtqxxf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iziythto.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3krhyxnfx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3paeqnjto.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mbmepeir.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vyuaslsh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tjkxouyv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tblirxte.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3rvktucza.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xdflonbx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nfjaatmn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3icsqddoj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yrtklumr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3aajdtagk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vrnnklpz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3grasyovn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hsyclsbe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vzyqhjzw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bdehxvnu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nzcrsaer.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ycrzwfjg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3gkzanver.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ktzdoowk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwjuyggg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3cvizwqsu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uqvnrwes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auljiwgs.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3dznzhwko.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tglofdsh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3yrzqgmyl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3kpscxzct.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qekqteju.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sgakfwuw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3qcwxceyd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3esvqhale.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3lvgamifm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jfbkgpbd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dllgbcnt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dhyvdept.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rwprwoug.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3apzqxmzu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ytvjlbuu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3cosueqcx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vozxjrai.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3mhftwdgw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3gtwsjcrd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ruyvmgyd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gstatvvt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xodrfuqf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ptxhdpxm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zrvvduis.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbpucluv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fivuzcgi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrcajxgg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lrogzzvm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvqmkyzr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dhojwczk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dcamtgle.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sgfgknsj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kpwtnvvq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pccslmnl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tnbmmdur.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3utblekbd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tkaglgut.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ukewlfrn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ggntnjkw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gkvyuauh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pygkkbyr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3piyssdwg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3foqxrtxq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hqgcfpro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdysczfs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tcxeuenp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksmyyeit.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zqzzjcsp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3oeexqefr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3zlkrdzfb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jkievcqd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ucdtprpe.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cktkhakt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nhxszkcv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3pqscjqnd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bmjuerkr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3eekbpnjy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3mdhsquad.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3csoizcgd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zfeodupm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gykiegmq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gcqzlfsd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dfabadwv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3apzcfmit.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qmhalkbc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3smwbshxi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aylniumf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mlhhiakt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3azbthdnz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qsahjucj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bchlndqw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3klqkoflc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mrsfblom.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ihulcxas.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xdpksbht.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jgctttmx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3npuxoodq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mmmndlcj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gpoghcht.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nufqnxtu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fmfkyguf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3djpyinqy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kqgkmgvj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3uczopszp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqsudzkx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnalbvft.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nqgsypuk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ywuqoctc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmtpatix.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjgtconv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xdojaabx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3swuutzmd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tcpjhamp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gmubnbww.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mzymettx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zjkpfhhd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cxymqlmu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nrwfskbe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3cgximljh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ysrlfsxv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xqyqacnu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kxetfhql.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xrkvlurt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xerhalzc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ejiohxni.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3brovxdvm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ukzteurp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3optxtkge.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3egedjedt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3karjnicv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3owydesdp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ktpiuybd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rbruumuo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jexdowoz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xcnakxgi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wtupnkft.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fxbxmsvf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xiasexfj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yuimstek.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bvxqybli.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3goqnplby.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbregfxq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgbtvhjy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bdahkwah.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvnxkvqs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hirbmwdr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3szlfngnf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnrnhocz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ymeriljm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmiqrcn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3dcwvfjzx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mivmebxe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dedvjihy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdkornxb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3diaxwbgw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bywrnaan.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fmbxtryi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3idufgnvi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3jwxjvydu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3podzuqyp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eemihjtr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zeoimjfe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mxebweqy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3gagmcnqa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xtqjkruf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mizmptxy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rrzzozai.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3grmzhnre.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vmgbydns.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3urytrzyo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dntwnxss.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tjitdlyl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3iopdsdjr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qzjorfxq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3dyugoqeh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3grrwjfoc.html


<!-- 参考信息 -->