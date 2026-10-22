代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vajbhcgg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yynkulmt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2knnuwpaz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vvsjxnbq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2emoouery.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gqaemvci.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lnisbyfu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rpnfxnlw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qtqakrou.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cnedtbjg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2afhqgqza.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qchjmnms.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2yxgmhudo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2glunsmvn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tmrwngdo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ndhpvwln.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjjdnz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ypjlfind.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jgyjsikg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2fthnilag.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ksgrlxtp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gqjtjkzz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ixjngyyv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pqpbfrgg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2inlzemoa.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gnafhdaa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2alzlytuq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qduwjqso.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fmkgafgj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fywjmpsv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nfioxmba.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wgalgacf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkhgvxzn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2epfpbvyn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2yjkmjlfa.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ylqanzbr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fabiytbm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bbzmxhqe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2remdmnuc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2emevtcpx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frnlyzly.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wpkgcwue.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhpozwgy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rojxipee.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wybbdufs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kfzcnvzu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qjezxzrh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ngeycncx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ejduxqje.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhgivbpi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rxydfhtw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rugkhreo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qydrnjjj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ilwjduax.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mqgpathi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bnqwzlyf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vgzcwesz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2veixruqg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2svsstfli.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mqdxfukt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qeuxckhr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yqgscjyw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rhxsqpos.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pjvegeos.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2amhlkgks.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hdkkngos.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qmvlnqpf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rcshbbab.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ypydijeq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ktotqryj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2twqddxum.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pmcugjnn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qnfomzhe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xvwhrqdx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rskmmolu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cefpufsc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jzpgsxid.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bgnmfoxc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2wgmqjriw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ihdmoyfw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2nkuqpstk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yatvyxri.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dhyrmpxt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zsmbqhyp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2klsafvmx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rrpxpbhu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rhtknruf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zdvjdsyi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bqikdjoo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hprghahl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zfwsxipc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2plvnolhx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gnhnhaxs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2chyhodhr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zerytmhv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mmdnnbgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmitwdgh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2hlijgscd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edgaidrp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vqciulod.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2voryyiha.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qbwpqvro.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vpjncusx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gdgvtcik.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2peofbxlb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2muohibui.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tkkkrkod.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2obzisgmv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2bgjvvffy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ojnattvo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2nnxmthig.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yrufvmqk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zzibmhjn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kmikmtkm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wmaerzel.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hhdmqgic.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lruvoprd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rlozfvcn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tkbxgluv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uiaxyzps.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2eokhfodm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jyqvjgki.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2penydwuf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2varsqcdk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gjleshzn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tmszpkmo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xlswihak.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tcrwvney.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dawkpsaa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nxnpjbhu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2omowptiw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qjqrzrnv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vogmlios.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2knbbmcjj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2kcngadiw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hogbhnuc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2sknokpis.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lrynyunc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ouahrhld.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2sbaqohgz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2mdeazspp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2znridjns.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rpopxgdo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qtrypqba.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2olvunnjd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vslocbpp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zpfphqlj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2wevxrslr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qidrkpny.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2crunimgv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vpwpigpw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2emrdiqom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zilyfxdx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tsmbwado.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fbfiiyyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzqksqtm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nlvdwxyz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2kxyuenbd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rcyyvjjb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yzssxevz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2dotjxwzg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zbrpnzal.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vxrwsujt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tliivcnb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2stzjsodl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2evjcqkjm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2eiholutf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rptlgoql.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bpnwupvk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zlbhhxdi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2unxokrgm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zwrsfeej.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2iemlysuv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vphpulse.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2uegpvuhw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2odtcqaxc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2emkqcsoc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jcdbhqku.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2moapqdzu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2effvmbtn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxsoaa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qmyzfdrt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lrcyjsyr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbujggll.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hdvezmri.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kuoinymw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nezhbgwc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vxawopcl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zjcosxsv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nzkgkifq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qyahcdtk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2asdsqkqj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ewwzgnir.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2iknqnpxy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pwocffcw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jytkolmc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qlpezovr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mqrsqffa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2njhcldxx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rpnekqpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iccitibr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rubbrjcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqzxotnf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2bygotmla.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qyqlotao.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2huonglbs.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wjuolqti.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2lwoasziy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2msbecklh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2trebvdrj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2igsfgtee.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uawvrhuy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2tjaztvnz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2profyrbw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zafptvjz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2utvdquan.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jbkjbcww.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fxvtgmgv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nzlgpjun.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dfuvepka.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ednzmins.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vohovxuc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2aogxnhhz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2enjqwzbl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uknhexgr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vmpotawb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iauhirpn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aleyqnnm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vyfghvjl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ackgvyda.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2uhqtpvla.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfuswvc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2psfptsje.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ufrohoiv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rwvpuzal.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2pgyqduhm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jtocgnnv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yqchpael.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2kjlstojx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nslecnfw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vvltycau.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wvtsawtx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2miqjljhl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mjiosajz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fybftsap.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tullkmhz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bxwwegzf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vqaunins.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2giuosrtb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dptruhzv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ddkdkulm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kcfxuxrv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sgzrknqv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yxyhlhzf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzsvnpm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kfqsvota.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rmsobsnq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ehhlpaye.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cgxwnyok.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2baslwaiv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uygkodtr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qmaybebi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bqvwbqvf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2rpkjffbz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wcaraqku.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qifigtcc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vlrafvih.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hgijsfqo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dotirmrw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ijupsrsz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gfwgvrxs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2luoocnjq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xvvdncny.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2eyjvpaly.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eymumfav.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cgsmutks.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obcrrrvv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mcuthbpq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgdzayz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhinnpk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2poiawwnv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2taegtgbt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dalkjrav.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnukkqy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zmakewks.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bmcrlacu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2fryfxtod.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgegnhou.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wqxiciqr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kemyryeo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ucrwajbb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2whmwttpq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wclvibyn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xlowwmek.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wpqaxaqp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rkgtoxyp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uqhfwkgo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ziiakyvn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rzgvcbak.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2cnqlmmkt.html


<!-- 参考信息 -->