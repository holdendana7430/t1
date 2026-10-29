代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gihprtycj.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gmexkgxef.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gbceihccs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gqrogkvnl.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gpocplhxu.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gkmslncss.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/guiavmjxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gjljzlsjm.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gwcqimtqu.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/ggwocjgsl.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gsatjnzsw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gfqrhwkgl.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gnjxlisqh.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gjxscssxp.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/grxebxqmc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/guwkfrjso.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gocbfgsmd.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gdypjrihs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gqqitfpji.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/ggwrrtjyz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gtzhrnslg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gmoxevqof.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gixqujubr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/ggfanxwco.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gktapfjzi.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gnwjoeibl.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gmzaoxrox.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gzshydnkb.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gmjwefyud.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gicijkgqn.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/guasdqehq.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gilhxetgc.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gilqxggkw.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gxbprmbyf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gxfthhxre.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gurtjlhmo.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gcqiarbth.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gulfwoklm.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gphuqipix.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gkcewcexm.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gwvplgjce.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gwupdkwmr.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ghiezlaef.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gqivvcoew.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gunzeiwlj.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gyxhpvwwp.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gkkuibzbm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gemxnkcuk.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gjnsgtoae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ghxogphvg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gdobbggpn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/grzerzjeg.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gjcsznhdk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gubsbputk.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gljlytydi.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gafwbcltd.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gvckwgrym.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gxejsufgc.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gefuujcyj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gjdpclhmw.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gejxcqnvx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gvaevugtm.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/ggdfcrkcr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gjpadfiea.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gfgciyjpi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/ggwnjrhem.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtaebnnno.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/grhtajxik.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gxwvodlkp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gilvykxst.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gopkwxsed.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gmkhtzlhr.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gbtivtlmi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gryecrigx.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gczghkehh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gnngqihmd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gfbrstlrz.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gdfftndlc.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/glzjepgyz.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/guthfpsqo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gaputsyqb.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gewhtoutb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/grleatnai.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbvmovvsf.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfezhkwzr.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gmlfaegdu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gtxjraljv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gxsywsqsb.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gkeflpltl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gxximfmnw.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/glbdlioyh.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/ghjclhmyf.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/ggecjbgsk.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gbrjgboie.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gofrwcgwb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gwuymjkbs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsbbbfpsr.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gnhcvzlcz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gojmbhhpn.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gojulkdlg.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gpylnwzia.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfpujvj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gjrskzler.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyvuwghpd.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gzdfwhcow.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggrevsway.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gnqcvvcyw.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gkwseaehv.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gmlofftis.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gytjpqdki.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gxedeumfz.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gynwedjrq.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gnztrwitm.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/ggfptvyhd.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gbqbifgda.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gmsnjwhzq.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gqtyseohq.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdcvscoio.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gqyolgplw.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/ghmrkrfhq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/giclmfuor.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gimnbzoum.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/galrbiafy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gvfcaeida.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/grqcikjdb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gzjumwvzl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gcsdfkzci.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gefdbvmlo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gxehpzfxe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gjqxrzcmj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gwdawyzhm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcskofoum.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/golfyleok.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gzzmcbovg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gaxjpyczt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gixvunbdc.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/giuhwzgmo.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gawbzlozy.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gkdjkqkfl.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gvwvjbfoo.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gwdeynoou.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/guyuxuflt.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/giyoltkgc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/grajuygyp.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/ghxagdpia.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gralmxcwf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gozfbdxgc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gdjggszfu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gtuoonzou.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gqlomcbjr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gzequljqt.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gequzdsau.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gayisvtnc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gfosmfsyn.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gipgpcusd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsocbbbkq.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gsjpgmhko.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gcsoijgsb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/grevjkjvq.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gdxbhedcs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/grnoxewiq.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gyknnfbpp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/glubcswxa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gcadzsgjn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gcoyfiomy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gnyinorjv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gtvsebqgo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gmnzdmmhn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/ghsdotpta.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gmrpmjgci.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gknryltlm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gkjexzznt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gsvtugzsw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gnlrahcwt.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gpueewncn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/geqefmqqt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gdjidfxax.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/grrqutrxp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmwnzezct.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmgtqvxpo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gappuhgat.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gunvyorze.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/guruulhwz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gvlnuoqig.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gtcrgtyds.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gztpiiwtn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gkosiuagw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gmuyoauqm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/garivdjxh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gumohkxjz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gupypkltw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtbnpnisl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gaojskpty.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grujdsrsl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gktxjflkr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfohxfspi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gmnbotlth.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gjsobahay.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbyaiciia.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gudbfgmcl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gruwdsuap.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gugviiszp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gasktojar.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggkgpwtqm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gufgahrfj.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gdxxljnzb.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gafjjduqt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gstikkubb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gyxhgziqo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/giqjnjken.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gvpwdhcvs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gnplfgnbz.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gzgpjxzfr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gvjarmxlu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ghwazzcyd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/glwjfhbeu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gquyuhkna.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gixkabjqe.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/giojsptci.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gzpahuqxw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gsvxvfgil.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/ggzydmwhy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gdabxqmlv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gccilwxiw.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gswjbephu.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gibrlaypc.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmebfexmi.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gszjovkne.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gpkzitddq.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdvhfnbgy.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gvbkmbkok.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/geeszmdjm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/giutqytgq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gxevejqhq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gbiujroca.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gnotykwac.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gxptlbnwa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/grmzlrxnb.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gahrymnta.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/garqteted.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gvrpmqkky.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/grrfmjdub.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkdrjjftf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzszbxohu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gzyzoainc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/giibmqrks.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gstyojbuh.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmrrnayhf.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gngphagzl.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gdayyljeg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gbezrizkg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gcytdkkdh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/glfxrbgru.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gquafmqmy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gohgjabyf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gpepqurdb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gcpmidlpd.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gvievhbym.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gcsbkjqyn.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gypaigoow.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmrldmbxf.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/ggmqwgpbc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/ggieojrtd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gtdtxxtxf.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gmvdmiufz.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/galbgiqcq.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/grsqpxqlq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gmwmamelx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gzublbzdy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gwmrtdrzp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gqjxptdph.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gqgvscfjv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gbqwggpmd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gwrfkvnpz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gcrmynjql.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gawswlwli.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcyboyuma.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/glcfrgrab.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/guxytorwo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtdjyxfjx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnrjlvcia.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gojfltjer.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gjslffdqs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/glxcrsnit.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gzfdfbzht.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/ginqoonft.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gsjmtygvd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gkocynkta.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gvciktvki.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fehbvm.com/Article/details/grdfuicrg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gkzgibmgj.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gyiunvpbo.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gczciwqsl.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gjqetiaig.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/garyvfozq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gmkjpdxgt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gnqywgquy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gvonwtfjr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gqvgbgmdg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gbjuxtadp.sHtML


<!-- 参考信息 -->