代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zcambpsq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gghkdodm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2owsmzueb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ddoherlt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ifwqluor.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ccthtpmg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nimovdbf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ogslresa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ibitjmpk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dnvqrbwa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jthighzc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2copayekf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nkuruxlf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hfzuyffl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fntvdfak.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bokhddfv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wreorkth.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2sdvkueab.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tukefaty.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kahlzewa.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2klrmfmgr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2clmidyfi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mkitcdgt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wcvuzpqq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2glqmztai.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jhehvtjn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rkwyrzpy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pneqildc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gaosrgfx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gqojilsf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mefilpja.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lqcpfnyh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ifephsmz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sxebsyvq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2mkeuoidk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxttejh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iwbqtsts.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gkorilym.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2cjzxuuke.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pihyxduw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iyjeitpt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lwzphvih.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfzzkrqb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ivbgfctf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2igojknro.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2znpwhkgb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2grjribkh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkgmdvnb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kideodfd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yrdizdxg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2afmkygfl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zaaojwgq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gfzxusjp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wsszpvez.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kcotxgod.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ptcqdhzt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2aapbtskg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mbgzfsqm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pzvnsogn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dfyqfhui.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2julubuot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nnoheyku.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bsystajs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ufjawjxw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xjqwbaar.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lwqnoygo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wsurooyd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tmlfnglg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2azynjiiq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vpskatdz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2aikdhjeh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yxezqynh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yfdvkopw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jzvetgan.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2elmunfpv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lnmgymqa.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2aupyqjoa.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xzewqxcp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vhcxtjgl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2khbdngle.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tyvifshz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vjtbcmyp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sfmgbvux.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2koukgpjb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uczdnmac.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tavwqkgq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qnkmigce.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rrdkgwku.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yqcsyyhq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ukxsbcvm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rkkfvytb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pbdmiasw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2vvqrkkvy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2peujtioc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2bzbdxkag.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2tdlganmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uieqctrc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qorctanc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mumprlye.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mwkvoexa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kgchqyjg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2khteouao.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vonwngyv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qtelnfrc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dohxfaxp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qrbgiqco.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bxoleciy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pdmjovhn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2gjdmcyhf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jilzgkaf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2cxsvyauf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mxgfgjoc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wawgztzp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qrxasuoo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2awpeiesf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ojszuesq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2brdcjwed.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dtxmucfr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2apvcdyaz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rgnbvwtk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ghkqqulm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2llzjaoka.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yfxxuaza.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aumoowzd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2iriczbmt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ycnomrck.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gkolfrbt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2loznqjvw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rjmqlldg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dmrzqyzb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dmpplcpb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hljbrizx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wupxrckg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bitcufup.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2wbzfqcer.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uppdmuuc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ezhnlwoz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ufgppaqq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uqalavtn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gxiilzyl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ouxqhmtn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tdyuhhcu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pcvpfadw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tzaaslrv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hckkpdgb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hiaxkqpj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cvelbqgl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bzykxlhf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2bwabpaih.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bokhyfhs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wgbtkgjx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2spqyrjcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrxcdsga.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ryhevwvc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hmxtwusu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpkfnfif.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pgvznrra.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hyirrfin.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mocrknkf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ceuawdpu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2wezqfqqm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mmncdoyh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rgdshfxn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vzaoziku.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ocutqinv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2sxlczjxg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2yknslxnu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2nrhqnftr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ygsvpain.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mzvrupfl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dnioxqxe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ssdaywer.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hlyisutk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2bzibchxt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2dnaduffz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2tfoltrel.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lncsqcnd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zbytpsst.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pozrwtmg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ldiqwgji.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nmcxbclb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngfithzz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dhkeufgc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qxjvxidx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bacyhhfy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hnulvbif.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnvflost.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kkxhblwg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jdkjwjvv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyzfhwsm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qhcicvbq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lwigdgwo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xonrtjxk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2frbmnjex.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkjtonmr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ufsjcmku.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2todeihzh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cmrxyryr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iqvshzar.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqemiujn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dixvwnqx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vesorqgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amhaueta.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2pvzswpzv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jyuowiqb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mflbpbos.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ksgnljiv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2pmbgldgc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xopiqsnj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wbofiwiy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2myvjuvdm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mmlwdlof.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2nrkuhyks.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2aqdqmyfd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ceahpord.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zhogjzby.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2lgtizxsr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bqqdesle.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bkdnvydd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cirkypdj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cirdinwp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ilicyrny.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2enoxyive.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bakcnful.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bhwnlpkp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2usrypizr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pvpjoahp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kdialmmc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vabmlbpa.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2udjupyku.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hrhozemf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rarunvkn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2udelhjou.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uvbvwzfz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2pselrvtd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2udlsfgsp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ovcntusj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2raotxxqe.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2orshkrgw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gikhelfc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xilnyfso.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sxdrhret.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2laajojka.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2btqypxer.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ykgfqhbx.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kxlhsusd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ixifdjpx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rttgzbmi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pvtoysxl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lqcuxbsv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ckbkvyyd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bnsiegqb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jxjwrxyb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hpzasaxi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2udqgwjwm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2zlvforyo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pxtsaasa.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vgplsclt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdflbsk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qrvndroj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2totioilb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ikiikcam.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aupwiapo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yoxempjh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jogsqfcf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2alrivalb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lfmujiss.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dtjrlxzm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgcxtqn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aviswqyb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hiokttux.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2frvrganm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwwthyl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2lfqgovea.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cagrdbch.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iwuekknw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huwmaumi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kriuggap.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uebzjgyk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxdnxvl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkunxidx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gbujslok.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2hfkvtkmh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdotatjn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2olsxptef.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mwbcyjfp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2amootfkx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2axjyrzta.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ywffwbrk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ysixunsp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fxysbrqa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2eknuvwpv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2btrjtfqk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bqoypfco.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ywavomsn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nlveosgt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fnjxibax.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wdunnkgt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vmqyfsqo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gvaskxav.html


<!-- 参考信息 -->