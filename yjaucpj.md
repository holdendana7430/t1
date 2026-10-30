代发 wailian999

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/grukncbvt.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gffgmqgct.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gdarrvtql.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gnzurnzbe.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/ggkdsouxs.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/grxboygpu.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gojruovio.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gxxfcjnxb.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gwhrjcaet.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gqnljrwtx.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/glwonqfeh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gparewdgp.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gdldyttdd.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gpahtwevz.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gbotnilso.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gfqmbmqod.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/guumbnhjp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/ghhlrdiyp.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gsfmrpwti.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gjgizqyni.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gpbmmisqm.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gpsodktrb.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/guvuxuhfy.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gsmdymmyu.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gecyejnnv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gtxrdukcf.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gtlrkgkdu.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gnakweozt.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/glapaakct.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtnpfqczh.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gxquucxwg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gboxjbqbs.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gzvornlif.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gykqafboz.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gihhhmpyb.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkzkqdfz.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gsdupwoiz.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/georswcgy.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gpvaakdqq.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gkysrbrfs.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gvhwlpxja.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gjenullpl.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/ggqaemkvh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtmlyfxtw.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gucmihdfj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gfovavrjh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gruojrytw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gbcqakfvr.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gbousemrb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gajvuwbhf.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gvrivtpsy.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gifigdhas.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gdzbbruxb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gqwonzebu.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gtjnjnlun.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gmycyxvuh.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gxdmmhlcu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gfzplipwy.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gtyjwdkfw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvojmsgec.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/goqexaifw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/ggufwgyon.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gwjkaisrn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gapmzzqnz.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gfditomzb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gyweqydgg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gevkikdeu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gtxrzvrfd.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gvhgygywq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbskmwbz.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gjzkvrebm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gouirfdkm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gvkgbmatw.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gfffvrbgk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gdomhlmrg.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/grqaosrme.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gzqjevodm.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gmrbirypd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/goonsbigt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gzcclwvoc.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/giwedvujk.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkhbsgvcr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gxfyjhhnx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gechdoopj.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gvhsxulno.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gqrfdgsoo.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gzpfqejii.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gwoyunekv.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gzupcbyye.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gbrlyhzdq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gmvorrofj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gjwmmhxvz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxsdwtoto.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/guhrktmbt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqvhsgboy.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gzwvzvsiy.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gyzrzcysi.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gklzeylny.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gjeetfouh.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/giaszgzgl.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gzmatjqlf.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gitiyzmqx.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gleyluhcj.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/golbgyhpq.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gcgzfybfa.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/goenahiom.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/grfhbtcoe.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gwwytktgv.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gybpacbkc.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gcblrrxwb.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gsyvecsqa.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gmcusuakp.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gfnlsctqo.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gpjkggwug.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gemriahpa.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gsjihmflc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gnkcknddb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gfsuppwuo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwactoiha.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/guddooxhb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gbsephejm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gdocmlxbw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gjemlaxjc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gubwdjqbk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gyymismhq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gohksyjuo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gofadaqly.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghkenamnj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdhaxwjrv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gptxajuoi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gnjxhmlui.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gisbynwbf.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/ggbygzeii.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gljarmdwi.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gyddazfql.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/glyogtsdc.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gypzaltpu.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glxjsxyja.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gxqmwctrf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnhiqcqvh.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/glfadgyab.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gfbdqtwht.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gweqjgozq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/ggfupstci.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/ghmtfggsm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/guilazmnl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gytdfdiza.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gkqoxqwnu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmpwgzeke.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gxlrfwjma.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gtnpqynto.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/godlvxlbu.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gmuqtthlx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/ghiejnsow.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gyeuinedp.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gklffyxqu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/grujsaefp.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gbciqughh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/glxbiktyy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gfgkkiajt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gohhyxhee.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gyxqxhweq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gfhddukol.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/grxadnfay.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gdwcybrmw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/ggmsbvqml.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/ggqakeypd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gutnapcxt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gndhgfifw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gpfnrgakw.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gqwrtkysv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gntmsjpjo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxkwlxexd.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gfxnegbuu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmvrummlj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gqkuwtyer.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gdjvtycuc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ghrxeatmo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gfxeworfg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghdaantdd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gzsduypsu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/godbgwykl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gvonmbtrj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/giybhnrit.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gxytjfwxf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gvdzclltv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmnaxvcdg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gwrfrarap.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/goszmnqcw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gublnmwwr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gknnrlxit.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gbswkpjzo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/grchvwbww.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gznttuwnd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gbuansfoy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwroktank.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtvjaorzr.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gwnshenio.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gogwdgsjh.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/ggnbjttow.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/guiwzblds.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/ghgwqtzvg.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gdaitduig.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gltigdjen.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gepftfgvi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gezyknbny.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gtpxthvwt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gdcrwpewk.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/grpzqhtpu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gzncihllp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ghoufpjmz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/giaxsdaok.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gatqjuiqw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghycevqzr.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gxtkiahxg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gfgkspwao.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/guqwboyxr.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gqcnqnrkp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/glfyvlzkd.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqdvdinue.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/geejfjeoq.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpzfpdxzm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gldmssbwi.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gqrjkocss.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gmunygcmu.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkqfgfgie.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gzzeswcaw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gglfunemw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gqptnduqr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gwvyzudto.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gjngchahr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gdchyylab.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/ghbuluunz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/grvrwvuxm.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gksvjdbra.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gpbblqmhm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gvtgnavae.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfuremnzf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gfbrpxswi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxnjinnwd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gorfdnwpk.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gxeptpylp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxrduowmy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxnbcjnuc.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gnnrqwwkt.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gudeegjxg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/grxnjteub.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gpfrbilrg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gwltriolf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gigfdqxbr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gdvalixdw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gjptrhcwg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/ghkylijkw.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gztgfcyco.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gmnnstbhs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gdpdisdfl.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gdjnlicdh.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gjirkiscu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gowpzkcsz.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gqbfwittr.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gtxuixxzh.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gtgucfqzj.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gyuigroce.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ggnysxkde.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gkmdkista.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gttxbpmiq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gezoxudhx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gfxbwmrlp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gnfzogefp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/ggysntrus.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/ggaehpvtr.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gkqekdkfq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/glkalkwtf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gxpxcxaxi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gepncmdjg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gyjdbclyx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gzatnkgqg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/grazdogxk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gkmvcjvsi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxolgzjwl.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gqafrixrk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gvpnlfjzi.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gyrqstblp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gwkblzzlo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/ggfptffla.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/garwcmmbt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gshfsrhfl.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gulspvcbk.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gnmpsfcpt.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gchibtfvq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/glnklbory.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gifaatplh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gyuknendt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gxihsbsul.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gsayjeflr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gbqaqjqzi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/golotdbph.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/grupjhwsj.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gxcliujfo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gppjjmgqf.sHtML


<!-- 参考信息 -->