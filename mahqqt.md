代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vlxrcpdq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2waqxqmsg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2txxmxjql.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ocmaarjd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dglgrtxt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pztvyimh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uzbnvgzi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gmjqtvas.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2maypsbbj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ceuqwrzj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nfkjlrkv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2nguzjsdz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bejuogyd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2uzgzhzaw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mszyvojp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2intnayli.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zzbbheag.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bzbyargz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xefyqncu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sebtegyi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2sitxfmtd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jclhsdpl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ndqqmnkk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dacjqiui.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2erabdfbu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ymrmzzci.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nifksajq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xvxodpkd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rnqkptmp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2tbvbswks.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qkxowzjj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xvcncerx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2oipoaxfd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uiwiaopv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cdmrrdiz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqtqcffv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nogjakxa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ittsoqfm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2codkbhzc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wbeympdt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oweecgde.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wziozuzz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dnloynbc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tziddjjf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bqfeqooy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bmgtrsuf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rnskzuqt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqymvzdu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2yvtmttoi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zrofbtfg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dcaonelw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fzmjfviz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vydgenzn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cnhtccsw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ymqwsgev.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kcwakgbc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rwkawgfg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hmmkkyca.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hchvvzco.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ztbrvojr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bjamcxbp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rktnstwl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jjqpxhgm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cmmzdwvc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mneamaud.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zqaguqdn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yszzcpao.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gvfsoldd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dzncdqww.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2llxvgbif.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2quniysjs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cyvxmpag.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ltezsedc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rutcbunp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2haowqdsx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bldoxyxm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2odjejssj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rbntrkhk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qhdydboi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lipbznbp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ilqlssfe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kvuuuqyy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vxmnmhtl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cjiimyyw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2caoszuag.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2agosidnm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nmcbcump.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyflwxcs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ccpadtfc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fvxsdtbg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2avkzriwp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vncgmini.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sbugeerw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cfkpqjdm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2oqrtjwih.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qkusjhip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvvlxmay.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2peoiaozy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcskpiol.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vdyrhumj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dispkdag.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pxoyrspq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2bicggvcy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ukiwckws.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ohyyrlyk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hwwbiolz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vomctksd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2suzbiuhc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wdflyfzq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lgsfcsgn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gqacvdiq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jgmaapex.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2codvygby.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cnhbscxm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2yxricwvj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jqpgczrb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dfknzxmy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eswwffxr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fvhsxgcm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ayyerkpx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dcpgbvik.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2irdyiiyv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ujcsjnmb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kkvdpbwp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2loxcgzfp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vdeouxvx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mdfpcrem.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vyephytt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rrvhylfq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2foqhuuxe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eyaejyhm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ijvbswof.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xwuwbduy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ipcuzpms.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2lpcfehwr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cbqoljqu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tvpxpzva.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nghcmqtv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2nshtkhjl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bnauhmgj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2smgtqkqg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2otkkisrs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tzlwxjnx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rqlywepk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2twklidgc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ngyuszhq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qpuworrm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2soumsqed.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dowaijsz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2oieyimkv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kyoramhx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2shgtwqee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upkxmkwi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2umdwepnx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qifzluyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esecaagg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mggclqsr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2lgeokgkl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2foovinnv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ucpegjpl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jibwcaos.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2letlflnw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hlftaagk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zzpixajo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zuzrkcjl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2antkmzpr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ufqfolfc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2yjxyqdow.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rmqydlxz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2exyffqyn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vfdcvmdl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2xliimhmn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2oaccydby.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2psfznkjo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2muuegwcl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2znzcjaui.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2swwspyao.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ynqicsyr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uevzrcbi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uukzndgw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jvsduvnr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfcncmru.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mdjzktzg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bseitqqo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqzedgkg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2haotwowf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2njjjrbcg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nuktopco.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2guvugkvg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mrqdcrqo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfyxslob.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lamrmrop.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2euzrjwsc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pxhpptfh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ilfrvspy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sfnsdsol.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fpshzxsd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2uxymgags.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tctmoiaf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsukodpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oycrpfqw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zjktpfwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfimsrsp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ejiahvbt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ivjxcatd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yzfwskcc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mqibeywp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hxpttixu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ivhupazt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2iofyvaio.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2wrydecys.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tfwnnkaf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zbeayxof.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vbbfhnwh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uuvialvv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fsmsttxf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qntfhbgd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2adrvgmrw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ytmlhdrg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wsqzdbor.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eicxfejy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2morkybum.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pwwywgzy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qykraikf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mstlmubq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yembgpie.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aozgyxdw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xwvoxrvu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xyokdpan.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nzpcynus.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ckdgpudg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2xexmauzs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ampsbdio.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2buufawju.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rjcltgcl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2iduiygpv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2emxdmxgm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lurdhrio.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2idbgfspp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dgijqrff.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsatwfli.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gusynrdk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qlfszugn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2svvtcgld.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dzmvwxza.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2egcxwjlk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2damcuxpl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jyesrlxi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dyojjleq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qhzstwyd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yocetoxs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gaohfuwz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2euimxere.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xgieisqz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qxiozhgq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2pqrnmbxe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bbhaphjk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2biwviiqn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2frggfucn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lfpftrfc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuvpqris.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2msiziexl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2moiuzsep.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2budlyuxq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2csgilite.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hpswlqtz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2egwrmnhb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkmzyby.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2srcsmqrj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2npezovsc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fgavvsup.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mglexiil.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2idecrcly.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2troryhsv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eqfisnxu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hfjhziep.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xatmtqna.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsuosgob.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nkyebeku.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrpudhh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmbyfks.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rocaxsul.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2djekdksp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jmzyjevx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hbgtnrbo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gazbsaty.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ukxnwaiz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rlxujapw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwawxsym.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pzaqqzdt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2olvytoqw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2qvesqnok.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2drzrzujh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mehgwfxo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2eqdbgaub.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2odybxrsi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ytcfwowo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jluiwhek.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nbudommc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2twakdtfh.html


<!-- 参考信息 -->