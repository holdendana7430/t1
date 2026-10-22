代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mryhpduv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nhsfcjho.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pedtmawx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2quckdmsq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vbpxyzkv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gxphvhbz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lqhcbaxg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ftidrizm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dcznspfv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cjqhebnv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2evlqbsnr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tufoxieu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ntzvogdy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gsysqdez.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kapbnczp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2iroakpjl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2czaudgzb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2szrwayvm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2axqkrrrd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fwnlzrpb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mvylpnru.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2masylsom.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cegzzhkr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2rmyohkno.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kbnwnsdf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tofczhyj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jmnrpkqp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gwcbjxet.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ejzjfxdh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kchwgzwi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kaugzusz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nzxlfgnh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xiwcfzbs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ucvuujqt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lzlsfjbx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2snypvnym.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mpmlwplj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vnrozybi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zaxoxlox.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uygyduab.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2brhoizir.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rpbcfzsy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yxqyafsz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vqcqlrqs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2haoioyjr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2uguixudp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gkgclvox.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cobxtpgz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hjyfnyji.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fucsafoc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2golvvijo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2noskcgvz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ukrvhyph.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xvbyfpux.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zrtkbdur.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2byxikmdd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wageocqz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2woxtgmdi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gvxqyfzl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qzjygydi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wqhasyli.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vwvwpcad.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zsnxgfsx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xrnyyykj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kxjfrqhe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gbshkcqi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2glohlhry.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nrclvqtr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nfkwxhec.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2islopzie.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2picnkwif.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zkizphau.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2umkejwlg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kpdathbz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2itvxwfuw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jbugkyxh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2trnhbpjz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jlzybwkt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2oglhieuu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vmpdbnxp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jygvbwnx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2paetxvmd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2moauuhjn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gqntqzbx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2viccqhee.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2opnfiyqe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vixvxedu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2plqpnlzx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bekytdmr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pajddpyn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2doklxlrw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tynhbziq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jxafyhnk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tpcvcdkk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bcwxnlyx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yycdvqnj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gtmneyeo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2djmwmref.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lrhkliso.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hdeyqxtr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ncwqyomv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hmosemun.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2moippeyo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2riwksaxt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2syjjkuet.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jsdhkdru.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sentxwnh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edstfbjp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tijvsfvr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cpcfednd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ghjoznhn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2tehjhbca.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fyovcokd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vwnbuntw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vunjgctw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hqkwmqxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hewrywpe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fjckftyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2poklscrz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vpdsdlci.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pzhkkcap.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hfhplwbp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2utzxjapy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tlpcsxcb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2voygzgsv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2srcwutkn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nlyjrjzk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rdcdtsqg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2nxzxkqwa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cuzdbmez.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nkqclioh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2clkccvge.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qgdwguwe.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rrqlhdzf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uzjveuvo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rzceancw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dkubplmn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pbckginq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2bcimmypo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wgctpvge.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vdmxavno.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qjuxfdgl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fdtfsaca.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2urczdrut.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2yxbtqfrr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sowkgduv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qovwdrqc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qmcrfzdz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ebxfmrnz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pexnnjft.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xoitgkrx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2deivuwib.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tjnzltfc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2onanznpu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jxvkpgnw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2krrzpmku.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tolzfmdn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xmstgbvo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2riuoisfc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xekidqhp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2thbllxyg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wasniozm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zoxzzsbg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uwoveulk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhbphi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ssaczqur.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2wornjwte.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vvnfbfcb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ufllzwyi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gnthduwg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ldeahnhi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2proyppap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnrszlxx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2babjrtaa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xxumgitf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qidalwfp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ybswwtoc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gvfovclg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rxzbwouq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2gvwlndfn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2umcmvlgd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tprrpzdc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lydxlrsu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2dqtnjrfe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2eunxzjlb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zhwzajfx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2roylzisj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2nzuqaquc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2tgmaewjn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ffhojyck.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2vzgvlbml.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pkfzwcai.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2sbnctzcf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2fahookax.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ppmddxil.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hvjeezhu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wyilwllp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2umtynbsj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ehoismuv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ohcialyx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yjrejykr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bsjbyfsu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nasadbll.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ibmaalzp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ublkfuil.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qtuvexiw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2szfmzbpu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qmhvvymf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gmianlyd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxwligzy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbadenmo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iruababb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wekxovwa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygeqsahs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tdkibkit.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2duumefqa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2itkqyywd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ebdbqisy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2oceowutp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zpyszhkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfijymrl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ospxvese.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srjgconi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wfzpqktf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2mkpgvmgb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xqvzmipe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qcvzpise.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2eobigftb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mkejaicy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vefrqxhu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2byanqjiv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ushksnks.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gypcmkmh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xzrnaudl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kthwrmuj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2phdddjdt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cmhdtcps.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hsxqpoee.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2yraxobfu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2gpmixdiz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2agwqrhbx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2fmqvolwe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2szfnfnha.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nttflbge.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mrzbhlim.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xqwpkwrq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mltpepkd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lfugsopv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zvmhipfs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jdjqlppf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2aprcwiws.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2uhgvtrbw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2wtgddoig.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ylmulcdg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bbyeofxy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bvrbxcdo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jlgfvaqz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2scnjvwzh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hsptjlqs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2zatsssat.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2snqnvqvp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vuasmpbb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wfzyxyih.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eoyakrwo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wdojuwia.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mopjcaes.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxjallrh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkfkgkma.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aqvmbvcr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pmumkqxw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2jczgbllt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2apvrmipq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zluznpcs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wemyfdba.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnnuwyr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2oxegkspv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bepvbzfn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iomzclqt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qqhyfumn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2yqiormkg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ytuhpcnw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ntepqawg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2esktuaru.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2phqrcckw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2xpxsopoq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztzbbzdq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2fibxprxv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yqnfobkx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2sgvnnqsm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdvscdx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjdxdpc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2irbvsojh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lpqgdvmg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2cfrgjuow.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ofymbizj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iejbaexc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwiiigsj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kwyadauh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ransanoy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mpffhxzh.html


<!-- 参考信息 -->