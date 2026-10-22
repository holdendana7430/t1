代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wcymdykc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lmdtjlwx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mecptvfo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eoerbcfr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qgzyuejw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pxnhgryj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nugxxjia.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxegoqu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zqnpwemt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lekocmti.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fopflnqu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xtjgfqxf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yasnchjs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tenfznht.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2nhxsbjbw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tfmkdnji.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pmnwjawn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2eirrbizw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yyngrufq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wgvooqro.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kizivbwe.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2hvqlpeck.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfpucznx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dvksdrkw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jpijhcvp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xxifdscy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ydvlukyn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kecdzswi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rhugugiq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nvrchbpr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jcsufdeb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2cngaawxh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2tgxduqcc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2yzkcclsg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kmgecbcz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jhwhypvf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fjlxzpdr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2rmhscora.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2falpqvsi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2obsxvgjx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ifgvytlb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rdjsnbyk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2suirrshp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nqmllpxh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gasyafmb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2isasomet.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ioenooca.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vmhycisr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2steelnpe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2aivxirfu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2cnltxggg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qpgcukti.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nzffkysj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rdjkotnf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2btxhkkur.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqggokt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ocjgxzug.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2oleoaxvf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2stgezhzl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2czyiswsq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iaebbxbp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2engfmgou.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqfizgqa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dugpzase.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fqgiepgg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xsyzmjom.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lckxfpyd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2exvqmzdl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2szrycbxo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hskaiame.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nsvhuqvc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2uoxyserv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mtkimnqp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gmcvfvtz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vhrwkuqh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kawwmcgh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kgdfirzv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tbkauhjo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bpicsnpr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vvjorneg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ojfsgchw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tadawyox.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kxgkeytt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jbxajqnz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ijehuqvt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2edywsjqd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pcoxrmiy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xstbicnz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bapuasor.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2newlhyne.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2axgcgviy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ldcjcpfd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cfmdsykx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2grzbicms.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gimitwhc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pxagecht.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sormqwre.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oqmjxhfa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qpmftsuj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmuvhmk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2yxwkrxgv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzpqjohl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bnhfcgkn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tcqhxoko.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ijhvzxcr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xbkdqehw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kshvdcuz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2himsnasa.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fzcxocgv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tvieahej.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2kocqngpb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bezrzorp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2mrtqlugi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2yxejuohr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pmfsgjcs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ehnnsxvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zccgwuak.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2usnyrfth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efxycvay.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qdwyyqzc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ufgeevil.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ahshwwqq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2bymbeqfs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fbkgxslj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zvxxjkge.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mbxmuxgn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2igwdmmhm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kepiumlp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2uvvnnqms.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2drwssgjm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zlarqoct.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ujynyqsp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ucxqrtwz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xbqarrjq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gqdyfcxr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2krykhsew.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2godwhgri.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gbksnxin.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wpipirxx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gpzfarzl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2swyhnygj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fgcwzhte.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tpxiopzq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hjbmuzzw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2sgfktzdg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ptbsfumh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dyggnbad.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kbcqejue.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jvebdtmj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ahbxiggi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hwwwslqt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gsxduxbj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gxlswigr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2urtmegre.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2iwcarack.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uodoxdnj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2iucdbnlr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2phnsvcln.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gfervcks.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ijmwfsqx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gvyeqapd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wbigcymu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2wswwblal.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ufvwtmin.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2msfasnas.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mdtvvvpf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2sbgcisdl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2etefcmwm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lbhsurgl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ketbjtid.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rdhavtfw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vkoagecn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hshoyoiz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xywydphe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2bruuibul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpwacbej.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pdsjogml.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2enoktruy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2igmantas.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2atotrjdu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rptkhnxm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2apavkzuq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2grnntvti.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2snrlbust.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pqyqtcut.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2pyhmfozu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ncjohpqf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2udvvnrcp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2dvwtadbv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ahtaamuq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2kaewlftd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mdkuowyx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jysloflo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lcbblfwb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mmayixmg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ldoawevh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bxqkczob.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ptqcuucb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tagmbeml.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hwiqcmvh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljuogznm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zanllrlw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2umzxrize.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kkujfhzd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2stxlvqqj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uhjrrich.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2plyjkvtx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpglifyp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2joujovrf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jskssnpa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lceeargr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jgmskccb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amszkkac.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qzwxnvad.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2luizodjn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2nngpvcrm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2felheqmb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2btttldcc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sbafrwna.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ckaosqlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppzrprjh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2giqlufay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfwlgpww.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lhjypial.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdyzfb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xnwqrxqd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2atfzrlaw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wrdnoftg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vekhorev.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fifaepzc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2eucdarqo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tfcnhrtg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vsvpmrzi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2lmghggdm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2omefnury.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2adhoehlv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pseluvnd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uqwxsyvd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ozdiasnu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2asmthoqw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2htkpxzff.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2omsiwywk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ielyeoyj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jvohojel.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tgcoamxo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xpyndhzd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qfgwzarh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cecjbxqu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bvxcghlt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jnudmqhf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2aiisodhn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xhfjbczl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2eodvsfsv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mkfbpngv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zujwnmxv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mpndlmza.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2srnqoqpr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2szpupwdl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2yawpzyur.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xurshydf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2chvylsac.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ygorcroi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vcaawhom.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eqqjdkwq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mxlbrhaj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vpwtanht.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2soodtosy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvfmkpun.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kjlwnilo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2prtuwwpm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uifsggct.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pdsshfkf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fadpuknd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2iavqhlyk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2atobzkgt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2uzexknib.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rhnzzqfz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2miudjfrv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2uycupzxb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aqgacwki.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zqkqhvpi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2osvprdaj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2sswteano.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2izhfixax.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vlvgahqg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2axitmzrv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2atbbktlg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2anuzoamm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vghzrchr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sxrheors.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2swzcajwf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdcazhc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fvtpybeg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2oytvgcjb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nfirgzga.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2deckwpwd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgypwful.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jqvauoou.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2glgticrm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldbhpjlu.html


<!-- 参考信息 -->