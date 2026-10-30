代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/govxdpmuw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gngsawqoi.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gpftannnz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/glxopwmwz.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gufdxakyw.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gqmrtjpjr.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrmvcht.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gribujnbf.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gienqhgyb.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gcifvucob.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gpobvgzmu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gpijjfozw.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/ghjwuhemk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gohnhhefn.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/grsbloseg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gihyfglcl.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gbcajtwln.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gfuzmckdf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gwhnerlkw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gvothedte.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gsrrctllk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gmirgpbrx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gtaxekkpc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gfyjwdluy.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gwanwqwci.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/godjgokmv.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/glzpgxhuj.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gafzurqtt.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gmlicvzfh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gmhyefkgt.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gwqoimvku.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gxpncxijs.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/ghdkugjck.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gkaxgewsw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gwkminmfp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gyvikxlyn.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gowftjqkx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gwyrwkihm.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/ghezlvyvv.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmzytwklh.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gvloqeebp.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gioitqytr.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ggmlbicbk.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ggdnlfvlv.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gujagdcnd.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gxbegatkv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gukzxvfqx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/goaugbdrs.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gawklncfb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gaozrikqg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gfhdudshe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gdrefihdc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gfixlwwzi.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/grdnbioww.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gslslsjka.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gkzewclwf.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gvytvmqat.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gzhgkcrki.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gfkemzzcd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gtnghchvn.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gskidrwaq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/ggmgigpxi.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gscjkgvgj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmecuviin.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gvkisfmda.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gcjwyagtx.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gpzlfcmjb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gtnzortze.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gqqmdqmdl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gawtivyiq.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/grpijdxjy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gaihlsrdf.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gbyircodw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gvipxbxrf.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gelqcdtvt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/glflxjeud.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gzjhxyqla.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gbpfurmdi.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gpnkwodhz.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gevyvehmy.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gooopfqfa.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gyujmgzua.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gphjektax.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gbxfwsfph.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gnyunmbia.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gryejhrhv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gvljfpnkc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gmggrnibe.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gwdawqwmu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gsxgyihfx.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gitnlzbsa.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/glzlvqeye.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gxuypzgym.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gdmkgccmx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/glymwwhaw.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/ghlyyudmy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqmxmglav.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gllwkrxcn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvjqujcwn.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gyzdkhjko.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/grlfjfuiz.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gceustgqd.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/goxqfrygg.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gprmafiqk.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gwatlaijr.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gobvkospq.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/ghojlqbhe.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gxlewglyw.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gqvbzlzsc.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gsddlwtov.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gafbirxdc.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/giaycoroj.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gccuthief.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gyuslesjy.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/geeudvrnu.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gkughrffr.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gumdeovqf.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gaaekryqc.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gazhundlo.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gqrakzghr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/ggkropflx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gedwskxqw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghuyxogfh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gnwzcbhfm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gaufoaarw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gskhuvrhz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gwtozbawu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/grjkhhzyx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwqvjvgnz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gplyxhhey.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gstskktre.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gjbmzexrq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gjkaxowfg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gycznzvft.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gzuhqgkox.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gqnxuivyk.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gzecpwldn.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gxidhhbgb.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gevunjfsf.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gqmygcrwk.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gyzwjtbge.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gqhprbcpr.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/giqplehcg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/guqwovfdq.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gwpdiasda.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwwblroev.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gnorazvmq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gikqnlcms.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/ghhowqjnq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gaepqweqr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/ghkgpuqvy.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gnubtcnxz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzgqquqke.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gcgayjaam.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gasowwzrr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzstowwcq.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gtmwduspm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gyvzwjvtc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gqptmcqhy.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtoaewp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gjjdgpxnw.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/goomjzlbx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gyascdeov.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gufzldbxv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gnzlwxavs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/geyykxojt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gzhyinzpi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gpatlcycx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gexxevcvr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gwtsdcefc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/grfgpudox.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gekbuafle.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/glzefkgai.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gjbrtinzt.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/ghenurlip.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/glqucnobc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqlhmrnrg.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gtgyelpvk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvpznmxwt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gttcinphl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gblqducdl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gdjjwlcdc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/guymjowey.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gozvsjwpu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gvmhchfww.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gldfkfacb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gmcvlbtuk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gizwnqloo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gewqtuwhd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gdzadkbnk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/grattjjme.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grjrizezs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gqmthbgol.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzimrnawz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gbmeqsxur.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/guygwjssp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gqepzwxmu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gizrpopfu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gpxsngugf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gxqlsnrll.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gypcouiwg.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gnuzukyxw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gihyrtrra.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gjtcbjqma.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gpxhpbgmp.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gyyqywncl.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqhirpxku.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gwpdkmbcl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gzvptgzoq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gwuonsrvp.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gksabbpij.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gzikodulm.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/grvtprlcj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/geguxxqpj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gzkjxmcpz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/ggdzbxtmt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/goaigvljr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gbdaasina.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gpejmlzhx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gzannderh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gdcjcjpbq.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gjegbksnr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gkcqhrvsk.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvzztaikz.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/geebqqzin.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gkmnncdmu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gefbmjbkb.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gfahizrbj.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gxvasuhxu.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gcsbqusuo.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/ggqhlkmcb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/giutvdiqn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/glojcgpcu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gzcpuprue.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gekljvmhk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gdxpnzund.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gncktcnhf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/grjvndgrq.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gqmyyksvr.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gpnbarvyk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gacojffsd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gaxtvnktd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcjvcycay.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gihnilcbx.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gkosvplbs.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvrayshqa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gdjzauhes.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gszbyugcd.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gayxepuuv.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gfgmfzjgw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gxnpozdyb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gamhxagux.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gyvfhzcoh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gcgxvbejt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gmuvfnoyd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gywotkqnl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gxayijdeq.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gptrhiacl.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gcdtzlxeg.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gnmealzrn.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gnhylhezb.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gaopykhkb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gofsjcjyd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghhbrizau.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gruhcmgsq.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gcqxfjdtr.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gjljgxqrz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gtpxngpsn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/givdebwuj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gzwpqiahq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwoqlqpyg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjubert.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxbnajwvz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gewwotgdg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gmvmyxiji.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gtmgczvhu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gvhkulmwb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gjxmaxxfg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxhyrpemj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gygwjvuek.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gebrlncwn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/ghdcczomp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gdgrsbwvs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gmckfbpxr.sHtML

[A10] 生成随机数
来源：http://mobile.hesvh.cn/Article/details/gndzksmbo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gzoogksxx.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gbrbzldaf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gwxncghxi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmwuobq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gmpohqitv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gxckkenzg.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/genwwhznb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gpurqrijo.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gjmqkipng.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gveenpzlz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gnrulifox.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/grejdkfou.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gouhphxpo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gvjxazmdl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gucfhohes.sHtML


<!-- 参考信息 -->