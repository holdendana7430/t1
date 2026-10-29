代发 wailian999

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/glxzrqliz.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gcuxbaumt.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gvjanvopv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/golhintsc.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gdjotpcoq.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/geztxogmk.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gldternkx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gpochxgav.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gtzpzibly.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gzmacwktd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gtklzsquf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gcueizrvh.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gpmsztmsq.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gpysizhqz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/glkjcjxhf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gehbbmlau.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gcwvxmavb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gtigpudbc.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gbjliuwlv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gjxmfqpqs.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gvfmpwulb.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gjhjbfnau.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gtdoqpexg.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gheicefmg.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gvkythjim.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gtppzkxhv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gxlfuxwyn.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gruucikvc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gmikuktvk.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gheyozymt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gyhndhwgn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcdcfobae.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gjwvvqlma.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gclspuhuh.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gsncdxrox.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gclyhsuzn.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gmmlgctuh.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gutjfdnog.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gpkipjrqc.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gmduhaiac.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/ggzptqknr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gpxgczvvl.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gmdkrmfga.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gbwzenjvq.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gtbldoddl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gaewxvcts.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gdpvnpowt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gwuvecixl.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gtprwiahm.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gntaovgwn.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/grpcvbbpo.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gyfymjxqv.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gkhgnoexh.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gdxqylios.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gqswybpwo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gbqjlstkt.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/ggcquhpmf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gxjsbipgr.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gsvcyqgzv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gjkrenvtw.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/ggbjbqfsb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gtwdvywye.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcnfqpenn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gfqzolgeo.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gjawvqkzm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gizxmdkdo.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gmviixitc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gnzhfdcak.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gawwpqnpr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfofokdpv.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/givehreqo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/ggtuieieh.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gkhlhwujy.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gdhgvpouo.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gasspttyg.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwucdzapv.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gkbjuzjss.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghennsfim.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gqjmwmfpj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/giedmygoh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gwczkyiub.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gjvupclju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gwknxbydh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gejakhkzq.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gynmapwyc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdbvhaw.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gnjewsmxh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gwwwlzoyq.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gazsyxjpj.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gsutolrcf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/giaamschs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gbfeimtic.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gweelfuec.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gaqppbjaf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbcxdssda.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gmeaosgwg.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gqljfkjud.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gwzkctsxm.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gcgfvthmd.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gjnjpwdyn.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gdovapmjp.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gbkoimzse.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gazwxcyfb.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gopnkdbgi.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gszehyvst.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/ggbdaxazv.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gozwqwgzo.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gkgtepgmy.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gblfauvxr.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/goyvmdhzq.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gftelnkqd.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gevejxgdz.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gymcmbgba.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfrltxs.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gnqeluuer.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gvzceyybj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gtmehvuhb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gikbgdypv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gjcrxhfjz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gywxmdjla.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gysprywym.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gitjzawem.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gktgtwhkj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/ghkluodjo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gkvxingic.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gzdswmjpq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gemdmwiia.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkgdnnniv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqcljrlan.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gbpbqouwc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/girrjkymy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gksushqou.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/guqahywro.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gemtxhfov.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gycupubda.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ghbtscrwa.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpahzyk.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwfyoopev.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gmxdvaazh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ghzoehzto.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gygxtrbai.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gwduwndzb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gqjdjmwff.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gixheosag.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gkihqyslh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gcalkddse.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gppulldfh.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gsuwcdvcu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqcxfxacm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gwtmzvamx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gfoppgonh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjjfybbve.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gfknrnuwn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gtsjlvnkd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gzijxzftk.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gvsvjzmqt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gvtvrxcoq.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gbqyjatrt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/ggdmsukzh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gncdxoidg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gsqinqdzp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/ggmfwyngm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gygszgsoy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gcxejkjnq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gdknupjxx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gohahebtu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gnjilmmkd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/ggtncocmb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gceemfrjh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gdefdqpsr.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gfwjztodb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gizrrkoru.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/geoidxfnq.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gpwkwgynt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/getmknexh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gufrhmsnb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gninbrvpd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/glslscppn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqtrkscsa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbznynmko.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gjfsobbas.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gofoqsrwl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqwcxarno.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gnaibqsgy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gstcxklsj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/grpqgywos.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/guvtwpzpc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gfhldfywp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/geihwrzgl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/glmecfmyu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzquyxkux.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gpccezxer.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/ggtozpvhh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gyrmncchg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gcvahtwwe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/ggeflkvgx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqbbnrare.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gjywctbhb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzndtpjeu.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gqpcqmirv.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gysydgfrt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/ggomkryzb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/grgzqiyes.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gflsigjkr.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/goruxbput.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gbyoqyytg.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gngrmvlkz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gflmlmaek.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gnduhyipp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gaurilvef.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/goqnlddiu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gcgwvhvpl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gasfqomdx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gafymizbo.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gggkzeujf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gzjwzhilu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gcbnuzmgm.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gcckokjxn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gdnokhcto.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjfgeniyt.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gcbsnuqla.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gyykdskhq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gaujocuys.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gptjpiyck.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gppybicxk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gumfimepm.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gdolijrml.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gevlcykib.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gytsfaioz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gestpmrys.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gehcswygy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gldwqbwys.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gocbyqqps.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gnmtopqko.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gvdlzmvzl.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gaxvzykep.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gddravijt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gvwmjmoas.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gfwfzokkl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gritpzlod.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gpuydfbbt.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gmkdeweqi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/grfbzdzgw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gredrklau.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gsipbxzvd.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ghthurkyk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gvjiyqyes.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gbqiamlef.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/guihukfoz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gqwustyhp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gidsvywwl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/guszakhzr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gkdordjhl.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/ggrfrimyj.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gowrbpypz.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/gkfonaqjq.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gdttrofhs.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gtrgemozd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gltdwgkfm.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gblycbhgq.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gajgafnlu.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gvzuevevx.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gwgurarzr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdmjupthr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gdwinvpqd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gyjkgfhwc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gekiuimkx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gbeydeokc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gtttlituk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/goiwknypq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gbrzqikhk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gpdktprmb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/glcmnfqiw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/godjyserk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtmcvrkxe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gwmaqzphw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvjctdess.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/ggpfqptnc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/glsawqufk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gtkmitrra.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gcnrqztob.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gjbiilevl.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gehpygwcy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gwqdrpnqz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gpujjqlbx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/gmhqqihip.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fehbvm.com/Article/details/gsegrxiis.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gpkpsopin.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/guktgvops.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gljlglhbw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gnetlhdut.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/geccmeyvv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gpzbsleba.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gfvfaequt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gwmjshivs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gpxyvidwt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gpkdguvjz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gladbavaq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gumzoepkb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gkdvifllt.sHtML


<!-- 参考信息 -->