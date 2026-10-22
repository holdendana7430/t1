代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2urooasuc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tresqqcf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hqiojxni.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2spahllqh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dzynpaek.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rugvtaoh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2sddwlldl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxqhtjr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pbucwkwj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fmuflsxp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oaxqcfxy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qmxozgia.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2tubllhvj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cjmkmjqc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hnareqxt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pzyibqsf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2iyrnemmb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dcqrxieq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jbkhewdo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vfmifaik.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tulsiand.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lhwyjwex.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2izsdlwjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vcawtmop.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jrapvjcc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2obujqvpr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gthfgvmb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lttsnluj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qfbwrqvw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iidxijku.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gijvorul.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2oahbixag.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2otugeqpy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wxgguwqt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tnozbdof.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gucyaiuk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fimsrghq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2efpefasr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ljuxwwkf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wwmdxyfy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yrxudolj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yygwscse.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucpfrexv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxxdmb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kgcgzipn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2drqrozhv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xdvlcflv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zfwdiivf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jtwvyjsk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2frburzbq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2celfkndg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ogatxvzd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ndbkmzlv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tjtpcjmg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xnfhlwdl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ximdssip.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uovnxxch.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pjdhcvia.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2aoticxex.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ooayqieq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zuiyrcbh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wuntqruo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2szohgowa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oedbsyst.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2purtcgfr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kzhmyjbv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nynoslwc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xrdbhlyp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hsjbiabw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qcevwiov.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nwasaiun.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zxrnuplq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fezdkeyx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qaykiwdd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2egwfvzon.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ycgzczdb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wfttnggm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2yplrdaab.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zoatjcds.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kipeuhep.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uffaeubx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xzzteyez.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xqgqzvtt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iehdtlkn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2apudqrrv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mcfvxzkz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2spmzzmkf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuqxivfg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pojdpyih.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ylkiqwgp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tewuegds.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vbptqxjl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tytozhqx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mrkqiftd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sygsckfu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fmrzdjxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mecazplc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kxrzcivx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkrddluf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2srweygqs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2phyuzrnq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ljhckwaf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fovdhgzs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nwhyqwgk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kjukbyhs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bskhyyjq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rdjzmgwu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rxuhczds.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qpuazpuk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zxmreydu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pbxteghc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2iwelfzjv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fveyzoud.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nlozaeuh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ykrephvp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2asgwzymd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wxjzskde.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tfcwpxpx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cjebzvjr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ixjmikvr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vkmtoszw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2haxlhytp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jgfrfubu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2oyzhnxpr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hjswkpyx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ruyffcdq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uwsylmug.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rjrptnrr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hchapktu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yhfvuesu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lkiairyz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ezwbmsfx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gombgqux.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2atpjahfk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ruxjsidq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ktscnxff.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2pycvkboj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2uoqgydjw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vhiwapvv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ydgmewii.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dkvukdcs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cccwljax.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qobqknot.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tzsaalpb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2noihhqwp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tauvqyyc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2iihetuwz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2azhghllp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2znfjfjkc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2vjlqfvta.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ffdadxup.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pwmhbmyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxfdfqes.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2sgvykjgi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wkixjkhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwsvzrzt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2pfvubrgl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2onebxwcj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nrkfnbud.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2jxrqhdhc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2unxlbxuo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lkxfupqi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2svpxsajt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2avtceybn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wufqmtcp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jkjvdvgk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yvksokuc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2pjpffxwd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2smzjusyk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2htqshksp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2phisrxht.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mnmpsuqm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mvyztusa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pqgqhgij.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2sygvqvsy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2cjbhyflt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ujzdpyrz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2smbxlzys.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sqjhxrlq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ihxxozzd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2htcurvvk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rqjgwilg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxegxfnv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nwbulyis.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2byyjchcs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lftmmbvx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tcunfcjc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ghkzpfli.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zdifinyy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajqgilqp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ctevhixk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gufvxxow.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwizrsvu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxlukmxa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aycumbjf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2juhybowk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ltvfqqya.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xdqukyzm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2chjkozpd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvssjxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcgsegst.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2yuxbasfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvgtfaer.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gkezoqhg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pfcltgvn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2atvjikrt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2riaegomc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wvfvdbrr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gfjznxqc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xlvnumvz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2jcasbpdt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nfrvpohd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2txqsrqgj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2olvhqasn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dzyehlar.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xhcyswqo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2olnzqbmd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dftlqkch.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jpipkfnu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2uapcpitt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2awrlcpfr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vyzgdngy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2hinuwtip.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ifwafznq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gwzpblhu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zeslxonn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vkwmbfnz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rasnbkbd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sjnwuumu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bzpnqeny.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mdqglugz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2avxpepas.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ddwanpue.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oiebijnn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nepehbmr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2sreworcp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dnavnfqi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lbknjeqv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bkxfqmri.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2mjqhxvgd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2msctfgxu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uflidxnq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vbhlztrm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jvdtsvrf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lpzdjyou.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vusrprln.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ugavhgti.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cpcnfkls.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fqslacen.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yyqdfaqr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tqvsgwkl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ksvtzghw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wgvkbfce.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qvcjtady.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qyxggurt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2tqsatgju.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yxtafiuv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hudaljpn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2oracudmw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2tyelbkkc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2siukmudg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uxtokewp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lzycovvh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ofgouhcl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2hgfudbgs.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lstiebna.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cfvpobjs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bmnfoohr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivthjmal.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxiqzyq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fixbayug.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2slcukdmv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kclkcjii.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2dnnydzve.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnezkuae.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2twrmuolv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbxachwc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmsmvqrr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxdzsca.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qonmveuk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvilszhd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2zntuhbtk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qjcpfngp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rjmiiwwu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2aahzprhx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jfzvmqmm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xtunlfzx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hppeuiwf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgesrlnm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dtrzucts.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pjmaqelv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2jqrwvkxb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vjcxmuaj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2lcxvfauj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wwzbtxsf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hxlpfexd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sdebvjdr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dsoduszo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nrewxqxm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2cpztkxuj.html


<!-- 参考信息 -->