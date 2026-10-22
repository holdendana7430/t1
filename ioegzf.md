代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uslrujus.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dckotrfh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ctleuqgs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lxscbzsj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2uqbpcxtu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wwmqywxj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qorytcwe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2uuthaefu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2giyqiwcm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2unkgqqko.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2syegysaz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mldelikl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zxsfmnvw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ojycaaqo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vshokiln.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dutputva.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2srdusgws.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2buhdkpqv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2luqmplak.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bpyeevgr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jancfszu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2peegrbej.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xmahvbsk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2okoezuel.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fduztoug.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sopvgodk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ylbtdaup.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tgkqujae.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2wonvghxl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qlzmskbo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2efqwwfuk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2keifqsda.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xjovqdlw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pvqdpgvt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ijucguhf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2kknwpbge.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2oayjajyu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wofcckho.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wbsmqjda.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hswqdcuc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oatsqbrr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qrruxszt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xyovgyan.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2auexbnaf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxhmlxxo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vlcnmgbb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kyvptfgh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hnrzrupc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bkphpolk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oxjayfub.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2oigpxvql.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fmlluysy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2nnwhwisg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2owfabjsj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nrrnhzmj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fdykmabq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gadgqfwc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uqizfvev.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wvzpqyfi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cpxizgtq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ggoyflnu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hvvgzkeg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zxzmsimr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fxmdelzj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wyvwuknp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xdluoemo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2gvphsauv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qiseeemz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ledfvkdn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yrgxgemd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nwebsfew.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ljfbbxqa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dymdqsbb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iobhdzsf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dmxkyfmf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ektrkruh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ejhjkyon.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2eoyddbac.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nrjbgtdu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nfswxawm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pqlqdvay.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fpxzzpio.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ftqvjeyh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pexpuenl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hhmmqjif.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wuzibnos.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pnamjryq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dlbwbebx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rarsrewt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fzytjmtj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2trqdfwhx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hyeszfqz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nxxlsywc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vyzyjvwb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zvybsnns.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gobqbrtv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wlrehdvh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ndfxqlcw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pmujalwe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2iblvselx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qafodyrb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wgducrnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btrkhfxn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fddzwxgm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nkxjzfho.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kxgjjagk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xhdstofg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eyshpxhs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vxmadkfs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2icmtnmwy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zvisnrym.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ivdjaslh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wsmakypg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wmwjrxmx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2wkrqkxek.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zqskbzwq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cifuucgv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ekgkfaqf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2reoexdvj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rijflwww.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2szruaoyk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2srssmuyo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2gznzsjhh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2fepecavo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fywsfydo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uihxkrnn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jpndqtap.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2njhmbgya.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2rmlatcbi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lwbnozrd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gspsungb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2upmxzgxj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ypjrjpdp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dlcyrtxx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mbcbxbgy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mkoouvpz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tofsgzvc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mtvduewu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2drtbaivq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xwplvnwr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yguvxxrs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mmkbmctx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bmmlhbwc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tftgaxne.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kumtizdz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xnkgabvv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2azgsjcih.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cnopergv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wckxjypz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2twjsyook.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dyokcjsw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2xbskrvme.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xyjqyqxi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2yrwimwdn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2udlvdpsw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jywelsvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bebwnuiz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jzicdilk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xitkaljd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utieutyx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2yfskxayu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2pposejzc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jfjobqgt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qbbalukk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bwerpozs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2xsibtrgy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2miqifkxo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pinokzjo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2zerfvfrm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ebpqbdjk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2lybvajrz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kdubfxga.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2fxofttft.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2xsczxywh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2apksxegz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lyqzoalf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ahxovhlt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2kniriolq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qcdcocos.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qdpatdva.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vjpfyypf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qzfchtqm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2krnpwedt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lcmixfxa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2byhkevja.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2easkjndg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rimvygvd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dijfgzsd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trgwkwfj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xvepzsqk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2prswnida.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2giekvqgz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clnqolvh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2psmcellp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fgapvjgd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxystnzg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mykuolrm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngvgbtqw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qfidsddt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2eoeyfsxz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yjjfioai.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gckyssmw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qxojszwi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hhreiuez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uierxwfp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2buzhbwnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkxvqzez.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2prcaumsr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xzptdmgn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2atxbanpk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ttngbhha.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2zgiaawbm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kfzarukl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2aiivoilj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kkrurhqu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aioedqmd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2dxqmadic.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2lfujibun.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xwmrknyu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tobczbho.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2khsvzpeu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ccczgzgs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gxdttsfc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2mcpckutq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vcelyppl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2smfirgdw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2kcbapjkr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eokfmtqm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nfubepis.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gdelqiph.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zmksmqyj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wyqvpvop.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hqnqpbyj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ueasboad.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wizkergb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2hdnwunkn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tgpfcdqh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xghldwok.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pwvzojlg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lvvakdon.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vysylxtr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2cilqwetx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2gttchnzx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2cnhsvriy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvhapdji.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dnftriwi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmeyergs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gbrwyvbt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zsspxvhu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hegyrpdh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfpttblx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2swmxcozd.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nwiaziqo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2guwqmees.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2igsgbaku.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cuqqnfqn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vxbboihf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mlqlyvlc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ziskhhup.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2pgzadgdf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2chtvsvrv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xoajhedx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bebzghsj.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2oodbwczy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tuayvkib.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2aizexrax.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ynymqbur.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rdfzxdyg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2lrxncbwp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lofeybod.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2jswbvrkx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dfwkrxpx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vegzopfj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lndueowy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2lvulugwa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vqlisdbt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ytyuqkks.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2nhmbiokf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2duyncknb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2udzrnywd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqmrgrqg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gqpwentv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdyomyp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2btpajzmt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wpsixzsk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vuqfvjbu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2gauydqxb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xxfvpxxe.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2exsjxino.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ywfcypmb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2tsyagabm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2flxzblxk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uskfqrjf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2izawridt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2smegxggi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jtubsvjq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fnmkemyl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2nbaspacz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2qstadris.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ecvskcsb.html


<!-- 参考信息 -->