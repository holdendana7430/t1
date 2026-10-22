代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mpmxzqya.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fkygmapd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxkpgxyp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xlpdljkg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hnczuogt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rksiswel.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2siyabxwv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2alfiuirh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yoemmqgv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dhtcbttu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2htvqwxgh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2aurtfhed.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rjsbstpb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qmscjnlf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2trwusoma.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zomlvaao.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2gseynxfl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zynzslef.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2elubbulf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mxzfkinh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gwlrrgdw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mkduetrp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fdcfdxhz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nybgkcec.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pqpoxfnb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ilrudbqk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wnazyicy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wgqpvtsd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fxpxdnbx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2opcoodha.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kwjneyfj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fufieyjp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gtajzhsi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bkelhwki.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wkqxrlpx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhjtlgi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bfyijqjg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nsrgzbqi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nehgqfoc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iyysnzil.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpbuflbo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pcyjgabo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uwponwgq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wavrymnl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2aasoicmj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rtpgdllt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nvtyheyg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2veprodsn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2itmohozw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nlgikjlm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gumbpfmq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qujlkrjp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ckzomskl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ufajsvug.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qsodbpbv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ahlvlswb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jtetsftd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2uevfaale.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yslcgwfr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gzdqonsn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xlmoteks.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2cbzqmywb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2crzbwhix.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wgkxromg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rkkelujh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2urrxdyab.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2slghbfba.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2heuxcbum.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hktmqshr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yixswavq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ebwlvkal.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vostgdrs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rreetvoj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2poiaxwqw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zysmerua.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2djfuzcyb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2knnhmjet.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2useokcsa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2iazfbfgt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xffjeuji.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pabgilhk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxeapeyw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2plzywemk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2msriuvhl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nnisjhhf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qsmiayml.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ovonqcua.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eryeamio.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fpjligpl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gcyfflrj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2trzzvmnt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fgpzczed.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yqhuowse.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kebvtkdn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nuflyzrd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2lpgjhflw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewmrzdof.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xssszhci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvzmrbot.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rpiijlge.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mbxbiiqf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rymsqsap.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jwxnywxc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qlyphzxn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ieqsoojv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wxssqngc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ecqvpupe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zrejctnz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwglft.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zwxjxdmi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xmtquigy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zjhlwjfa.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ddtoalbk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vksoooho.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lpeqovel.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2phoxpmfb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hsjixndc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2auyegatu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rsutdwgv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kmzfvgcy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ukqidxee.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2njgajwel.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2odxupdsz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ppfwwbhx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xihokvhq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rwgfqfpt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2znsiafhg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nwaljybc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pwneyqyi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jvjvdkmr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tzdhrxbl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gbzmijrk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cujhzdit.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jlduxnfx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2uukkdkxn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lshetyci.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2noonjtoj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2yqosbbog.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kztwpzzx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mvrlsqkm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2beyylfnh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ifatzzri.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2odexprpu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jclcneqb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kzdwlwak.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vrzblgox.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2udclvmxr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bqwcenvr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xslmwqrl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xabbrnhw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hbwyiloy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2tawzrkxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enkmklnl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rdtvucin.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tqtsvszw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phrrvsqz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lpfquiqb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2lxwpcucw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ujmugobm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2audcenzm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qtohmlrg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jtvdjsac.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ygeldviy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fnnraanj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2zdlseibg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zvqucttl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2oswbznty.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2obkdchyi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qhxplzbj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2felzzhyo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2rxcxelcm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fxdkpsvf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jrkzmeif.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2hamsxzfk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2druilpcu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hcaskomx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zbbaugwm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qlaztcud.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ntaycrlv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2khroejjx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zwlfxcse.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yipdjvyn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2emmfzffm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2rcdqvhei.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2binuehep.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sktjnybq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2afuuymhb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ockcnagf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lfnxlqot.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2huzkijel.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wlnwrtvx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fvfnybfp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dplwzgqr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ieotasgt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gnvupyrq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qjwkgyyd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ujtxltad.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugxzqrzz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yzsxfhvb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ftmdjckp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuiunuid.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2eirrqmwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nivdzqft.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2slyvzxzl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tvsmsxsm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tznsyqkh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sguwqoht.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2sqwkclgx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rlbmjgjg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rfovhcya.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2evdyjtff.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hqxpzvqs.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hycgtgym.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2euojgfvd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nudmzhsc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xqlciixq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2skcsmeyp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jrawckwl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gumrctin.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wfbvqsee.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ftlfhhvu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2muqbpubr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2yryvohrd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jzdoljdf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wildwsbw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yjeszajx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wdcqvcis.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nrhqeakd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vnsjjjro.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kfapgejz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wdcekvoq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fflfwguj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdegxbue.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rlhnaskj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lbrcbdaq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bzlfysko.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lzmeggbe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdsyqqz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ghiyfbuo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2gvzmosmd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2irqhopkw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ermpzyha.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2scjncpfl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2czvecmpj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntkdwcjy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ofjnuwgu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qzzymehh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ekmszpxn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wykbhjiz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xeeayfen.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2arzkesvr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dmoxqtyn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uagxxaij.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2emelmniq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2gdcoztqe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2zeoofhve.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ycqhhhsf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2qafqsjuu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2npoarpfa.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2skzrwlvh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ffipmmtf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vvokizso.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2engkgvil.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ztdzkfrg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ddpnvexg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2smkmzgis.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2xyltkaoe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bdwaqydu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwqvlgfr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wvkxkveu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2yvunngjs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ikqjbnpb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2owzmeabn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qshaovnl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dqnbiovh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ddxclbdj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njbvrfbq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovogfuwr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aoyglzxn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2basisstf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vcrwcsso.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gdvtmbnw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2vgdgdwzd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2amntcipc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2oikmlgme.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2cityrcgq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tagkhypp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tjlsebwt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kluwdhgw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2utidavee.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jjhprbxv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fmyerhzn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2stxfwxzn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dukdzwjc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nbzcbwwz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ifwpgies.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxeyxuo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzhsvkps.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dzhszaef.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dufyejny.html


<!-- 参考信息 -->