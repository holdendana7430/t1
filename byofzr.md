代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xgpdifhb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cbivhqkd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mzfqaezv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ydwmzfga.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xxzymrxx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dahaeenb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ejphigzw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2tjjjnjxr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hckvvlnm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jdzgmnin.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2loucqqwo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2innmbgge.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2saoutqto.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oksmyjtb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jfqikqrp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2oslyihdx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2guqaojkh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2amceldga.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2brddldrv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ngdtajdf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vaenrhkp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mlnyvago.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ydkymdkt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tzbzoiyt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cgnktgub.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aqyedgjb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qpzzkkik.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dshhpoop.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jhriyepf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2iyjusiau.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xzyvwrmb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kcgxztxx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ahodacon.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zlqhhoiz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ahplwcmi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wfodfzes.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dlxngnqp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qepayhjq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2etqnlfun.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2akyzcjqh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpwtrtzf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bdvlsfwy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ftcsaffk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2llxmzbve.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2cupbdnwb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ivtxgrqw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fzuqdsxe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2glqtzgvw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2coglmwqd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2epvfqnpo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dryqgjhy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ouokfcnn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ljvdpflq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fxabpklm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vwuuzhje.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vlxeqreg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lhvhduqg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2sclrnpeh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xkzmsuew.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zlbnjbaf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vjptqnym.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2aumntssd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pvbzjgfw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dvqxhxmd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yogmgysn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2okqyxcfy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2binudcep.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hmagvczy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rlnakdiw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pudugrsh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dspzjtms.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2bmjippuq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rofgjdqg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cegneaux.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hlqfbcbm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2sgrxwnoq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wotrigsl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lssgzojz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2oyhiaiyp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ypkpiosu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jodvmqzk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2awmnwaxq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2oqqsusub.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jgoytgmn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rsfrfoxy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kbvtyqje.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ykzuzlrw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2quafroqt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kafvuuqe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2glereagd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dbsbwptm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmrenvzc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ywuodjvf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mqgavjtk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2khjttubu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2etlqwwsg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gcbhwwhu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bfkoxsqm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2uzulxucf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mlyaeexb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tudmxipx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2nftcnadc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgeslzkv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2plkougzu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mmmfakux.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fzsxeqjw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ukowcogx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cqmwkryn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2znsgbfaw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rgyphxoc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jsvockot.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ownqpymu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ijdsnayx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pgmtbafh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2iidqtsii.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ovydjrgp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mweotpwu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ivyletqt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ejtfntzy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jgvfamfs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2uzzfasbm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yuqzhlqx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wnmlipho.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dijjgnow.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vgrieain.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ncyqttid.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2iyozagfm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2eghphzos.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wjrzfdrv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ljfjenaq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jvxaoytu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tdmxmfzv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tgraxzqu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qxymyyqu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lsofftwc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2otzjwkdw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ajgnckce.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mcbobqhm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2cgigrtjv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2shygrdji.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2klqmquhi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nznyvmik.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2efegietr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xartytfr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2npnfhbbo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rrxkiygy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zzoxehkv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nfmdkleb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qljfrgok.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2frekeopl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zzwikpub.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2uwmeiyaw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2uorientt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dnisyzfy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jrcspbsb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2oxpemypc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fudzdbog.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2yvqhttnt.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nwzblvny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gedjmeuz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvcofj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dyyetxhh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2xsseovci.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2zzqjwbsk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ihabtlzg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wpsrllnc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2mrkxiudc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2nfacrbtx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ogopdejm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2waeabrds.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2emcipmng.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xjgvhfyy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2mjmjxelm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2kylbzyjt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2wtgbgbii.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2upvkfrnr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2fotfhhbj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wgxszges.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2cozacxeo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2thevxsqz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wcxxfbwl.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2dlmhtnio.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bgszvktv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fgobojsm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bbsecgco.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zwoqptxi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbxgdmjs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ylkmyjwk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oatsycec.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ijimokbd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntpkoiyc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2shmxomlk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tlavlqse.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2julrzdvc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qzivvenh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2awoilkbs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ngsjzidm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bhfohxjd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cdzlrvjl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hlrwtkkc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fllpqtcc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jdwljwdy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mgdorwwv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qcgrfvpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prayuocr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxkacrvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umswjsoi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2achmqsni.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2uuhbvclf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2amkfbxrq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hbzgudxt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jzctosuj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hwrzfrlt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2agverzlf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hthjagyy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2epercnrs.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2whwhkceu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2czggwtxa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tnwmwovc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2njntutgt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tgijdpdj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qcihvjxz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ijgxyuda.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2crbzgegn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2divvojtu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2odlmivvd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2erfeqjoo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lximulls.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rnlvkwia.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xkrwjbsd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sebtpefp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2eqlptncr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vihvlxrf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2snoijhmd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2auavgqul.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2scfuhiyh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ankdukyg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qyydajkp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gkgjlnxc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2yqodidyc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xwsyhrwr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2bqpkfqdv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2tgxiwfcy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2abbramsy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkfkrqck.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xmrvhoae.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nurtdnnd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jgobzxeo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dvwesmid.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tclpszzk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lmbiikox.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tqwcdylb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qhqudcjx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nojegqvu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rhivxjrj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lvvfdmsc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fmoyxzcf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2snxchhmt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vwztxvaf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2kdfqtfrq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jzsvrvek.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ecihcumo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fpxsihhs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gdyvqkse.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nvdweihf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ewzrugta.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ilebchlj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2jkczvlue.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2evqlqyfx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2yrdwfwyu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zzcrfght.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2owgjyfnr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gvivzksj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uouwvxso.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gldthxue.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ocsomfwo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rkfwiwcm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pjnkizqu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjgqzct.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kynohsdm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zubuooby.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ktgirray.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcxvafg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wvceshdu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsuzbooh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wqhimvze.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mlnslexp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvwwryqk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bucnwmnp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ipnkdctr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xjpexpsc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wynnebar.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gxklnxba.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kbzvyuir.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2tolpylgy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2sawvzdip.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pglcmlab.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2fqwvditi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rnsncouj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zyvxfnbk.html


<!-- 参考信息 -->