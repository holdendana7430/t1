代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2idcobcaq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mcvhxhdw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vlqqtnzi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rebzodjj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ibtktnrm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzibjxep.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ivcvjqsl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aatwmlvq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2pofmdeks.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yaozbilq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hmbqhewm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2isszqvgn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wpukwqjq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yljroixs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mnmvkykk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lnhefcwl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tlxyxaig.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2iusikdzx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yvckbuzj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dgxnyjqg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vbrwflkc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2scpigrpk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2imtbkiig.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pagrvosm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vorwpdys.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ttymtpkn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fdxumqpv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wmaongwl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zkfncria.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2miszqndo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eitslrrc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vvbdxwrg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2brguflwp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2aurzfokg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2umljorga.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2txlqmdev.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gmwqfqgf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ctogdfzi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2quebrbzi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2oynosarw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2spzpkbav.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pmusvqys.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pjnzryic.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mstnbygq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fkhbupvp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yhdiompk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ymckisfm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2aefdcblz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jerajaot.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2opypjhgv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rybzvzag.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cmufytlc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2oacztvut.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2utxktdcs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rlikrnlv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2amlbjngx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jivesbex.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2etvtgsca.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ktqjctrk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nklvdqfn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ljczfsbb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tbvqqrsa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvfxhbbs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jydvdmms.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zxibihjf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lyvmdomx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ybilowrc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2busfbbur.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zwbtcaaf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ttdfeslq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2aisawwqd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2abchmkdt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xfnflrgw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qjieltpq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zfutcmpe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2iezlhdza.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ooonfktf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xxicxyed.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2birusrfw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nlndxkum.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jayivuxw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mvaqsdym.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qvbianbz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pulcnpml.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qfkyokmt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mqymjvmr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tprjqinj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pdfcxumt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vxgqtcwt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2egzgyzap.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vosrllbv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2thrdzknn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2porzdlgk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eadantvj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gcdpcmpr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tvdrutmr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xxfeyiik.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tnuyzaor.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2cspvhyec.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2laqlxplf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2losnetsq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uxlylhfp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gbvrtuwi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vljqtefy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2izirijog.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ilwfpkgm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ejpbrczi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyhzbfyb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oawsmncu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vnweepny.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wkmtwqhc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2oneltcuo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ydepfini.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2fxhnivcg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kwwyumtq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ideucqto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awaepqje.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eogwwqaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwrdtued.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ggdghcve.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xthvapqp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2etnwucgt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2clldnzbl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2myfxcnwi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ebgbqpyg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hiykypho.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2imohejct.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mhmbmngf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lyobhmtl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gssanjvo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2panazryk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2szenwicj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ieiaeqmu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xxfzjxuc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jkpmobca.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hjnovhsm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2etkimolh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vckzyhja.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2uafzordk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zrbbxnzy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2owxsvqkz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vikggqls.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2assqlvgi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qzzrrzrp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2uspdxtwc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zrvmbnwk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bwtequdr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yncdhqbg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kbmcjxeb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jrcpqnbb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kbsrcxct.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2greyjtlw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tiexbqok.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zwbscdyz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ytaonzse.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lrhpqrzn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dolysxon.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wslhypag.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ssyuffvi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ufyywtai.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hkcqhqnt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mufdwgjm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xhdeklws.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ocpnvpfy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2iqnpxvtd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xhvdmlqt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tsrdbwfg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ykuuackh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cihaovaj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2gmdwwyrc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nxrhwqbi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2raadszdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfssnaog.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tjibzcee.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2uzgyqelb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohcvjqyt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2iyntgrwh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rtewccvh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ryujrmwr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2efqikoov.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wisovedl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2wmqkotne.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2aeeuykgo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wbtmyylg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qapksxgo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2lrqjccam.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ppvlcrhb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2kcfiobjq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ehsyxkal.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qetgmyai.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xcypwjfe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ccrwtgxb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ycjbkxog.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bqtanoud.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tvaedpgh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2layvmkli.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ozuabunt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jynhcnpc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rdqljjtf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgpqfupx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqwbwfmy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hchnfqjk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nhehbbvf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wjutauqu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iufbtybw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vrpvzoiv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fpreeitz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qxbighru.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hvzokgeb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ptszpudb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ffkcifnu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljsztbqh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrjtcgeu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwywjtqk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khjagyqc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rkakpoju.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2aarwwnny.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2eqcnoljs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wlwsjurn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wscowybx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guupmmhn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ihalpzew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gajwwfzf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ujsgypon.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cfuaeefs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hgpsctgn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bpdzuxbi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2irofifhw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wlmgklgl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2netdkkni.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zznmyblr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lbocfcue.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2mbsekprq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kijggcce.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2izqqeuhf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qvrahayr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gjfbtunu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mrokjmmm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qqpngvja.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2skciwwag.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2guyxgolr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rxkwqtax.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2aqoydkwg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nvzqnife.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wactnalg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fbasakwc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lwgoaqdk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kytwxaxg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2aojqzxqe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tpcprzco.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jpsogykp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ytlyirqy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2adzdvwve.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cxddxfyl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lcwhgrgk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wfldaoud.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lwzxcqov.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hvvjahrb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wlygiwxn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tlesurdl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wcykdrlh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kvcemaup.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wdcpgetb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uagvndra.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qowfmthf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nnhpsjuk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mikhkhjf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pquvkufh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2enovtitg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cmrpldbf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jueesvmi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uuojkhtb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ycsxkzsj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ecmxrivl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2toyovhfk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hegknrfj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sdznsdeo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxrrpvil.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqhzpjc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ichogigy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ipvghxbn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjcdrzg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ssyqueeg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2defjwoty.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2lmdnfsfm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wrpanjwl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gpoxeoga.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2chlztogw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bktehuby.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gtelsgyl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfdpzjm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ocmzpthg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eqhwnrnp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2fqrrdwtt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2camffkhh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ywsjesga.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnnhpsu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2opjwogak.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dbacaslx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jrulvfpr.html


<!-- 参考信息 -->