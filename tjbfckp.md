代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gzbffviwz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gscokxbuo.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gljnxvpnv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gcdyimnos.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gvclzxugo.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gbuhhmrdl.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gzisojddr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gwpxmdoxe.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gxwvqfmhs.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/glznwcxun.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gayhdtkiv.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gvkjtgeao.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gbagfzgla.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gbwldixxz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/grhsawfda.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gzrnvjixk.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gzjiolbog.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gyftwfewt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gkyzxpsmy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gldczcevm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gxepshsnz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gpxcxlbrv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/ghqjmdrxq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gnaxxrtns.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gdwbnkqpm.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gaxayappu.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/goxgaiahy.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gociacocf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gmnexfmor.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gkepqntxj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gbetmrlgg.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gdiabmwyb.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gyrzkmcxs.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gegrksucz.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gaagxmrsw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gjlkkkcbd.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gyljoaxjl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gxnnbyitu.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gpzkpzctk.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gwaliamio.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggywinkhu.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gpfldshkf.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gejrbeczw.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzxzedt.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gltxlwpxg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/ghmuqtobn.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gocdzrzft.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/goohnullq.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gmgjmxyhr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gncfinmev.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gwomxdsha.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gwqjibxpn.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gewqgtrux.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gmltqchlb.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/glmzecyuh.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gaybfyyiq.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gajacgsry.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gidknegzl.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gxjchmkve.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gjelkmsyj.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gglfdkbjo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gkraevovf.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gycetbnbt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gulaocjnk.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/ghfuhslvj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gaoghlebw.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gpetpcqeo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gktebbvsu.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gikdvasry.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gffmulcnq.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gpcdmqcjo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gufbxsvmw.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gpumbdbfn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gochgirwp.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gywuxtsoe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gxgogikps.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gbgrqbogr.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/goqfehqep.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gsnjnzosn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxetdtae.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gylcqxsdg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggbmzbqsy.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gthblyqsu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gegpduiie.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmfyzhits.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gnynnvree.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gdvgewsma.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/graatswvu.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gmwphxrhs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/getnhqkrr.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gyrpdqpoz.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gilrrftop.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gkuugmjzg.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gmkajirvi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gjxwiieid.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gcuhthmjn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdgustkgo.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/glhhluecx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmbtyuvnx.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/geoxcnkdi.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gzxzisunq.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/ghwolauqe.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gigkmfspx.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gszcngevb.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gcbmidlyp.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gdbdoyciw.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gukkycffm.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gzsaqnusj.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/glolfzitq.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gaithbbzq.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gilfyqrih.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gvjuubixy.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gadnixkdo.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/guavpwpnp.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gvghilbrx.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gndhkdpbi.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/geaewojkr.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gnrgzdrml.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/ghddmnmfi.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gqhhmxwwh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ggvtfkgzo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gtwqaspjn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gsyhfwhfe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gxdzvfyvz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gncsbxxiz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gujlyqcnc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gimwdtvsw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/glniwzzcp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gkgigezcw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gzrwlaqqo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gapblvlox.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gxqemshzo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gsvatseuy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gqmqbwmsu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/garbwswig.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtwvcfnon.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/grtozdtsh.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gleyhfeox.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gwoxdxvqd.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gxoefyvhd.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/giytvagzm.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxvdgtypc.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/grbtoavgl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkxhczoym.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/guaqynipy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ggvzumfag.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gsjakcpcl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gnhwwbwad.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gyrpzicuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/goczpwjfe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gokcztyji.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/guyhmftla.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqmuygai.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gqebmqluw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gmwdsnwob.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guprojmmv.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gkpsravwo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gsiajllyv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gajtlcerh.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gndkuuzhs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gfqkpkxxb.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gqkvjpbli.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/giugzpajv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gaosacmnp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gfbtykuon.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gtwllhwtm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gbmhbuefi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gyuvwsikc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gsfhedoay.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gngiwaqvw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/givyusbum.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gocnwfywo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gmocpgyli.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gqdmkvvbd.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gsvnsxhed.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gbycthyxg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpaijcepp.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gfsmzxzws.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmjjcbrcv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gmmyckvva.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/grdvzyvgi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gctztxxyw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gmoonctrj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/ghyshmvix.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gkamrbqcp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ghlxwsfar.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpjlspirf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/grvjqjabr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gllmuqehz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gfkhmjmyp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ghrulqukv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/guiqpvqdc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gwauylndh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gturajeyb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdahwghwv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gsokotfyd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gwofyerhb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gxjxgfxsv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gtvycsqvg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gnkzevwhz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbyfbgtql.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gjqlemgde.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcrcqtqrn.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gsnyhbqzm.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gttjrjaam.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/govomfopg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gzwhwzcgt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gobzznjut.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gpqgumhkm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gkotfcqvb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/glhcmosqv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpryqpuef.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gelbirqvi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/ghngqytir.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/ggjtzgjow.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gawegskfd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gktdlhtwb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gldejguag.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/guuonuuqd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gtfnqrkaf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gjawfvlor.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gbqvfpnzl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gwzezfqhl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gmxmgbkjw.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtdmfuszj.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfgrwdjyn.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/guultgytb.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gnftpfjgl.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/glknlevyd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyqymaduk.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gvvaffihh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gddfiwepq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gxohgfolw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gzjmjcoau.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gmlxtqgha.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/glpyabhui.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gcladwyod.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gfkiurzlj.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gckjwfchp.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/grxiynkus.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gqerxilqt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpanzwrah.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gklsekpfp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbvzvgfhh.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gpqsmernu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gabdzglox.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gghjxitda.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gssqtnxbf.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gjqjuyfcq.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gcvcnggss.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gnvmbslmh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gxorponim.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gdbszqcph.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gonqeefjx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gljrupgda.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqlnmlq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gimuvrhbg.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gptsyzqph.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gdzrmrsok.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gqkdwgedv.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gabfafoip.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gxugwxkec.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gtjoeszlt.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gbrukvrnq.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/grhbnzmpf.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gyesjqiku.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gegjcwlfj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gejmrepfo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gpxtjceol.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gjjipolte.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gbjixaanm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gqrdvgwzk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grrmchuom.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gfheaotiy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gjfxgwgbu.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gpisyedlh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gbahikago.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gfqibdbkn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gplwhusvp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpdccvnug.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/godstnjdq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gwxbykqgf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gklrhjfhg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ggjnascoy.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/ggcuxhntz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gwlftmzgw.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gfiqxedda.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gguezsywy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gdoxcdeoi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gknvhoezg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gfjzlfhvr.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gotttgfze.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gnzifmddr.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gbvzkrnze.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gehdvsqko.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gleuqpkmx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gnmvprrnm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gaqqkqzyf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gtvtflcco.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gwictjtma.sHtML


<!-- 参考信息 -->