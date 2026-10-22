代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2skhwxmiu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wkctxktq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cjveiuvd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hlgmptnb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wcewsjqb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mwrjbeip.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tytgfqlf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2sftysnut.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wzmahgso.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kynpeuli.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cpohzjno.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dsowbagi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ebidwwii.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmehoax.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kebeenco.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dlmhwrim.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2nzwazxqu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vlrtdhpx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gnyzljdp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2anmzmaid.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hcqoxofv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gpeogqbb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2satauvnl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2teezahsg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2imcnaqfx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vpzqpulw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2iyaudmmv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mytrhevb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pgviyumr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2mzkjewid.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kokxrrhn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tukybozd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2yzqravpu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uwcpqahd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ekhqsptx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zcvgmhrm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2yrbwnzjm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2axgqebaj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2crorojqr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tyacmdsa.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iwzptmxn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yiqkksrj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uibqsefj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2uolnwykt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mmebfoev.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aguhitlb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hmjhlffe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xdulpgbc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2isjneijw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pfbpvvns.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2yewoquuk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zzlrwluw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xljcangv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wrgeovgw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2octxuyxo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qmcledzt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2enkgxrck.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hlweenmf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kqpdbixt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nxrlxwmj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2bhwwyqcn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hkbrhmii.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2quqicqjd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2emidwqpw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ffxmunkl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2utkkrcbr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kpavmckg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rsrvbumm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xfhwvcse.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hsfzifrp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2arwxrmad.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bzokfldr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cdszmhxb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xmletcqv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2amdkntix.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2krcawwvp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jzidhbfm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2huavccoh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lrybjwkq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hksxoqse.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zflbmyre.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2swqkwjsf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2hnyqmwxo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qecbqzqu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tpbhjtke.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2khflsovy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bysljwur.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2blookyla.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vpbtuvtu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zjomicmz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qcgxenin.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2woucvlcv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2epigcyta.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2roncqagp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fxcpiztp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uosfmlcx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kqmqpvww.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zgggokwd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gyibjeda.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkobuaho.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iyctomeq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2howssxyj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vknbuamb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2aepkgkxt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yxdcetlv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lfudxatm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hnbniqol.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kjpifljb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgmutqtn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vnwchsfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkrlxxhn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2plborbuj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bzqxphlb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mzjwnwfo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fpnhbhbp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ctwdjnku.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2khqvznau.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2medqxsuy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mkvlspzf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zbwyoiii.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2gqaibifd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ztobvidq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jvwgdgae.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hnjcsvup.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2adetyvoa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ahsehffi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2sdooofqn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2sigicztd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dyldrgvs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jgdeaocg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2huylzwcd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rvupkaol.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2unnyjnyu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qstpjqlb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ymabfoqg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2irqtflef.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2tiyksyob.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fcctwwrh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lbaksjfx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2syrkoawf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ivwkiqhp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ixhobutb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zbztitdt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eyzxkbkq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fqtcltgd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sabdriqu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2irilkqms.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hbkcxjzs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2jxtldurs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wysjqlbz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2owttwrbt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zoxsynmd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcbhhe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xeeqsnkv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2oiohetgn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nnewxdur.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2inaqozae.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tlvywpxw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kwfsuouc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2soxvfnub.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2mnkulpot.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2fhyfybap.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vdnksgti.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nmkpvanm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfovmzzi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wvhszyks.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2goesdkhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lndafnnl.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kmzucgza.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qhaidtrv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kiulzkjy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nkuyavcx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2cwmvglxx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cwrdsglt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2acozmhvm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bcjbyrri.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2litbqhoe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zxuagcul.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2olldvvnc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2izinuiyy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2colqiyqr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ogedgnvh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lwywgsny.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nroauoni.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2bsjmhoav.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pvrxuygd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bmbxpcla.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jvsfqacr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qsmaodlv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vqdyzevy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jtmxktfx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2azmslscc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vdfvrjag.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ezrwrnzr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nalwtqbp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2uyrbenqv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eoinkpgi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjpbaziy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwlwormm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2drwkrxrv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kcnnzbwm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ehwgyqlh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2spnhzjir.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntcdlwkc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2csdaqujr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2lcqqvkdd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cyxantzw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2zmdxkeed.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hhxsnfin.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rzddwneu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ikgujpdw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bscftaco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rexplufy.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxjgbmfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vamiuehf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxqzlyyq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2azxlpslh.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qczouusb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2apxvnswu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2feqquort.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qgaehhtb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vgwmioym.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mgftxbzq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zbwvtyel.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2utllwpby.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2umgxpphj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rzcsaxma.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mvetplzd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qrdyeepz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pibpuvst.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nhtnhdmj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2anebmhjm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xyxtdclj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2mkkzjegc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ovecfmwg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rprtzbad.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qezfazbs.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zbgzldem.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2atbzgdgq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qpggjghq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kzmqdxvk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jbysjczb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fedyjchr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sdsxrxkt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssotalkl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2moxozucm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lcbvonqj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vxoizmay.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zyhtuaku.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gyygmnmj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mcddhnhc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2lxfqbfyc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2utdgllsh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yzgxlxpw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xsmoaqui.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtdsqgfm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lthbstwb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2abdhqsyk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2projxdqm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2onfvpsnz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wlwumket.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qrkvdbff.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pomytsss.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zgnekunn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rplsbqyv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hzsqlofw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2xyzezbvg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ivlusqwo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oybmjkqq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tvlcibmj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2etyqrqnt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2whjpohgv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lbyksxay.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hqbyvfhv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zcozzlnn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gptqklgy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2fkuezudu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mzjmwdyd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2rwylemfo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iwznmaem.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2icgezavz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2djflhvlj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2kulnskzb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2blibiobd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ivosqgms.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2hbextwpr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jrbtkkoy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qaojkarq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qaccqltb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qytvphyt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xoctehgu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwzajbz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sftuxaxg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ovvtaepf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2nsrrabdu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onyvvjik.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mfmriwwh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xlvevtxq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kyrqtviw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2celhgddi.html


<!-- 参考信息 -->