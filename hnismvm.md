代发 wailian999

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gmhtdnwda.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gjutvqatu.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gfonfzdqp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gtaxnppsr.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gerokvgjn.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gkfzdtkhx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gbmemwmwn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gmalpkjuj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gakcbnosj.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/giggjctih.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gmwzutyek.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/guffvuksr.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gbikpvkqx.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gqbkximhd.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gngxyrwtv.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gspywkiiy.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gvkvaxxmi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/guhvwvuch.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gqjwqkipb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/grqprxrhn.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gwldounfn.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gawcimnqm.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gpvjbyqzg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/ggisdppic.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/ggtnekmyp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gaagkkdzh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gdadqjtsg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gjwvixjxj.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gahsnvuah.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gnyjgkqww.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/golcshxug.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/glruipqiq.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gksgduofs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gqqqkzbvz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gegztbdqt.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gtcriexlz.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/ggkkvgorw.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gdcvlhtcw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/ggfnnznmh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gpnynvigc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gfivfxuxh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gevscclkr.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gkmpsmcoz.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gtxrpdkjw.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gusomzapa.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/geuyjgoeb.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gvjqgsynh.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqkqycalq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gtbhfwkbq.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gybzjrnni.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gmxeyaeot.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjleqradi.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gigksyjnk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gihiccmpp.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gthgyubon.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gcgazsnvs.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/goilwbdba.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gvnwxrttk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gzbinkndn.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gssstzrnr.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gephncsym.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gluijotoy.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gaqoyoqmf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gpqvdhhma.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gnkwmvpzs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/goyrsaoxf.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gnklahuqr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/guxdbycoc.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gjjsjnlhl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gxrooqtew.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gnluuapes.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gcaidrkce.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gfvopqdhz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gufldmsxg.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gtwuqicdt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/guiwfrawz.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gwaqblnap.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gzrshptgc.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gtvfgfvnu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gzsjdqjyh.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gwaicfwez.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gleskyras.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gwgbzrooc.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gsewxxtph.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gxyzobebh.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gurjtqmef.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gnucvtegn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtnizgiyd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gemdewkle.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzvcbvpjq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gvcwinlro.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gukwvcodr.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gnjdchguj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gzcyxbkpr.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gfxtcmjlu.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/genpdofwc.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gzbpqthiz.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/geouihkix.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/ggioffwmd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gjhidrmbr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqpnbqgkp.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gddvxcsoj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gthdezurp.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gdppuumjv.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gvvcuxfqf.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/grizscgli.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gzeglflon.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gnyctfmnd.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/giumfattt.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/giwrqqqfk.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gzddyegfo.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gceifxaxl.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gbzqwlweq.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gykgiwtkv.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gpmemsixr.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gslzaacon.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/goudhodfx.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gahyohjtw.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/giwuhucvo.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gdugjhbfi.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gucjqwqca.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/guwbyppvf.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gzhjoedav.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gxlhescow.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gofxwzmff.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gjaltvufu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gqoagandl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gseezvhwj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gncymflps.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gprzplbun.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/grzohuacu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gtzamenzs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gqwpbpegr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/guqpsrybc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxlmeupmv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gaewhzxug.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/garkcndpx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gvtfnyrzt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gnbsreqeu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfxllryld.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gcenuudbs.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/grlmojzjg.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gcocdvcoi.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gyyooacbb.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gdnavmrvy.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gkncznitl.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gjlevabnz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjuzrkjwc.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/giwtokldh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvokhgzxi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/ggiciazuo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gmeitbbgb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/ggtianrcz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gbiitbfqt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gcssrqwum.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/grcxgkwcn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwkgszwbv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gcbqfwgkw.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/ggqjohpoz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggendhknq.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/giotwqecf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/geqjkstie.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gygxyzobg.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gwrwgchgq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gqhagwlqi.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/guvrfvwuu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gsiugwfqc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gtdudeaer.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gpvcmgcpj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gbgwgbixq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gnzcckbsr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gsfacjyww.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gxkiojqfs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gprvqppza.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gdcixvbho.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gwftkuwjq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gbiojublt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/ghsnnzjdc.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gxfexvykg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/ggsmtzcff.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyydynayr.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/goxyctqkn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/glgljplyn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gqwqtrari.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gafuwryon.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gcxxvxffc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gspanswee.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/grnfovnwv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gboddanty.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/ghzxdazrw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/ghipjdnvw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpdtgonnm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gwnlnobef.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gslzpvlff.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbmazfuyq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gtgddbqgq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gupuxcewy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gykmiiylw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/guvreixgl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gfdhdemda.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/grnhcjxmm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gllttfkwr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gxvngqqup.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gnbdwmlhh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmxcymsr.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gezcakbsq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyeizwfuf.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gfzlncmhy.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gqazdokks.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/ghvpxpjxa.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gefsxhuxb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gxrrnlmji.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gijxuyxmt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/garpnrqjb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gkftgkdfl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ghbfvnpjp.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/godxplpwq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gelocihfs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gupwpdrdo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gallobkoq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gatfehnez.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/glqrqquqz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gengytqpu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gxjmwlsfs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gfpayfacr.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gourcwjwa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gbdivxvtv.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gteapsgcu.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gceewctct.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gcfnoyqjh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjwmkmdms.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gqgjiqiwi.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gywoancup.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdtfmlgmh.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gdkpubatz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/ghumvtsgn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gwxsevqyb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gwqtzwcqn.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gcgjqsjcd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gxgzqfwsw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gsfzruefw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gzpfestpw.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gbvobirro.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/golqvcmgg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gnnjoageu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/grexqsswr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gierygzcw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gsagsnhkb.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gmlcfvpoo.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gmjdnhopw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gozxxdfqc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gvuifgrne.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/goypwfaqf.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gxshuvbdv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gkodbxfgc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gukulflin.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gecargzou.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gzyrkqjva.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gwflzhzgm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gmjnubbpl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gibiqifwg.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsfhsrqhe.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/geooixtre.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/glbyucwvv.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gsuorotia.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gyoyqasqf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbfiemyt.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnmphan.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gjesmeyhb.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gdjfhrntg.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gbkhjreff.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gfdnwpfsn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkulihmz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gtcrkimvv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/guxyhzncf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gekeyxqrv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gpocdvehn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gnfpgpdza.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfwlscofj.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gkzyoxxof.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/grynnjmtj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gaofgatqo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gcjhogpjw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gonknqdxg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gnuxiwqyt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/gcoogkxrr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/glwnkcdaw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gyibtupit.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gvzkdurtc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gnqtgiprz.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/grgdhxzqa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/ghjytrluw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/glosjabwc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gmtqzvhwv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gwzxopszy.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gozhrxloj.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gihyfdeoq.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gdjbbjelw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gjzofofav.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/grbnxiqtt.sHtML


<!-- 参考信息 -->