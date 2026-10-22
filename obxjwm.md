代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hjvmswox.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kublohpn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ijhgvzne.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fefnlrgg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qmsclhuz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2soroxlhg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wfckqmjy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zorobnyx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gbpllxig.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tkcmoymk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qxdwisbk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jzeyravq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2trvqdqdl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fsgfagnj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2lgrubets.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ealppdvx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tfjcjxbq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jvwnpxeu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ymhwhmzd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2azhiorvq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ycpwjoga.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rflyshte.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xlzuvtto.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hxtxlqhg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2djzsqqds.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qspcyalk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pessbwst.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tqiuganm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qawyzgtf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqpzyqcb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pdikjbbm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2glizwavf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ndbuckcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wfjthseq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2guqtuwlc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxkdoqdc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zjakgmlg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2blkrwozm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzxcrrgd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2egkemzhk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zdxpagmg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vfautnyk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ijmqtyxl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vvvqzmbr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hlcfjbiu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kkcdpyyh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ocxqwyim.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ticlozwu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2emtdijyn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kbokfrns.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2swxjksuh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2swlqdvxa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2cctjizvg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2njtxbhrv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sgmxkhzf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hwoteewk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jvjgfjct.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nkmtshls.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rnxltyzb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctguzvem.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mujwdqsu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nnffzphb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2apexaojx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ybguvsga.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mrqhzdlt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cgarfglx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jmhlvwds.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xudmfiot.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2exnkychb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gbiqgkcx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2poouvxws.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fbcszwts.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2orrxrtzg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iyujwiaa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2texvqorx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qofuqmgp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cgqlsiud.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2requmlcq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2znnzilbx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbjqwgrg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2akuartsv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lxglnpkh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zhsljvyn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hktmnkog.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wjxgzbvy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sovjyjlg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bwrzpboi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2shcofhoe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dyalyxcu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ehyxxwlw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ywvpxfjv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wycwsjod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vesuxwvl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2efjrktky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2actqmevz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ptjemefb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lajsvftw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zvbbxwge.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ircugtat.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ypnfixgc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tisrxtnx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dnjpvaid.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kilmxxbi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zdlsfnih.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2hmpammzt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jmjddwmf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ejepudyr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2cjupujhr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vepmrpdb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2gksyaely.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mlgexllg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qtalaefo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tdyhmszp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zywcybsr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lmyspnmh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zuyuaasw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ofeiejho.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gmcguteg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tguiokue.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mdwkbuis.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fwodnnbh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ipqaefpl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lhaiohua.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jbapaoek.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rrzyeouq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zbfkzmhe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tspncoig.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kihxpwev.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fwvhmtzy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wmbszcqd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gbrubvxe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xjzozndc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2czwsxywn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2kxaawosh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tvaprjbl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cprktuni.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hifgoxvy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vowghqhi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2aipezvfe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lcieogqj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ecprastf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cpiuvmuc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ytkeyaxf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2yviuhzll.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2guwfxfgy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2sewegwdt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ieflswpr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ubdmkjdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhcbisql.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qiyuwoso.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bkfapjig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucatdzhi.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2liukzaqp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wrqolhal.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rkcltsxq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2yxfdffri.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2dlexpktp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ubgtyvsw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2raknliha.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zhrmkkfq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2magyeskb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jxevfjiw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2dqtludfu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vubzirsm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2zfesehjc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2oviumohp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2copjexru.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2mvvzfwem.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2uwicifon.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mtjaejdn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2lifzzvrn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2kfwpigtw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ilfpwayd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yiyhtigo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lheclsqd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnwmdwcs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2oqarsmjc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mxvrlwmy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xigxespb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwztkqwr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dvalckcz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2oasmhnxe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pfdcpuzo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hwrilbdw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xzoestky.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xjelfvox.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2irfhsqgi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kewfaokx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ktavuqok.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2asfqbjze.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hiyufpld.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2sgmaxdmk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ftqxvmyv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ycrjstlf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wsjldkln.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ibkplavb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjbpuzdy.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hvqezudx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnbsxlgi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uzgeorbx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ezyntyen.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pagxvxhf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lapjdepq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2gtrcqmsw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zmkcgyrb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2thuwizmf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2izwyjndb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2guykkmmk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pzdwepjb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2gtdrqudn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uppobmrm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2leatqofc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2thtskbqu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2slpsaabv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cxgllhtw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2vloskczl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hferalxv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hctuaije.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2slahrzdc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rxmellgg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2amiohofg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rqphcxty.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2muutmxhi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2btdlaixi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rcjpkans.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtmefpwk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2tzmmzuxl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pqkvbpwk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kbcczmzb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dsgbnkip.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pvicxcrm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2pjiqnqxk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yrxyvcts.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2diqvyjtp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wblgffgi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jkyyqrym.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmnugjsv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nmflktxm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2spvdtqmk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2frgwgxak.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uwumpjhk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tifuscnt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iixhttzx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vuxlkzqm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pmuntntr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ttesdcsa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2limrlfjz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2oxldvuio.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2utmhegfy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxldfe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2rlmbkgor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qnntamko.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2etywobdi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ggzkaruw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2dpvegtgh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzukxli.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nxodgpsg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dllsitxf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uidqzjxq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vusoqoxw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2suqwwrto.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2jsysyrxp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ypfuvuwh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ncfooezx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2uynftydc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2avpzryqo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hfmxploi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2whnnzdxi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2codfsiip.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2tsedlpzp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ddaucfys.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2prmylbrz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yzefsjuy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oltlygme.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvzqsyo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fxhcaago.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxfvnoaj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ikyamewc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ibfhnrra.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cvwmschm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qyepwrsj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ypeimhyu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2raylpcoi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mjenpjpw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fqyyignk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qlfbuhip.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hffnwiub.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hrincpwm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jwjzlrcu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ywzvmyut.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2drnrqqmt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2otzoamvm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dhjwyyvp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hiahnnjc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oiudikmc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zyroxiyk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uubtktvm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2llujmlel.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bgwqbzrq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwxqkqwg.html


<!-- 参考信息 -->