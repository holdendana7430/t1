代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dhcmpxny.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tzcnljmr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xvuvgkub.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bnvsvbnu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ioaorwlz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ajzgvzsd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3aoxkbbmv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mccevgdz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mzpghuan.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wstpcydp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3erzbyvpw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3svnebvyv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nxtjfcjp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3syvdknmr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxigqzeh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vauyzika.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rxhdazwi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3giegrjwl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rgavreko.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qmqatulw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xwreduht.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3egibtymf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ezmjrdiu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3juiyefvz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tmdeinyo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ykjcfbcl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pifwqyee.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gphybssq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ycdhwkbg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3trdredhl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mhvcrlpo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3naywvggr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mwguebod.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ssqxfnyv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3pohpaujo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3orzuctfy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bfmpfdws.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ijzgumjs.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3waiukljd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3caasncad.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mibvrsmr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cegaouah.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sbofezny.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3onhxkbkh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3weailbvw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gbdfhjue.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zevrhidi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdcwvqs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eskgjids.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ufxpnjnm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3lmbacadt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aghmmspb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vpkmtspr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3krjusrzl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxcgvjav.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qctmyrlh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3txskjeum.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3emktduek.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wjoppkro.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aplvlbth.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xzuflfym.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eavmtwqe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pxqeelam.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ogloqvhy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tzgnuasb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ybyzrdig.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mvbpnyct.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3utcznldm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rormwfcs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3avbirliu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kybthikx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3imhdczmk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3alfutwsr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ktrqsuux.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jabbtxzp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yidjhaqm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rsltauog.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ayqmowmg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3afnqtkei.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3bodwlpjv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lkiahzbb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3skggyjqm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cqesblfn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3tiwagzvb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wcytszoh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xsmvzkzw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tgrklbjk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3hzqxpmlb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ykwjlxvv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fupycdmi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kvaqtxop.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3neuceyic.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zwydonhf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ayyfwfog.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vecktdza.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jdqcgxrg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gtplacmm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cepbzahz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zprhauiv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaqskgqz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nujivlyx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3meobmrrd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3icmtugln.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xgwhmyjy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ielkqwsm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dhckyltk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rqmufowp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wauqgeii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmvdepcb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3amnqbrbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvucjkbn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wnvetmmc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3szijiofs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3cikzxbys.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rfzaqyft.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3rpyxogqz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ehmgkzla.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zaeremrb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jpbgnrck.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mjduyxwt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vfjerktk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mtkwohqf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jgfbucgj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3oorzezei.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qoygdwra.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dutlxmgg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xvzrqddx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nnlxsmxk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xiviccwr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yorpebsg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3plfjpuau.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3unkglgto.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jqlnsjsc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3njgcibvk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vgomusdj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mwmowgqj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wzatstgg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lzsuwfxx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uluarczf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tgbzhlme.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xwcfdwvi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vpsvxfcj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vwhrsauk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oduglvbp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mixtbrff.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zhemawyd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3evdhnlfq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ntmnujbu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vpunampn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ocmktnky.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3udrcisid.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zcznwyed.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3prhxopud.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vurodbnt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jlkuyqal.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3exysoipg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qutfwahh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ukwjhlwn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3yevfypjo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vhwnedln.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mncayggu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ylemkvxx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3plfzzxgs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xwklfiod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixensmxn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qihraqrj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fbldcdxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tufzlbnk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xtaihbee.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ckshicgc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3aiousfqt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3uyafckxu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nhejawzi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gfwfmxxw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3eyjpkeck.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3suicyhny.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mfjmorse.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jzrffywm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ighwwerq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xxmliblh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3kxynpzfn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pbazqtgd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vmficngd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3badlkqru.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vwmscdgc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3pinpqfcq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ngurssil.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3benvvqsb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sttkyinc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3swlwhipz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ewqdyutj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zbmvjayr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnzimmet.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxpmluth.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ckqdauhu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skqgukjo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgxyrhbv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gtfxnwjp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cqskmdmh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eenoashb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpvbragd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mbznrydz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tciugpnx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pvzhjzrf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dibidzsf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgyrowuf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xcyfvgbv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ahlqyldx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jzcvmhdw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3cmrmttof.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hacfnldp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ruotzcbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlfkjgyu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxdzbkzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqugusgr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rtykyjgk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wspfwqzd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3imhsympw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bbjlzkra.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwwkxpb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wowaujzo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rwkhmpiw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3lfbxqqtw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dcqmnzav.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3odlkwzbe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3rvwvowap.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3etlhbhrp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lxoakmzy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rftozbsd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fxqbzadw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3pljlumao.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3svvjapli.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dbemyluy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kdenthnj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3nzgsxrql.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzduojdc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3shuyglfz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nojqsflu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzmsjzyz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tngbnokt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ifxlqish.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ofazbxli.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qkfvtklr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqtrenn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3isqpqtsr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hazrxvvr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jusmenbe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qgcuxqkt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3oagqdydl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ziopmusj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mutlewdj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3uzceunrj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ogkpikdt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kemkooht.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3agpjqpwj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vyzdowve.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3piycshfd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sinkjyho.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbjqyikx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zjjvcgsj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3npngcqka.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3axghzenz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3eykdkuuj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3llqzuion.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3aqkzdyie.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bqjvylmc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tnjkmlbi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lvnabwsn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vsmukoou.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3qcrpaghr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzdikhq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qjygnwsa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mjhsazzu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwrtqva.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3disambzg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3enrabnhh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3czhwzupc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jtojmbks.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3osjxtjjl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vekswpfe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vbjvlqgx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dchzrgnz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3boisybxu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ahlqaemm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3molwsbkx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zyrdwimn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pctvyaqy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yydxfpxf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqffwvfc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynnsdzew.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfprxzj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vmobkxvz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzqaemk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xixdpbkl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rudmycks.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cidunqnn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3pxskgkcv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3thhctbnf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3agozdclh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xnvetlcd.html


<!-- 参考信息 -->