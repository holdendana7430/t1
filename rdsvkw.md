代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ppyujbgq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2aokbvzfb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2itsudfpm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqjrzj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ursvbvar.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qvepexas.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2goeearec.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cyllnbdy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rbpisvqd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lhazfxdg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lesgkekg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2iufhuaku.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uegwlbce.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xbqxizmp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gohcfhoq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2afvltrnn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fgxjvbul.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2frlnytlj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nqorslqv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2kwkyfshw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qnejibjd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2newaikab.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2zmhiarkt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlynommf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vnltgric.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sxzagmtn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rgqlrynj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxeezjqu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2firaxpyo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ghdobwra.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tpabpkot.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tzljdtas.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2robqjcex.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nkglsydg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sglkyjzk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybjmyeyq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lwmztiul.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xymmmbug.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cgzcxkjn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2weqjfuho.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qgwdwezk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jxciwduc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lhqpwbzj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jurihaqs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kxcuwwvn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2igjruurm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vxpjhree.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vkqycnvs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wndsinbf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2evjyqqfy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bjpmjrjx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yissrevp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mahigtms.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2evxewzdm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cfepjgfo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nlsceeok.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dlqaixlq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqpkqzd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vcrtflrq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2updfsiwb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vlektzso.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iybzdnjg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tjcqazdl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mfnayknp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jtcchjkl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cbfhdcnn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qihhbmlr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2poilruiv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rbdzvvrx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nxnarajl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lnxyiggf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wymichkc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2emubpaka.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qayqdbeo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lylzfude.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpqyszlq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2srvfjynb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2uriujqpi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ogylvcwf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2zrhizwpg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ysznbahq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bavcmvqh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nonuxltx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2cgldrbwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzykpnaf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kyficfes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plsgdmyl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yizehvuo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wheolkin.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ubiqqytu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2anzssjjl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hldvggoi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pgvcnibq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2evcctuaa.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nvfozecn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ckcscnpi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wqkbmafg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2aarrvqxj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pfmpeveu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2altqprld.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qcmgyjdx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2balohkie.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qutihwsa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2gbmahela.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jaynbbxv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pqdmhigi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nlbheval.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2diiqfuxq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2drqzvtpq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2djqqvetl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pohiayug.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zhmbhhpr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lbhprnbt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bwmpgrfc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lwfgujdn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2atvgmvrp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kujrlamt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mzikqcys.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vjrvcaxt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2igfpanel.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jykdvvde.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zlpmhftq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gfydnvju.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vrrqgsjz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2phniyqfv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2pnhuouiq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vrqrybff.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fznlktry.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jdpnwssg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2laseibqu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2letbwpcl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cijqyxoi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2whygvbss.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bvrswaue.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zkwqjwlh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2sgnkhwqe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cgrcygwj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lqfgqfgk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2nxrdbdqq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fkqalwei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydugeirr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2dwcbglta.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2lpcxlouc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kknwlnpl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2eorwnejw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2nebvonfm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2epvehkuz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ycusyxgm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2mpfvrjyk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ccvsiico.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nwbucwqk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fsppowax.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2eijepfab.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xjwoxytg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ycpfiime.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2uukeimbq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rqrtebub.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2jqxueqeo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pmryxqso.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2pduxnhma.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tmoxaiig.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xjjciqth.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bkybuakt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2odnfrtwj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fdtjyvwd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vipikpcx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lsrhbtnl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zdvpxrto.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hlvfsbyf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vrtiieya.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uabacqbh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2uglvmqvo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2omvlugrs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kawtnsxk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hlbmmbvh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ufxjtqvo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfeutoel.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hhrqifvh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2blblljbi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2spjcumib.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ztsayauj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mryitidk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vvopsaci.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2wkalpzsc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zlpvhxho.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mseichcl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ptzgevhp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zdvrmztn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekoynigt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xeonwatp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsiyryex.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mmfgkwcm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hxatpfbf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rzgedudx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xizfmdxa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2cnlxxwpl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jlfkdxbo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2womdolvu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qdcmtnwl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2upgkahdd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vjoxrpdt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2iduqmlmx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2oshwafyi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jjyfenax.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2bmmcgdpn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bnzbffyc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ilhcryls.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xqcekxjs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vfqybgaw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2anuyolra.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wlgeyshk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pkxcahzo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ppzicqpl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tureyrag.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kzscnbhl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mfakrvef.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ynizlmos.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xwnmjwoi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2czsjbpir.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jppwyvil.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iahfbdsm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cjzrkcqt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yexzbast.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hgxxxckn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vcyhwnnm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpinitc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lfhxrysf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2okunqlri.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mkxrnbgt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2busvkxmj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2foylsnoj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2siylfqbk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vukywbkg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2svcryizr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xgfrxmzi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mmbrhsxh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tlxduntg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tuyrkqlk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2biuyhzxd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2csiplyrf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2izojscfq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ycnatjjz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zjhizejv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2lnqtiivt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ovbwnbcw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2okzgamsy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2prmhcasi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2phwenetb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sxzpejyt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rzucmmtn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2suwrqnzy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwuyste.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkifqz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2esbfpygu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lflepoue.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2axxkmzew.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgdexdv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2leecuhop.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2alklibyp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mihltzas.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bopklzju.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lgodojhl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cgboivkl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2anhkhjky.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnhiige.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgscvguc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hrfkmupt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ggnsgusw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyqjyupr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vzmyzgcc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mvrlnnfy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rdsyfoam.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2awwidxct.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2emtmokry.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mqdtloxu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvwtpggm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijfbrtqo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dfjvesay.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ohnkwsuc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lkcsjhox.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2zwmxokua.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2uldhlour.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2llhelzsu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eukqhbnp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2okmmrlea.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wechkdbe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ocrbrbep.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dyyzrrkc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mpvhurkp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rgpdlphq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iyltryua.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ukehnwcc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxuncrv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2thihjyrv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fqsruqlv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzngaah.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pxknnxiq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cohlbdcv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2thrzkuhj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kbkldhhk.html


<!-- 参考信息 -->