代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/grzfwrfzv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbynzamiw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gejzixhyt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gxityxikr.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklfbclun.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdtvgxjg.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gsjrkrydp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gelfbviey.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gaahlgxsm.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/glxivvxwx.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gghdufmug.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhkbwwoo.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gngrncrlm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gdsuejajb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gogsxrjjd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaeprvmm.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gvedpeaas.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gogvpykbe.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gryzepaiw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbndbtdx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gxxqjclec.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpmgupud.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gzlmrxqug.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfdyemyk.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjystcnv.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gorwssyeo.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gwognwmrl.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtbayugh.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gshvmirbz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszxugvll.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/glwiredpc.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gktkrxbfj.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouzozysf.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvddolt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfcgsozb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gusykxzxc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmhlqshap.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfwbzptg.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwionriev.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gifpleoqy.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpvszapsb.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/grljctwpz.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjxuhzma.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtthpndap.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gcybjjnjv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gweqgsdpu.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadhwidun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkelpdmi.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkynypdk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gdqiolcwk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/glmctjpzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/grtgxzshw.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdufoftnz.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gngszuytp.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxjfxvwr.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/glywwmprl.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/grbnaqimt.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwekcmajp.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/guztvtvva.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfffvsnaf.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/godwexrun.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gwdavycsf.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/ghasinouf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdosnxqm.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gcxmkdfzk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gkraaojiv.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmrwaogt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gidtqztno.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/geroldgyz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsnrcdwq.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmpqpggo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gopjsiqrf.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/glmawwdge.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonlhnqub.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gocujeili.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/glxstdwdt.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdznjahnk.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyeairnc.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjqpitmd.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttatfdig.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/glwcdjjzd.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gagigoctu.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzhviuxt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gblhelqiw.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdssmtw.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gevmxmbdl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/grmqnahrv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghacqmbgy.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/ghbtipwzl.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gnmxwqxxl.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gtirlypmn.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gketuyper.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqgdvrej.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbubvinrf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxxplprz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gmkfknful.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqomeikat.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkedqeck.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyvxmpvba.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gfblseujf.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gglppdlei.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/goefyuarb.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gnvresbiw.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/geyispitf.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghetjrvua.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnlveneh.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gaywcbcfr.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/glgnxvatz.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlpuukgn.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gozsinhvg.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gjumruymk.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqphltwe.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjicleud.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/grlupuyve.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gcqaylzch.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaochemk.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gpmyuomnp.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gzptjduwj.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcggrpxg.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gczalknwo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gsecqkcca.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiaawikc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gjwfolzvw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gejcluamc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/goauyyryc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gkknvlmqs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gonqiyujc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfqstmsj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkuceruy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmtwyhuz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtpmpayk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjegxwzsr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfpozifw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gtambhmum.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gpooefvik.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gudcmscwe.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntsktstc.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gtpbxbeit.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxzusodu.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gmunyukpp.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gutdlmeao.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gsbsxqzox.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gdzvhggvv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gvggrjwdz.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmcrcqbd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gdnxgdtjn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmxwnikk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxqseasl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gsfgbjnhy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gtnbkccdn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgxadwha.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrzdxcpj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmlrbztjf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gzohrgdre.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnkgkcyk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giqergbwl.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gujepxgms.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gocysfznq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/ghhnoyysv.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gehgnyevg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gypcobnxg.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gsbugkcau.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpwwxwes.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/goijszovh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gzplwddkb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwosvzalw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtejkomp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gwxptgygq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gliroxqpo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gscbvpqix.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gpqbqyuem.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlgjqhrf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gymdzxoyl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giafszoql.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gluzyqnok.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfxwlocj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghypunufg.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gtrqqprfk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnihaabo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grwjhnopp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqrtbwmqo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeqzlesi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtukqbube.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsoijjew.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glywohpsd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbxtarvt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/goqejautm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcwlyrko.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gidnkgcle.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddpewygp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghajgjusp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzavbwvde.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gagbwdzve.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdoijmzfm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlrrgwmd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxucmqzxa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcyfajjdn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmkrjinj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyswgxhu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmatkbmff.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfbllfby.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmfwjael.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlzadveg.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfabegc.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgmorhug.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gguxvvpds.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhfqzqoj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbrdupxs.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxmnatpw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gfernbujv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gozirzrqz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdcxmym.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gbpapowza.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwrodgig.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gdszhsetz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffjjnnan.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiihgcjr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtxxxvoi.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gpveygyjr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gjpazdtiw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gksteuhra.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwttpuzv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gnbdaogym.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxyriacb.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzwdshdz.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gcofokqbn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gerjemlmw.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwxljuod.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gqstjdlma.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmosdeuzl.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gyxxsezjd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzjutlmt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbextmrzz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbkagfhq.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/ghnfsrohx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwsmoels.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/gpbazthkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfzacxbe.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fanxiaobao.xyz/Article/details/gvleonown.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/goeuuytjc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fanxiaobao.xyz/Article/details/gowlwajbc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdubquccc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzdbjzkfx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvhckvw.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvdvbvhls.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvnifubn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcxewzunb.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtepmodzy.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurvijkzr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxinosxo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gogtbusbi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gikpadqcf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxpysmcu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmolchuey.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvwofmkf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviakykbv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmvpvwgl.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gntfdrcmr.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqiomwji.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggcgphmb.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gyftoxfxr.sHtML

TS:   String(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowtaesxl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncnnozdj.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gpqmhdhce.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gjpmtvccv.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmxaxonr.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/gddzcsdqk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gusbozfsd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gycvpduvd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/goajochpc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/glxbnvjpc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzyhbwli.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gkwqsiker.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gsllpjxkc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/geqkitctv.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqhrvukx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzuzbges.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glozoctul.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtjcxdfk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgexlcla.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsigaybh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/gyhnlhspb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fanxiaobao.xyz/Article/details/gnkutbwwb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdidjssnc.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grrjgnbot.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexpkqsfq.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrqyuzhd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghavoinez.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiuuuugr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gntobuggd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fanxiaobao.xyz/Article/details/gymxpkyjs.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcqxfozg.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fanxiaobao.xyz/Article/details/gavidmkcr.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fanxiaobao.xyz/Article/details/gscagftbo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwczmofz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvjvawe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gseqkocrp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmojgfwb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdknwhwi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqoarbvd.sHtML


<!-- 参考信息 -->