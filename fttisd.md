代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mxssjdiu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2swgetjqg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zycndprc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2unibgeyw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2egkucnwy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xqlixtdc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zvbhhmry.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2yujltrkw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2txeivpuv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xcushokw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nyzhntdf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pnsvyrdh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qaljqmrj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ukiyyusn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qnoqwjie.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zapiemja.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bmutzrwt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tcvusbbb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2umvmirzw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2phzambpk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2azwkjmur.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2smzvdcmf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2talkcxab.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kqwxvxto.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2stkqdlso.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2camclobc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2aqkjdhgi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2glduaftl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rzvrrvqv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2izcgdevr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wcjwccap.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2viopvjqv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hfjfsmxj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fxtdvidf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cssdyfiv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uabatdpg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2awjebqqu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zhabybra.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vporfgzb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hlhkooon.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2syyaozwt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ivasicnh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gsunljsn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ygxxsxht.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jpfaxlkf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hwtvnsvi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2reycxzhy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2btlgtaio.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2twrbntxk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rrwzvsfn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rjlwjduo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2euhzeyra.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mfscfppa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fywlxboc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pqlegztm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2tkjogdmk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yerbqnur.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hzedspyn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nvnixizb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tbxtldkm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uyheqamj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2euukmkvs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mwuhdezr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xzroflen.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ygpqotkl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gkwxguyl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lgzdtpbm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2prkfefus.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2duwmwywm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ucsdohss.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kzzwxbfx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2khomcuym.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hsgmcpwn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqaevfd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rklddtzd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nvdlaijz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lmpsvlsz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qvvmxfup.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2cnyiitqu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xxlgiurc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ikoemkro.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttumcdvi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ndszbgha.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsxrnvz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dwtkqtuw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gcpovbnd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pcbvzwyl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ejdddubb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ervlkfjn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ddgfbdfd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fuydotcb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rxmknpam.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lsgjgmec.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2fvniynfm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2glgcrknz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2tzlwmxuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urigbyik.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2iihkatty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbgsurcz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gknlvbag.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cboyimyr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xpcytfaj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gvewrdmr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ulzemtme.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xuyozfft.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cykyzloi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rxlhrifg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hibfrpkf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fchfrjwe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xopmlxpe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xaduudyw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2unrchcxd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2sujyzjoo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jmauuwic.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tnvnctne.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2rwwhttsh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lwmchdzv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jvpikpfa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zuwxvnol.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wposloju.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ijgmuhcs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bsrkvtmm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2czdvpzvd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cbkhxibm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zupmjiqr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2huziarnh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rxliuriv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ehfggfzo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2czthtpzl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tyzdphby.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hqddhxoa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jywhrgsg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nvwltcor.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2meypnkio.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qzfpammw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hacttylj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mpqbsxmi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gpkwtbri.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sfliqkad.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pbpjkbfv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2slyvgkqx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gjtxmjxt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bvscrkyk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2prydfbjl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pdviylgi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dtplfdgs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2eeqvwzbr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zwdpztcz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzkbig.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2acyvuohd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zkfggoqe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pehrkkdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwaxkczv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2fknkmtjj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2lqncrolt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heqqjxtt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2txrunutk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ugrskuka.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bjiyxazi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2clddiqrl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2sklejmgl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2khzdlhic.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wqcbsefk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mqtvryyg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2aqygeqtl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2fkqukhwc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qgmurwan.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dhwsihvs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wvhtuatg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dxlnyupm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2laawelba.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jcgdbfve.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2elliqmyr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xausosae.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tlcpkdeq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ktjrlgyr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pxgtwxhk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2bzphvrfp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2moxmzlsx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fnxjazgl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2udhfelge.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yohhdqda.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kljogizl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2sxylzyra.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nipnuwwq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xckfhzlt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dranvqyd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2adxumgdz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nilemrcf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2flvamozs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ddivdrji.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tmcttpsf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kidstmna.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bnexcxmr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hedciuej.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2npxrxtjb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvxeswqs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2aerhlsbe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2myngmpqe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wcofjzze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uccobbsb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2rbyvireg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqyqvhwn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fphtyosx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yfaqooyo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2onhxjwnr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xypntggz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vwhhjwzs.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aywaqyho.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2giejpbuy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wfypbuer.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2umpwfzbw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wogtqehr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vlfbzimo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rykstkqm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lmulhyoe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qgqfcyve.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zzaxppek.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2mzcyauxr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2viicqmfe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ezjvvaob.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lagrrool.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vjbumyjz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2exeapvqt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mpmpqnet.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iacelkyf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2otnimyqt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ctbxxycg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lshlznze.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jmbxzgwc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kzlpswvl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpcljlw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lblnpnrp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bmbrsnjs.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zhylubtd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2raiviljv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2arjtexxa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xokaswux.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2bmspumkt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2gmeqvhsl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aykisxnx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xarijyfs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eogrevsj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ksnxrzid.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lggjiriq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ttlkszhu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2apkjsgrw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xtpttmzz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2guxazcye.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ojpprvse.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2obnpqhxu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hglmbpwt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xzdaymyt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pijfjgwx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjwdygn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2czhbzhnb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kolvwxeo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2djpbqisf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ggevoidx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qywkdiju.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jcboxtii.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nosicqoi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gxoxucbp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yigipevf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zjyiwxsh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2akxhpcqz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gplwbidt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcedugx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2otezpzvz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gcoesvvf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ndvwpebo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cszqmjxr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qbmspbcw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2trvlwjra.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2koxtiwqp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lengmjux.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfohusjy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmvymukh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czkxtaaz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oaddmsze.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgqbrto.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2yoodyfvh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2peldyioy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tgcfahom.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zjszfyxs.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jhsscncf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2liooqaxq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqryramm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bmnouksn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hcyexzeb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2eohdhitw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ubreblyr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ngzruthc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xpwbmfuu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ijkdwsgw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vghgtiml.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2obueaikw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vqpbwhzh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kpikhipy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bmjyfxjc.html


<!-- 参考信息 -->