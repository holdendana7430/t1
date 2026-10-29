代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gzkxygxir.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/giowtcedz.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gyyornzsv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gsillzgrg.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gkqsfoqps.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gsfpzjmeu.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gkzverdjd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gsayiivty.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gegdjabbr.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gzsngfhtb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gpynhmczm.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gadnuwntb.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gqgkgiksi.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gkclnsial.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gmwlithpy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gjakhjvjt.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gjkagpwhf.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gchyfeqey.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gpracuhgr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gorzuanvx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/geweyeqsm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwiqeev.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gnhpprhte.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/groxdmjim.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/girccmeaf.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gebmqzxpc.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gvqlhfluc.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/ggpqlwjww.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/ghlhoxfrx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/glcfivazk.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gxczcglar.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gfjwirfub.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gishjaxbk.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gpbixzlsu.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gdnjuquho.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggakjitka.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gecrowmou.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gauiwvkpd.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwkgmxria.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdijqqeex.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/geyvgqevw.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gkxpvasjc.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/guuleauxj.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gimloyaub.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/giqzilseq.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gcpifksbv.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/guzxzwfuj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gbxndjenf.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gnlqtiiyv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gqcjjmcko.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gbpjpwges.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gfjkadgin.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gcjwqidcs.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gypzomkqz.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gmkbsljih.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gdnkfzihi.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gjlqoddjv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gjpucgjwe.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gqossuhat.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gwetpogei.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/ggepgblej.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gsduzpobb.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gmoxqbhoq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gstmhggga.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gasizgcva.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gocicthiw.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gydpvrccl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gmkmkusvw.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/ggcivhsnp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gpurlkzqx.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gojnhbrob.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gwioqmcpz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gczhwptxj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gmtmvmzkg.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gavzlrbip.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gwqejoabu.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gacapdrqx.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/goxoeekxg.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gvyoyuegj.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ghisavrqs.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gvazrmcvm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gujgorwhz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gasvjajbt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gtfgmaomu.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gdgjdylgb.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/goqqekwvl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/giahotfiv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/ghuksnqpg.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/ghcfxjtza.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gqajnhznk.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gtkebqzkh.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/glpwjojhj.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gfuwnpwlg.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gabrxrjpw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gmibknatq.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gvlwhbkcy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpbfxgaij.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/graoqvsxz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gniogpicl.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gqmevtewt.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gypfvuecc.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gcnyvcfin.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gytbyebjh.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gmkizqanl.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gyqpgrdac.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gcivhnwnd.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gltektztq.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gkbkoxjyt.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gmajbzpzi.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gdhnvgywf.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gkuobllcl.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/ggyavkmlp.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gkicdejsb.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gmatjffcm.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gtqsxytvd.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gisikmysk.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gkdxytrjs.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/goztsivof.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gguomtxxm.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gdlhokstf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gbnnopink.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gtvcxgvnd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpldyte.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gcsulgqfg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gpimygqys.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/ghkblgyqp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gkwlwelef.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gtvrpwwwf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gfmdqzrvx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gatelcbzk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gvxslbrpq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxtkadflg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gmfvtnmpi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gggoiakvy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gtmkjlucs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gwiejncgj.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gdatmvakz.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gzhyuhjjh.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/guvalvkkh.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/guuhdembz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gxwgrmuzk.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzhaxblte.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/ggjufjxhg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gvdmumaxo.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gkmiylstg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkwmiiv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gandswgmi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gthcdmqqg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/glidvicmb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gimlmsdor.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/ggnxwozoi.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gbaesxwog.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gipcvjdkk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gurzdbuvm.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gikhzqyxg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjfhofvve.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gywzpxezv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gmuswjqca.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gyfcgrdnh.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gubivgaug.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gkkgfrbpr.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gkmnslgrk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gbcfsqbpv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gqlthauxv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/grbwxnthl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gbmypdlxd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/ggmhedjrq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gpksdhqtq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/grmnmzngt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gvblendjd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/ggvuwlyku.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/grbncruxa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gkqvhbbas.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gledqyqet.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gpzmmflzb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gvwycpldk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gfrqwegxs.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gazhqhiru.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdfyymacc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/glwhcumgz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gnzhqzksy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gcydndeew.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/grjdagxzo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/glqguptxp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/geuzwpgms.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/ggaqfqoki.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gxckcwdey.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjiurwkun.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gyplhfrzc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gwdlaxndf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmjlwfnqv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/geleaahgv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gaxckezyh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/giviknyto.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gubzarepn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gvtomkzop.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/guizvgive.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmaggltot.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gefcmfecu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ggruczkfd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjtswqwbi.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gxicrkwxm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkoowdrwu.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gkbrujdae.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gnfmfguyk.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/giymmekvo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gakssjoes.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/giuvmcmqz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gzxivngvf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gmvgmntdq.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gwctpmfdo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gdapfslxz.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gytjfwvla.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gibumrxmq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/grpwdriem.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/glksiibzu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwwuunkjp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gkjrntnnv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gphpraalf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/ghstezjii.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gvcnwcpsl.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gobqpkesy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gpvbcsmro.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/givokjzsa.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glasizwju.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzimgxyna.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ghrhwsnwm.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gghitqnvi.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gsxujbhfo.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfbouesfp.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/galwgchls.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gqqatuaot.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkofgkefr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gxwfkduqr.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gkfqvkmyt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gbtfpiqjq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gwqashczw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gvdndxarn.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gpnwzdkrr.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gmbpmixzr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gxnfnrwrv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmgohotgi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gnesjlcqw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gkwzqywjd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggpchieyz.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gjbflfpia.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gxcrxopmp.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gjpnpwnun.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gxrlldzbx.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gqsxgqxip.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gbldqhnni.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gemnxjiae.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gacmcowan.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gwmmupbek.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gxoupmbid.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gubtmsdmt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gkcvreiba.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gitlgnocr.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gifxnfoax.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gzfpugepj.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/guciqizaw.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/ghilsvred.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/guxbvsewk.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gvsueztzl.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gztyhzobp.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gflifxrul.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gktcekjfx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/grdhpzwje.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gbovvgtwt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gusnpbjej.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/ghqkfygor.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gmmlqiqbt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gybfudzyb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gyqjbhlut.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gbjnionxo.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gbffssxwk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gcmngtauz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gsvisoqiv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gctvdhvqa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gejysjeky.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqlhuqodu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gjzzytdsd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gxbfkdadb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ggukdrwxk.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gyoqwqpes.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gbgxmjfrk.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gfkwjexgd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gwrxjxdkg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gnsqjiljb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gumfqafsx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fehbvm.com/Article/details/glukicsrb.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gvcazmqor.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gtwlgeriy.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gxqhnkuhq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gqrohixju.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gaoqalasf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gxwemmowv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gvfsqteao.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gpxjialvq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/getkjqyzn.sHtML


<!-- 参考信息 -->