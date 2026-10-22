代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vwrqqjju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tuafwnwr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mxztxkff.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2oddjsvfk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hodufrzs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbrgpbzg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zmdqwsga.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cnjdlftw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2etaqikcu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fmvgeymd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jshnmhqm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tppxeyir.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hjujrnvc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2podwrqlt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhzkklfm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fxboiykb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ycvcaaei.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vmyjnsjk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tpnsuaes.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rrojxvgb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2urhcjere.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ckivzsug.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eynybnrf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2etilgkua.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zbsemlyo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kkoohejs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yskkyprt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2eyltjpea.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vtozmxpo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2cvqstbvt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pixklqtc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fqljfdbh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2sxgfapys.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ayixuhhh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2zlqvimgh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2evtlxcph.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jcouvspd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dumyzmsl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rmqxyhpj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ufbyazbn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cswgumqc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jqkxrhow.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ltvuevub.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2plqmtvet.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ftiysuho.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nlhkplsx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2izucbvma.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zjdlswqf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2galsurss.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kygsuwlc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mwsmofgs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2puxatohq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dqrycoon.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mfjeduaj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vdlohcti.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xrnmdwlf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dlbdelmm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sjrxrovi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2fcoysuml.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmsnjsfe.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mogqytid.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ahmiobez.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cklqgshd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2iotnajnt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yxxepnmr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pnvtkvcr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2iozkkaxx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zaaohkrv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2tgsyrvop.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2halksbwt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lykeypde.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qtkolyxc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2iekrxdsy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2aunwoqyq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ksdjcusv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2msipdmwa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ddyjdgak.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2amxethha.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oajrlchg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mchhujhg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nbrtvygx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vfeywawy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xuxygizw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kzynqrav.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gkrjhaez.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcqijh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ddpcpnvv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zebxkmhx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2anouhcnf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lrikfxpl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vtccfpqz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2swmzgwkp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ftilcdxy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jcxiqteh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2uwzlsuvo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jhdskkyn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2boefaevx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2piyvkifd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rhsozeel.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2iqfdpnpo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2psvsltlg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ccislazq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nfbepcdb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yprysgqi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2nyzucckw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qipxrskz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kdcmbdfr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ploahxrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aizkuomd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2crtusrjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdxvntss.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xafpqbdy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ixxmqupv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2narhlijx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2madelchg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ownvahrs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dwavkscj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvdesqzg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ettmcpbw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wyoocbgl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rzmqmopl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jzmiwupf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xmfexnau.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bqagjhbc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2odjejjdx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2otsbiazt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2imzriako.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2mdqxxrys.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mqdzmtfs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zlhgxtzb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2hnqrycbm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2rugvzgib.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dnsecfcc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tadgpeaz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gxgvowxd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wcawdksh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2qibbaffx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2umljxwur.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qcsxfspn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hjkzokyn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wxwlyocl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pmguupkx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aiapcuyx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tgwoyaou.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2daaxmxor.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2otsebldk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2pcffzyaf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tjdzcksh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gueibeuc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dzcysfdi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2miktmgif.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hepowror.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rkpukivh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dohqsggq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rutfplnk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vzboqwso.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ixvvwqyi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ahqakhph.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2bkcdwubd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lrbafaxd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fqmyfiaa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ntcdxzjm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2iuvukuzx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cupbybmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfgsyapl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vowhmjpy.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2npehbhos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtllvbhq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2plmczwvr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kknvcdag.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rjcwiodq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vvruqyiy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gievitrm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lihkapyq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ibtyibsc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ahbislyk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2yftftfza.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2bcalkyus.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2rlyftvyr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2gzwazlwn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vfstsfps.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jtjbkmbo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2rlhzjncs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tvuizbde.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wnbbhetc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2dczqusyk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2bciswcxu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xeagmfjk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vcffatmk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tulanhzt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2credaxxa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hifizgit.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmcrtxdk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oywersjv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtmlrctx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zqdowgdl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fuhuiyym.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdbznxio.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bkcujyck.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ujpnceds.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2racibozj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gzboirpq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fnmhcjar.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2htmedsjw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pqkhleyv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pejtheof.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fghocgfe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2gxxaizpu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nueqtjyc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sctphvpi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2grlmhrbx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2nqbihrsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmcbcznz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2lmpezjca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqbjyvdh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2omyayjvz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wmxhzedh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2nhrghfdt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sdysjqce.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2yecrdyyi.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fufuzfbe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ktewmyon.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ntytfyjz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nqzwbpvz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dsfliqhk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rmbrfyvi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zyrjenkg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rqxldskk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2frbiuban.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dcnprwuj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2peuobbwl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2euhslhqx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zgwulieg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kuxiipmj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xxjsiodp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wvbqarwb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bszcohzc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oogjbzlg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2piyuzozp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wkuxuirf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zdwkocsa.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yndruxlc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jimyhmjt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cyecirjp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dczolgrz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2oyehunaa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uztydwfe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vhwvzlmo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jqadpdre.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ijokkqoq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2nkuewqwi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qhqhfxpg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntvpusys.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uqdauqds.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gjxwhlts.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xdyzycap.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hputfcfp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bnxobdeg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vhkfkmzu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ojeauody.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wbpxawih.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jkdlaaoe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2xurcbkhr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bjzelabc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gtnmqohc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tfbomper.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uaajwxdn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2cytnmdbv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qhautijk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pzthcuxt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zzhnswmp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhwcxqn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fuikflcn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2pmqarkhq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2abajgkdj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpivrev.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wibqzknw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wsbuwntj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ojbaloua.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oytwbijc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2siuidxez.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eylriyba.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xcurnjmq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nwcgtdet.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlgjits.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qffqxqds.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ylutasdt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hqhordrn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjtgoaw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iuecdzks.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgsaiusy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gbboyils.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjtgqep.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2nbacezyk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tmxowvpe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iikxxuyc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vuevxpgb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2pjosphvo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fyiukirx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ugdexdln.html


<!-- 参考信息 -->