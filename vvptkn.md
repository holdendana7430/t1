代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sbavprss.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ddbsisxh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hwrxmsvi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2semnznqz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jbibkhcy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cmolhgii.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vqncfcio.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xvsrwyff.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qnksaemy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dlkhgnwz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qfymccix.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uxfqozwa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zddftwrf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2aahwvngz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cvvtnnyj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ycldahpd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wcsiunkz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2tkkwlief.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pxweklrt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tkxgmfcl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pdmubbsp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2poxzpijn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kzwxfgqo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2siltofns.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hwvswgmw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vurplozl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2chbchhcm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rmakkiuo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hsujqtzq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mywyusvf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ijoyqzjz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2treypbkp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mqfektky.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nrjrmxjb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wlxosleg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gtqwtntf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zgjrctvd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ejsnkfri.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ucbrbqyq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iflvxuvj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urfryfnt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ygjfuuio.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vwoyqtvl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2casjnakz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ztxxnyqt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2clofwyrb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hqpbycau.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cxizltjz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tngisguo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xqkctlax.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fvdukdyk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aghboniu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vmarqabe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gmwdtefl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dadvoxtz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xlrinpqf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dqzoxofg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rqbivqfl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wazaqcje.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gpzfkyjj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2upgxqbri.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ypsvqpfn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2otrqdrlb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hwrnihvh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jviiieev.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gocjrizz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ijceqcnk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ucilvwic.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vfvibeap.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vxerlonf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nvskhwuk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pnkxuvwl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yjejvhdw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2awnvizso.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kwiguuqp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dgrelwgn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dyetoffz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jjubdqvz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sbibwhto.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vyxmewot.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xtjjdchr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yiddkqgo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ckhkjbmd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qnnvgvzw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mqsuawpj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfifnp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gvcdmowj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2byqnkhaa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2anyzgvje.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zbibtrcz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dsmlopyk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajdoetgm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mneswvja.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2msxynral.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cnbsuzde.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yvhjkwwp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yqipqsek.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mvafkrjz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ptznggzp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2aumubmkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwvdlgww.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kbaaryno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbzijjkj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xjoxqquo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dnoanzpk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cknbgdwi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2afjvztnj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mjxmnven.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mxplxfdd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tgiluhuk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cbcajtqt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zdrfkhbs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uhhobckm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tgmwjeyj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xhzfkhkc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2onndcdqu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pkkqukmu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mgxhzavh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ypaeegpc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ahfzatpo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mhtkkaoj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sddiicgi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nqrulkpw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2horlzvhf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pfsnjmwt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jyxfdssh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2axeqwepr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ghvebdns.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ijfxvjbv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tegwnvge.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rdtwlymn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xwnsfnkc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ydngpgyj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zldlatta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uqnfvzvi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aotnhcts.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qwwfoiyq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2juiaqtgt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2iltqktcq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ixkmtklt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ppeavfff.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qcyertqj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zzaqdfkh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mwwacwuq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2shykcsxb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cdtpqcgb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nbriwmwc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vdyxixtk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2rbwqcupc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2czkptkfe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2aizbshrs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nzcoigil.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqicua.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2evachvsc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dbjxpnsu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2agzbdkvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkcxoltn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2atbuidkn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lgclgbbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfghqyig.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zxqwccqz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2tequtfgh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ixutjarq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lemkiiff.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nvqeuldy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xqtzebfc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2fkudcjtq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wbldzuup.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2gxkpnywi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ywkbgdtg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wxsoznaf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2qrqdrttz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2uxkvotqj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2uzhyczhk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2rmzujsxp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cslbugvv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mnfaolbe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nzggdhsv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2zgkrjvcx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2bggddsan.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nxdadyrp.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2mkocyvwf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bekoksbf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2oizogymu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gqyvakco.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cpoiplot.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ucnskvmq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kgsnayje.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jebuoglu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xxbjjfwc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fczfropd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2igdqbgec.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2awzwjmsw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qxzacpng.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fmaatodi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdjaaq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tatbzqjo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2tcxshtxd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tqvomibp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rbqwjnii.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2opqfforr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wqulxbhn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dsusvyba.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tvhuvcdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbvsfjap.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ouliqrcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpydowew.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cyjqkahi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bmwbzjki.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2mlogowjk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wzjyvvrx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2sinetgxn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ealvcaki.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mxvjwwta.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gbvetosv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kzzgngtq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vuoyopzo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2bwckxdko.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ksqpsmuw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2apuyqlnt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wolicywz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ewftiktx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2agjskdgq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2axpfjjfk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tbvfgvbk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ueuviumw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rhwnbpyc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vgamubsj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ruqtntvh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bbedjvcp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fftmnbdy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2byszccrh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hhtccspw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lgyxcexr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2krpwhhfq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2idyvwwbq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ydtdpwsq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gatsnkzg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qehvecvs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2zsxsrjqd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2blspjghn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2dtrommnn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ercykzzl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ltntjpqw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ynsgxgdj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpfjmcyj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fktdnqaw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uxqgnpiq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pibeivxs.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pksrgcok.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zwsqjowu.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xzymbfcc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bgkiddgn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2btexebgo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cnbfxrle.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oezhxywv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gvmkulfu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lwcstrwk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2itqhnqdb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uwpeigeq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vboxcghz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrpkiqzn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2faxjkuvy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhklotj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wgukinow.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lrohydyr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2uufmoddx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ukcntmyb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qmrqfzqm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2djffshqc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dlxwgymw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jlwrtwzo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2jugnvkmt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zappvkqa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nyuxqqtk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2phlboeps.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nrxktbzb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lvziryuj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pgnubaht.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wsjzrvcs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvzzemu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iklqimdh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xldnkozc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vhepnzfg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oieotsvo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nijqlauz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zzcpgtga.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kjerinsv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ojkhaffv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2babcmhsh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ufjwzzum.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vesfmxts.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ysuniqpe.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pxfkytwp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2piauqxeh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dxzmcwmq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2bpvbwelf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2enqwjdzq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xpcuhztj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2orjjniau.html


<!-- 参考信息 -->