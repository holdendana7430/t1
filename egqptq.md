代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gmbzupnu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2apjctxoq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fpvunlow.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zvkjpobs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2myedoush.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nlcrkmdr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2htckswbn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2iktfxqcm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fqxvddsa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2urzccgvt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2oearsoci.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gtzcslww.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2aiwdkezd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pimlqheq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2upzjldza.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mjilzkae.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cjvznokw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fswpookw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2hxuesuyx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xyyihipt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gfhtikam.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2cpddktsd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rcmeojuc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2abnlawre.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qsgimnia.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vnqujqid.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jmuyhejp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xxfdilec.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2usthdtto.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mrphilei.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fimjdcnh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xjtnaamx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rxebeamx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vtnsajel.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ajcieqps.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zfibaoyg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bpnwprxs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tavqdftp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fyqektxe.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cqyspdwk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2otbspodi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bhtmunna.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jsqyxxtk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jfakmnbw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkpohupv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2indllchn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bnpjecun.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lxqdlefk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rminqluo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mfspyofg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nhcaatrn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzmexgmu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlfettsc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kajiuzav.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2waqkrclt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mvdaqowk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2blwqoanq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xrmuojnk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sbbwycmr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eveyymwj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2npywcoqe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ykrmrzen.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xuwgwwmt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nunlioir.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fckfsmox.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yabrpfyt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tivbefyh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2btjzdelo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rawaxyzp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2njcypzpc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vmthfxnr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2sntesyll.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bffaezgd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bvetufve.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mfablrry.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xaqvowzq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2uytfqhog.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hyfjjual.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ibjeteja.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tkvzhmjk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ufhhudcb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hqkcpbiq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wvmqposo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vqwdzbzv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rpbdfwxn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuyeyjj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2stqtfffl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ytivbtgu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zxaopvtk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nkbrymcf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pnvsfanf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vivqspmb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2nxyhsxuc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rqgkxwhq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2myefdoex.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zolodoqm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tfoqjszy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ogqrkxqe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rpbsckbz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hchljwlw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ukohxhvn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2urgluvcr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zthcfnpt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wgpuxpzp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2chmjerah.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2dfqmbqxh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jigokaqf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2czdguehp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcusfduy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2okwthdkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngmxqcjq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2adylqnew.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ledwohjj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hkhxwclg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ahcotonn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pcoaolkg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mhfqriza.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2enpeablz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rckjbgnr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jtmxrzdz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lcmhjcel.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xtqihlmw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hheiszix.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hvtpkbwk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kdrpkggl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ivolaskn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2oyppfqcy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2juvrrfsg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cgxusarw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zewfbwff.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xrlfvgsw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wrlmjloe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gfkmxhtf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2imxqgheq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2egpyyofa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wnkoyavx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2omlhimng.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xpcfrhao.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uqxemdqv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2eejcrnjf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hdiypawy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xezrebvt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2owfjrjxf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mxzaniqu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2teuirsml.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qyspkxke.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qzyqujzz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bcrkswic.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2bvtdvhwr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jsfmipzp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zlysunjb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nfyvrmbv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2etdmedfi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sfzmupbe.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rzxhwywq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zlxvmpne.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2begsjobu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rrymlpwj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ndyyolcn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rahsnxvw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ykccjhtf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2xwcxpkux.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qcdaguko.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vesknkrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxycvtee.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2scscagte.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2sqqqvbfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wscmwziz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ikxehgef.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2xlvkwlyv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ulpujqjb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2eaurxivk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bbqcklcc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2sikhfqur.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xktbthmv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2evoiniaq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2cuinjvbq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qxtmrsjo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2twgxvqrw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ujgcavns.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2oebcpkhy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rxbcsesv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nsdodbhf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ksmagxfq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2nphougrp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nqwxmazm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2hknxrqqo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xheesvis.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qgxsdyrx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2yknkquns.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ubcwwocv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zemzwqki.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qjlqhhrr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nljtgdry.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ltwwmrjv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dktrvfbv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2drrryrun.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mzupjlkv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nztnhxar.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tfdpnmfm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ltbehxnx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xclmujon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pdkqfcye.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jjbkuxds.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2payniuwr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bkushuvx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2itpiqyep.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xropyrqu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fnoyqafs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xstzizum.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2szftajkh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbuzcpue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuifwqnt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gbntuqhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olxnwpos.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wtadqtnj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gsoqojfk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xvuxyycn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lwkdayrw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2fqvpgfgm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tvnmigqo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cixohgrs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2abnbgmdn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uoagjnfu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pumnteal.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jteljmqo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ggtaqmwg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wmsimgrl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jtwvnqoh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2suqhmvbc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2mmwtchgw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2fjkmxnrn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xoganyjg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2anvgrdhr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mqnfogtn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qskfnghm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jdsncinj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xqrfhrfv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bkuhacgs.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tsacpzsd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pdmuuucc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lqdyczld.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2plhrfmhv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2koowobaa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtdzwcel.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hitscyas.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xzzsbbsk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2lbdxgfff.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fzopcndm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2pyfvdwgb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2juqgetyw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2uqhuetge.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aamdbrxy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fcmnymwp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dfhubrod.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehyjfrqm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dltfpgca.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pivokzbd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ljlgudlj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sgylddkn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hithhuvl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tmhnlmmu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ykilqgxy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pqruezxw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wyiqbimx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yietzppd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xcljnxap.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2brjvedrk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jpnoropu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2tuzbcost.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zmjhivfz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bljothwz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edjlgpfs.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xdsgajnd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lffncnsu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fnlufrxe.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dohihfrd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vzimfyuz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jrwpdcfu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2trccvoxv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vvzoxceq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sukiuomr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2oexhqpkc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfnbrgy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2healkgeh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rgtaunee.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ohwuxssb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ymurtbhu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujjlpukw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hczekork.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lokimxkp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imusnqma.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeufrlko.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cchmjgtz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cgszhzac.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bborzgyn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qijsbqhe.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2npfzexyj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ypsxwtns.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyxznuho.html


<!-- 参考信息 -->