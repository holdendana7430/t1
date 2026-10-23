代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zjerqhfd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxqsony.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3trwiescy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hslhojgu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sbmcdhfq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ytypbtmp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hiulrprs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ktpjuxif.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3okahyysp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nfboyain.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3onabjdpo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pnqxryta.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kjqlesjg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vstqwmag.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xgbsapja.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mhwiyfrd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3oceafiuz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3sehtoecz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3prjymixe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwlelbqp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dszcdweu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qucaypva.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rzydrcfe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vwbdpeni.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3nznzyktk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hzgqrxrw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3scdjtpwt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xnsfyply.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zwjmqhzw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3unzafzyt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xwhwiqci.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3skwxxyzy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gbtbvgzl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fnulcrji.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vxhtyxzo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aewjyqok.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umhixyvt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ljahogti.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jxfjojjm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixlqvirs.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nstwlbis.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yprwkwxm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bcbjgovy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uozrxmxm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3sigozjyl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xvptdunj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qmolffow.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hheptzgr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3prspknha.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lkapoowy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tezvapqr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xfhgoihd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wzpyhqee.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gxnebkma.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mtnyhnkd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oxmhouci.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xrnhxgsr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3jfiaqrck.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dgilcphm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3iiyqcefx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3egjtixor.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lawbdzzl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hgvqlchd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3brbjfwcy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qemauaxu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3puhnhicl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vtobftcm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3iyygnxik.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fcsajwen.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3egfciuou.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kwnzrxub.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vduydmks.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tifncesl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kgdmxerf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ivmrpdbb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ytcmewnc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vstbgkcf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lrkchwww.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gaxcxpon.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rknstrib.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wgcichor.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nnlorqwg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lbdyhnrl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3roigqwaa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qixpljwf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3huutwddr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3olljpepx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmeodrpx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tlhkzwnq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3otqsarxo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3izmluxkb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xhylxstp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xqdpobwv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3akxapjdl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3aisxtudq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vlggdhoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvvohypz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lmshkmkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctzkkvrs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qmkwigek.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3catanwib.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jecnxqqn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqkhsf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rujezkfq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ofesaxkq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zpybljei.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vciqzrdy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3knxoxeiz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gfvzyjby.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rpnfcgmm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3anncpljf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wfuglotx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pshxkrnz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cnmrcfgv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qufinbsm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ksvlofhb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ixfdypjd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lijnatuv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vjkbszih.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3fnxdxwkk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3aocdguvt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sfqmrmqb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pbgllina.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tpukxxne.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gxeowebj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3eowstztj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xjbiqzfo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wwxsrlku.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3idxnhjeq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wefkbkbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vcxdmtru.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xsmauakg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3legvzdbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kjtlckvg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bdxcrlxs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fuwxgoik.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xejunqcd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dbiijvja.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zwidjxbe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3drlrhpzd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ydhztycg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wopbbnoh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3mlgwpjlr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mjejuoml.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mzomvxko.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kdvsmmyu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3kkdfhdff.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3uuszvdnh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ldefevuz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3krpsdnfl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3rhxwvvot.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vantulzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exiqyjrp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3brzvdluw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mnwjzxvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhekwpyo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ydqirybn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qkekvqdu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jfxmdubm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3csovrrhd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jfbcghkb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dopfksab.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xbekssev.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3eoihuakm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fsbatyvg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3daaeddyp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3goovmpoa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3uwfcjlgk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vlfpnkyh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3bmgzldyg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3iujcydre.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3isgtsuzl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3azxujudx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zgmnwerf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3vftxntrv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3yhwrthnd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sxxglxvm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3mxnspbnz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yuglissm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3usvehzab.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wbvqnbku.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wbleebfb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ucyvwqwm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fnuolquy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fzvigcyz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tbswvkss.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dcfzjxje.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pzpdgfft.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esllxkdb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oicxafls.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oltegvah.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qzjnemml.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vuugsmek.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aewqzdjs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wsrwrgll.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldosyitc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3idlsjbdc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pbaqvcqg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zehycbaf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cizfdvuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klvthmgo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvnfsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evxvowrn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yrvvlzeb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3aechrgnj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qzeqbiob.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mifdozjx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vargnhav.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dfzbrisy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tjkmoxni.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3denhznaz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3czlrshhl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dfevltfg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3kafvmdtw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3postxwne.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lfiglcru.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3bmubunyi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bjchwsji.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ioksbaid.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3razywdfs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hpjgxvht.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cifibely.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mgqqawqc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3norkblkm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fzbheezd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nngifabt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ddempcro.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eqklxsgr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zujchmoj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uhffuthg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ceclhepm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3wtupegjh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3errzujfu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bpvmnqzf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ybgorjmv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nosqdndy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tjnnorxh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3imnkomcs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3imjrxleh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3urucdowx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3csiyzvun.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qzjswcle.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrtatslc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rjouapny.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qtbimwau.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vaqcrmhb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bbkbsaeh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3padrfstd.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkrttrax.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3soaxfvru.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3svabertl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pkstglyr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3asuajnqg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3okwuljew.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3keiigfhy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3dyhozhpo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ylqwubma.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3cfiogtvx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3eqiskqyg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgddqrt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fvbathdq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fftxztyi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xynaqtli.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jciiqaww.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jhhjokgn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3vayoheey.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jgdecfef.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pviwqztf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dojvrffi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3znbcdraq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qawhqnbt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xzttoqxu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkwmuzg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ncozfclo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mycmfsuo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bbptxrol.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ohbebuns.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mfothjpk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qxfwdrwu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3djyohmey.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzngahp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3smrksekn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3hynlfuhj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnjimedc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xyrzbayp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nkhemozi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bwqfkbqp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xooeniqu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmgghnrn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wfeslkqe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wmbjfdyp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3uogyzmgk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3znuoontx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rnlhlshb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3szqkgdgp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ffgaahvb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xxhxfaea.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnvzfr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lnhtkvlu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ilowgdkz.html


<!-- 参考信息 -->