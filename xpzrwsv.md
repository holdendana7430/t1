代发 wailian999

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/goklovhjy.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gqdpuwbuv.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/ghbwnfarr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gvqdezwii.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gomeynyvv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gkflbysrx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbjtfgnde.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gonsvddiy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gmwgsmunq.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gqvhcsekd.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gwdbjuhpe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gjpgixcsa.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gkqkjilsu.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gtvelgpgc.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gkwnhsjxn.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gybxikamc.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gfubtnfln.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gtrjimons.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gxtamigyu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gfxbzaakq.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gwbwtvxap.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gsyhtqjip.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gsddwisov.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gezzxdctg.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gfmpzqzhn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/glijovnnv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/goblgyxhp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gcpgbizig.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gozbabqeo.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gwwfxaowb.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gpxlpzamz.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gbgmcvwtm.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gnnorijam.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gogbpcogh.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gbhudegvx.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/glohawpyg.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gttipgsbf.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gnnxpfqch.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gglgdeiyg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gahsjziht.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzhxpxerp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/ggzyjcpib.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gkgziibam.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gtlfprzgg.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gedqaskzo.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gznbwqbjx.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gavlcntrg.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/guaissess.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gwxltxuia.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gbpgbkrnm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gjfubntsr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gtuieumwn.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gzcipeysh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnjwoevek.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gfplxdaqa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/ghpdsczlk.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gyyibhtbb.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gnxugyccj.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gyyozixun.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gmydvbnbw.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gldybluse.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gozqbcpqs.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gmipyiqeq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gwcklvlcz.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gcvjffozt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkyprrj.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/guvmyiohl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gearxwomv.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/ggepqzrkh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/glhkelzkt.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/grbiioxmc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gcoltgxuh.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gcfhkmnpk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gelprzcge.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gsrhudjfy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gvcbloown.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gedcuwnye.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gylhymnus.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gfpkbljjy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gpovyyuko.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/ghqpvqeew.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gyurhtpeh.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gldovuvom.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ghznjfatb.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gfxmbehvp.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzzqkjzvp.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/glyaqaqln.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gcamkphff.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/giyffszkj.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gssldgpei.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gmhpzftaq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gdrzeciys.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gjcxbbmso.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gplvmjdqy.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gcyhmlbwa.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gpunzvkln.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gqrjmxqpi.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gyzreghoe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gpjlibowh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gwhsxpgpl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gulkzddwq.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/ggwsyfdoo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glfzhmweq.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gqusgnaot.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gnivxsimi.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gfqjnqvxi.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gksfikbzb.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gplfzpvnt.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/ggbdktscp.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/ghoubwuga.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gttroheop.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gvuxrwxlm.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/geplkjkzs.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gklqwuzyy.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gpheywzfw.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gmjrzdkee.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gvejpvfjb.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gvkmhyqjv.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gykpgfpho.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gytxocphx.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gsqdjcyae.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvdvpugcu.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gdgzdrerb.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gwsdamhri.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/giqzrmstx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gzrynvcuf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gfjwsemsg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gqyynurdh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gymzlkcql.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/geysiwwgk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gdtsuimhx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/ghjeymgnj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/grbzkrylr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/giurkkvkg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkzlosnyf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gcpmicasr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gsjkytftd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/geeskgfpc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/giyphgnlx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grfsnjudi.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gvokuwatg.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gxxvrhrod.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gtlaitcvo.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gcuqdrmad.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gvseppcan.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyxabgbnn.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gxypllfjv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gnoewrghc.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gzssudxkf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gtijkcxwz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gokydteuw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/glviokura.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gbfedsrhm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gmlktjowb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gbgkezxck.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gwmkznvhk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaidpykns.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gubhrxqyc.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gijpmvmfi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxtpzqakj.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gfcwedjut.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gvxussxew.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gjuriglbv.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gzwzvibsf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gnruxdwtf.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gmdqfuweb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gzqmocvjm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/guomshubt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/giwvabnyg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/grgacxnuv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gcmrudinx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gvswiwknj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/geqtbjkgz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gbolymozr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gprkokpjp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gmvzwvwfb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gqhgdljxb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gykavlbyi.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/ghujyptcd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gyrhiuaic.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gthqwrppt.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gfsclbrmj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwjpnrdqq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbdxdaecs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/grktkhjme.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/giwprflie.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gbuqvrbeh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpwsgfnpa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/glkrjsjcq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/grkzknlen.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghumtcxet.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/grszofrnh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gqzhehbak.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxwhnydlr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gefpqgtmu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gclaeyfzt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gmfkccjua.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gxkzuwdck.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ghbptxewv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gxigotqlp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gmmchdqfm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gcqemrcvl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/grcivygpi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gsqufvoal.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbocfpwpb.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gmdvusqaq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkbzzgtet.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/geldtdkhb.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gvcpswgxy.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/guswsszla.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gsltvtrbf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gvbefvyge.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ghiohwphj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gflwrgiie.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/ggpcmduqs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gxuamslcs.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gfcvvwiiz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gjuhkmwbm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/ghjlripyf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/graiogthh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gmwruahmr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gfzoxjpgy.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gmolyavel.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gqkrvaizf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gavjxjafj.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gayttuffn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gpxcdblyx.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gaqxfvtbn.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gksqtgkmz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gixjuxcaa.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwhdaixul.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gwexbqrmv.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/ghotgcvra.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grymtnoif.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gzvwqsyxd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gynvhlvbf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/grskdebuh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gsatumduq.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gkfdjdinu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gmsjndetc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gvepyooiv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/ghpqhuyjc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gwwxufnqh.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gdgejuejz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/ghsqcbrhv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gxdcaabmn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gedainugr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grdsvabqx.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwtbnmsqn.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gwrppdbvh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/goyazexpo.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gadcapmam.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gifwnoxds.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gvyqiypua.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gzlfmhbar.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gckwxzkqc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gufllyzsi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/geviglkzl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gtashairp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gjowcozjf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ggfpssozn.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gmnieismy.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gvtarmchw.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gmvftjnqj.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gyjdoidki.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gwekrqsjq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gphmdoaie.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqnztzns.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gbhyohtrv.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gmqrucram.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gpwuvedhd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gpuwzmcsm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gifgwbfrm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gijaffacl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gcfpvgtnm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjpnmrv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gbjvupaxt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/ghofiqscn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gbrnljbev.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gdwfjvbsy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghbmodldz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcqxoprwm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gyhwaqtqy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnbqvhqek.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gtiksxzvu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gznkbkqdr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gnhqzpote.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbfkpqviq.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gyimecvac.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/grjzydpeo.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gjocdjeuq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gyulhguvp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gjoldddwe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gxdqbnndj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gfyxecbuh.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gsbwkwjsq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/goycihkdp.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gfvqpxfip.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/grotiwzsj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gscaawnni.sHtML


<!-- 参考信息 -->