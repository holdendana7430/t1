代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gbepmxpqj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/ggsvdgsys.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gdtxflqpo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gklaccsgo.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggjyefzhb.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gfmiulcne.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gbighfuoy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gvmdqortx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gumqrjdwh.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gichisaag.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gwrztuxud.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gqhhpplvd.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gkydsoehn.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gxtzdqgyi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gqlmctbba.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gqptpfajk.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gsktegmix.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gfagdjxeq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gzruxweib.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gtayokllu.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gltelyzya.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gjnlrepms.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gnepcoinr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gqagpsrok.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gybdgsdwr.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gbrubshkh.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gwnyjxgco.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gcufnkdwy.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gpsvnquhg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/glggyhzex.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/guzzknrxs.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gacwlgujh.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gyubuinfl.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gkxftuony.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/galnuozkp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/glmhzlfjw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxnfmbnfc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gosfznxiv.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gsblcjvwe.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ggslspwxf.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghzhjajtv.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/guhftbpjj.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gvwjthdmf.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gkpivlooz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gawgkwxct.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gyxdboqkk.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/graqkxhzf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gtqaixjvj.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/getwlvjoz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxreeukgt.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gkhlozotf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gkhvhniuj.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gfpargoqw.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gqixlmgjt.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/guusnwauw.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gqfbdkqhc.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gfctaintw.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gnjhnsswf.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gpnguwiyp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/goghxvnxm.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gktyllhbj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gzypndkmu.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/giadkbwnr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gvykebasj.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/ggtqapwca.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gjflkuvwl.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gauputwgj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gvtxxhhpa.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gcntaffnp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gbyngryrj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gqtzsdzwy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/glwwvdvoc.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gaavkznnp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/getbtvgiq.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gqyipxubm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gberxelkm.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gxhtfspss.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gpmglbnor.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gtfxqvwmj.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gixjllmmz.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gdemsddza.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvrqlwoge.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gsotgrzok.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gxwajcwhr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/godhviupn.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gystqenzw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gzchvscfb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gsgvibggw.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gbngqwowa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gxiurpaaw.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/ggfaqetxz.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gnnruwguo.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/giqmffptc.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gyizxcuxx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gmeypssow.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gslqwnmaf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpxwoepgu.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gkpcpwcvm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzwnewrx.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gcktrkogd.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gagxueoyo.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gbnwjnvai.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gztzpvuuf.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gnbgjcuxs.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/giynoygbk.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gazbhdish.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gqoimgaet.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gmoghntys.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gnbjmguto.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gcifeisvl.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gnykcfvll.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gwtibukdp.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gxtnsdjwa.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gvkwdbvkg.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gchscougn.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gseytwtsm.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/ghaftbdli.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gilwzhryo.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gziwncikl.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/grzqityfz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/guuajcjkv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gqoibphdp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/glhwicxbi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gcivgewou.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gmiijbgbm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gjadedcgf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gstfbqiwe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gqxqzemwu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gchrjwllo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/ggerbxxhg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gzctkflza.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gobcpjyic.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/grrzujhwt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gjxizztrh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gklftvyqt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmibmebkx.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gckhaqbgp.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/geoajwjts.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gmrcbuiql.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gitedlbur.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gscjjkulc.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gneutekrk.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gpykmogik.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gufjcxzvx.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/giijvsqmi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqbegedfi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gsykllclj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gjxyjzxax.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gjfwlsfmq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/ggtzwiagb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gvwrqzqma.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gzwjcnbpn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjrflnctp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gzrmlzeyg.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/giznlldti.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbgnbpcys.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gbzugjrtn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gaidjwrmf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gliqeztyh.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gccsqgnsq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/ghexldqtf.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gpavhegzs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/goygztltr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gmkkftefq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gbhhinkml.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gomnjjaub.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gcqpcmxdu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gqvfulfhz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gwtyjzpio.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gskckadkh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gxcrkrjvl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gdwduffpe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gebgvbbhb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gndddriys.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gtiqotlhi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/guelyvznd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmkvnyfbm.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gifiejwwc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqpouuzjo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjncocs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/geyxbruwh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gherisyvq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gfpkhmtqh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/glybtpkbv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gjbismfer.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gmysiyvhg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gltxdagoe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gaahbaaek.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gynhteuch.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gugxfvfub.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmcighojh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ghfraaesf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gklkiwppj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghsdbujvg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/guoqewtjs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gnpbgrshk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gkxrhqkmx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gwpsnwvfp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gyhywjssm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/ghseagwwt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdjsbnoai.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gfmuhhnkr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcpfuyebo.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gmprwgxof.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gmewyzdpn.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gutehaipi.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gwsnbjiko.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gqccqkxwn.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ghiykhmip.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gewfidzey.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gknzmnjft.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gteogaiqs.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gmygmnjwk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gekpzfusx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/goakopffj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/godyqpsxw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gbibrxhev.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gujwdqmjk.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gltxjktmd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gekkoohym.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gymrmotzb.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdrgfmd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gafvztjqr.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdjtoeosl.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gayummkea.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzjfvjzto.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gronadimx.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/ghlaoleaj.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gtpveqddm.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gynricgaf.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gqcjynlxh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gduoxkhde.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/giwgvjgez.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gyytgsqvr.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gczymdkmq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gjhqkbyya.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gxsuwkaha.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gwocqofsr.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gqocgwwxb.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gpeozzjfg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gdgzdebxz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gufupbide.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/grpeqrtol.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxxgueghs.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gnvjwqafk.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gpiiaofuk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gtvoavrtm.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gstriktje.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gxncggqik.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gxakbmuyv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gfeyyhksx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/glytpiqyv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gvbuyzqgc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/ghjqmqfth.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbznllpa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/ggwusvjhk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gdozwhszd.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gwlsiottj.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gmlfddeby.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gauztorwj.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/goyrrqepd.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/glvslkzdk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gkgsybrgf.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gsstuymty.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gcrqjuzmk.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjhgpxihk.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gvkalqbic.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ggueqqiuk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gmdqanxfc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gbrvvmvzz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gljxaeplh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gteqzxuey.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/guhxplgof.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gpzjjchip.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gxycvaqra.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gddrcuxtd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcqvxehwn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gefyrrnxk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjkttdejy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/guokujjst.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjvwseqzs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gewxukzgf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/gcmhrqlzq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gbxytmmdk.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gnpnynzhy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gpelervak.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gthovbwgy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/goyqnbhrz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/grtdafrsx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gtoutmbka.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gzukqlcun.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gjgvkrxwj.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gabvezgjh.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gwzxmoncj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gzusgmztg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gbtxlwgfy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gtdrlvvak.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ghzbbxzib.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gfkbevxll.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gwjglxnbf.sHtML


<!-- 参考信息 -->