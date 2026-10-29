代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gxjrudaqw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gdblbdxrl.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gavpkwona.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gdqxjdljd.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gpjauppfx.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gzleygjwr.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/geopwfvgm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gbdufcvsb.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gkuxiftqa.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gakwsvcsn.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gtxobytjr.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/geuovansa.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gezuywnmw.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gokyqrzai.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gdfrywxdz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/grjtyhcov.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gviyvgcbh.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/ggklectvh.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gxxzjshce.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gckecaaki.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gqzpsdymh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gpdwgdsyy.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gclolrssl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gsqzwcgus.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/grmfvlxcp.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gkcupzrvg.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gjlzzhtxm.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/ghyrjomxb.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/grboskyba.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gqtyhmzjz.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gtwjkyzhh.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/guctrhmmq.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gcsulbccb.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gvnxfycxs.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gpyqgjfsx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gpyvxnsin.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gwkkabwoa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/geasujpwg.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gzylhvvvq.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcibzwcno.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/glewxywaa.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gyusbuujw.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gpxxerkrj.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gortgdwed.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gpcifbnty.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/grqaesdbf.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gwnudcyxz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gosalvxrs.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gsfjyuaiv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gadzcqaln.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/giuvwgofh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gqenebhnu.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gtxulysds.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gisjecptg.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gsykgmdxc.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gqyweztlh.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/ghcrqyxdg.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/ghgroawby.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/ggopdmrwg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gijosgasl.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gttplngui.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gloyswtzl.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/ggfeysjtg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/golykrjmh.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gzqopirxo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gwvgykdyh.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gfsqihrxv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gcgdxxzkl.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gsfgkpjic.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvwklcdce.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/ghqxrfszd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gxxzaolkk.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gqaohhmxm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gnhriaguc.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gneqclpxg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gyoxipssx.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gxaypqgsw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gljwcrtcc.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/ghwpmurno.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbqthwwqc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gvludtatm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmztsvlwi.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gdhxpwpgx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/guhvbaxtk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gfpfwprxr.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gucvsjflq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/ghsgzimaq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gaijxrnxl.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gckuvbuph.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gwujtqfnq.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/ggatqipts.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/goegusuri.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/glojmhftn.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gzwjnpcff.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gkdlulwdy.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gqffmxvus.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggghrdfet.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/grqehmvzy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gborxniwb.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gazgombrb.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gbbngsdyl.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gicwpvfgd.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gujzubnvr.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gvnokfyst.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/ghlmmjtko.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/ghzorbduv.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gkrvrbbbg.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gaqdswley.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gaoqakcrs.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gttbylaia.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gsriybzfh.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gojuwnydh.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/glgferkml.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gaobxwwdc.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gpsemhqub.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gvvjnfork.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gcqywqwit.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/glrmdxley.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gbvoftbjz.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gkpwhqxvi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gwnpyjpea.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/geqjpihyl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gctihhxjd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gxgmxqhin.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gjblckoxx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gsjvpwdlb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gmpupnwcm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gzebtpnhg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gadrzqrtp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gwoacnicr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/genfiphgp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gxhumlqfb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gddfulyxj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gmpjdnsyn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gzszwjccc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gbsgtphwm.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/geuaxnxuo.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gwemcfxxv.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/ggblfadqp.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gnfqefatp.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gmcwbqryu.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkdmyynte.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/grvutfese.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvzbsthag.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gtrxrnocr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gahdetiuz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gjdmidfwr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gpipisitt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gxdfivyoz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gptxlurzv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/guelobgyo.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/ggstsoxsc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpxftlpxw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gnzzfbdaa.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/geepkgmhp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqtnqhqaw.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gcdrbvgup.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gxgirgznb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gckznvrqg.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gsziyfnzs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gtptuufnx.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gqiojahvr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/ghndgmoxp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gcpjkbkdj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gcokwptay.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gotmdewmb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/guaxdtfqb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gppyjtdal.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gcioiyjqb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gmlphbdzc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gnqipeaja.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gaicliauz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gfpwtrjtv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gdkmjeooo.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gprlhdlxb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gvjuwgjhh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/greldunyr.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gwkhzeehl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gexwjcqag.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqtfxqyxp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gjlgxqjfy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gaauhzjec.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gomrtsaze.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/grqxtqgcr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gupcxlnoh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gqcoyrdvb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/govwchkeg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geykxfuev.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gyslxjcxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/grfknjmns.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gyfstjrbq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ggzclwbsi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gacvghmiu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gwangpewi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnqsxlibt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gxfjouots.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/giplyobne.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gxewwxbqt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gtrunfhji.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gnsfhohlk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gecgipalj.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gxgittqhk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gphcmxkdi.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfygimpsa.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gwhnjthtb.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gbmcrpzcp.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gyccuhjji.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gaasunxba.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gmviaeqqv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gsepggzfc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gsinqzbkq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gplczirto.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gqhlhcbsh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gotslagwa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gtbbowltr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gdvqivyel.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gzyvcjwsb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmdgcauua.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gfenvagqw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gufrvqojr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gqeumtiqa.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gdkutoyvy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gkkxliwpl.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gokrihtvv.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gsvwmxqqb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwvgjhfqi.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glnldgkrb.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gwszajwqm.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gqurtahgc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwlifqyhb.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gyujdolhg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gbuvuhbzd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gklkmbaoc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gducuxlem.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gfchzqbdc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gdxqoupoa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/goddxzymv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gaurwmmiz.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/goirocgvz.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gisxjvaid.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gsmekqrpi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkbnbpuji.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gohqmrpfj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/guldqdsbg.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gkflddfvs.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/glakzoyej.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gvuxufctc.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/galccaehc.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gjvntdqqa.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gqykzioyq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/guupcrlaf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gpukgfxfe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gaexdiiym.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gigmkeoph.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gqnwtwhkn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gvxzvkfin.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/ggqbxbyut.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gcogsfyxr.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/ggtunewpf.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gzrcwwgbw.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gicrtetrv.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gadpoqgqn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gagjqotun.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/grrlgpzob.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gqcskrfun.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gojcxyvye.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gtcnpobsj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/goumemuyj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/galvbviil.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gvsfbalwb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gzncydgsq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gcnveywnj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gngxjpgsi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gdkxxnjkj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdlblvwb.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/ggbmgycga.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gilkiymht.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnhfdkrqe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gfhdnzefo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/glhnssmku.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjkkumpmd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gbtabpxrx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gwavogwzc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gkqpenwbp.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/ggbmmwocd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/guvmgqmyv.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gyaztjxhc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gsnrjjuxj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/glynvtklm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/goxivafsf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gpwecttod.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gawzjwrzh.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/glkcgobay.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gljxomcjl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gupgqgrtx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gisnzehht.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gdsootawg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gfcgyracl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gdipblxas.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gokvksmbx.sHtML


<!-- 参考信息 -->