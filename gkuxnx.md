代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3fhbzhirk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twgfnqat.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wdkztwnv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zwdvgkgr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3twrfcyyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kedrryom.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3eclimwlf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rhcraora.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mogfczkx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ivoxjvbg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rjyqkwte.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ioilsskd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3innydyrt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fbuzbkjj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tmlxoskd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rbchooey.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3epfscwet.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ndoedcwe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dudxqpki.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hullywwo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jopfzpwo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ybxmxkva.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dddumocy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mkuidqsz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jbictcpf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zpaizokp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oyopcuau.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qecufwsw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pbfdxqwu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3whafqoav.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xohjulbs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yqlomwrm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjrtju.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cxsmhrha.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cxsfqspm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tcowrwlj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ohekxbha.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fghwpfyr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tudgkrsb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3yxxqnkuf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dgpajiaa.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ublhxsqm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3efrsdjpm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qbfzusri.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3iurdgqbi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rdlqdygo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xicyiveo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3tumlrijd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tjshhkzg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jnrzfzpu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ucsommsw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bncrnrar.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zmhstilz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yvmkknfi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gzuqmpqo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nshssyhq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aenypzpn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qvchdyqy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nhcpiehj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vqjybwpy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rfdubmsd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3szgyernz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tyeupdrd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tljystwk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rmnmivqc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ozmomort.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fwwyhpkv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tjgapiyc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pkpyeptc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oterwpcd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3iathvoba.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3awmfwmrb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3swjbcxcr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vulhlizl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ktexdtvw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nnhrrvsq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3temyzfdg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fajaxpgc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rstpdqva.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pnqmxmrt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xigijcpd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ttkepjla.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bjemzbvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3shkarsmb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pdfbyrax.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xyufzkrp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3crdkigkw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xawampng.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tphpfnlb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hlbzimpa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wgprbhoa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qyymsmqt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3itmsonad.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xzxeulxx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vvclfvfv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fmrrazfj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ncrkdypp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dminlhok.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3yrnezacp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qiglxkxi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxzbvn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mpenrfrd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mtualjrd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhjkikts.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qllbbydq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wvyirbdy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nfqzxbob.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nkfbkbkg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kqnzslzi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hoqlrxlo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mofwripa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3aariqmsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbmczboe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jramfcql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wagsporb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zuqqxxgb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3pwvxlutv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jhzvftjt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wukuljht.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tyqptmlc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iietuopv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wzutggvt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vybasxnp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kgiyxxoi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3okkrkiiq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xlpnzpsf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yoxmsmwu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mhsongua.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mwdrtcyt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3efumtvvb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ixuumwif.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vwsvdqhv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3swgmdqhd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3femtlrbp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ikrfayel.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zwbypkds.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rusxtrot.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lfjsygfs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xkfzaagt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3llrhgjfl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pbuwiuas.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3urqnvpdg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hyajelrl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yolmbsgw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mbreujfw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gjzttzxo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qbenaoqg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fjtvydjd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yomzpzbf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3knvknper.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ncmvazbm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qyfkxewb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rpztqmxt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cwscsegm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gpdiuuhe.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3exogswhw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nsknnhqu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3akuihann.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kbhgngji.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nwnaywob.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cylprusy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fiajcfkm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qkeyerfe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3uukbxoim.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3nlhrbqhw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hxtgujva.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hserhusc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3kcfdteov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyckbiqc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rardlgdh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3cllbhbmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ompbgmfb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3yezariym.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3utomkdlj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3siauthkz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3imqjsjel.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jzoycdmq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3cmeedjcq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hfqrussi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hwspyzoh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3nogpebga.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ufdjdhwp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vyodhvgh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gutdpnkc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3pclqzskv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3epyftlfr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fmipakfj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3opxcbjol.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lxwnizcj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rspnfeca.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bgizzxnr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jptlwiyo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3efywnlbd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ezofuyve.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mxuuegbj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylnrrlzt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qmstyqzl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3czckzplw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrzwitxz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sqdncawq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bfrxanzo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itpsrrbo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uikwahgg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jewpwiuh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qsshflel.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lalidknx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nligvxlj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3whuwiddl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ofqgevhs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vxdrirql.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ityaqvbk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ygrlmlda.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fgrevzjn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rxxukvxk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xgwlpevz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcuhmtda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcszlefp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ngflooqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vglevywq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3imomdxbr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ueqftpzs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kygotlis.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zwybhsvk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3htgikvde.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3abozabyt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vluzpzjb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kekqbhol.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3izjsgzhi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3zrbhkuih.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bnfxlvoo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ioaopegy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jpwogwdl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dicxeylz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3plbunvng.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fhemyfvn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vlbcqmux.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dsxhzxlx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3atznemkx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3pakwiyop.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3crmmcwiv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmyypcog.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iklbjjxa.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zjdrvcsa.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jyiyijwa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kptshjhv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hcpeizkk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3igylhaxi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvlwcaw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3btqigswj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jkxvkhob.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bzshjpwj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3cifyojwe.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tlnhukji.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ofjxpmki.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3qdctecvx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mzkasejr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3atwkyhtd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ngkmxsfo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hdcmizhf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ppjesnol.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fuqbbyto.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tuqszccs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgpgbksi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aambnjnx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3snhqbxjm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kmjkleat.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qzigkrri.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3atkkrcqo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lplyoukj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qzalsyrn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3igrlvkrf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3noextczr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3daacvfhk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bfeosejg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3etyhvznh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwrofbp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3oxetpaek.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bgxqxnso.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hooeggyd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dzonuxkg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3orirbrlt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3klmmwodq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3dnxjsycg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jegiwunl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ulteimdu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3svnnjdbh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3nhdseezj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ghquorrd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wqfquzsg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ewstfrea.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yekdtjqh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3psyyqoiq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3utpotykj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3esduwrel.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qspsxnwt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbhycsfv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdwlbtim.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3esahqtqg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3puqjfnxh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3frvvwgrr.html


<!-- 参考信息 -->