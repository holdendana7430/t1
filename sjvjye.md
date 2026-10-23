代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ueykhxth.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3avefblti.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xusbpfkr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vhqoxxcf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3odqznswr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3adjkkmth.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tgkddkjn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zaveuqhj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3eqyhgdoq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lusieqif.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xpknczqa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cfwpgodz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mnwylckv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bgbxuypv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xyvegutx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wdwsaqkc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ncpwoekx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3scyqfqls.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ubafbppt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kktrozph.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uivwvzaa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zrikynuq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tbrkgvmw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yivavvzz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wsewxqen.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsmsrxp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nbdvxutm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lysoarvy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3azmmivjg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hoawvtvo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dhnicmcb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pcpiuyjs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dfxrpkbu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3whqxjpik.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zaptwmck.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3btdksmfb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3oynxajdj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pgxlyesx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hlttueai.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ucsgyatc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qrkpbtco.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gqwfhxgx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cqnjesat.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gxqzlpgy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3efbramul.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kckrwmwh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hzxgirjg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3utmcvkjn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yiaktbcw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gnrtseja.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qoztltoz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bxczrpmg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nllasmix.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3seaoijcm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wkrnlcdn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yrgyqsey.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dcrkqeai.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cxqgygct.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jrsgrzne.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjtgqkj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vpbkirxx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xzxcdcva.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3btrkcbgh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rczqzyne.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hhfzctjo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3pgwarczw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmjmdafx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqenspo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3yuxtnrvo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3savjiurn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3cszmucid.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssikjwcs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nmluftoy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qfdgjdcu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cctshxzs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qdhgjbge.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xijsfrae.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qkdwgjtl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lqsixvtp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hshpnrll.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zltjzogx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rprcmowv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fmkxmhhn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3oqalhojd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nezjkwwc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rnclduta.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3knaxsxrl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eiuwdnjv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tqpwkksz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3urflbkjd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hyqugjbc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yoajqlai.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3monpbbzi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3guusmzsk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgmedu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3verjzobn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rwekfcqa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ewnzhzie.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ejfrkhvh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xidlmsjy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dxqujqep.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ybbtlxvn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3echtztqk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3enlekopu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vfcircxo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hacqcocr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qtgrmnjg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3grducbqp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ibpozubo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zjlvweuj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ochlbona.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3bpnuztlj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xgaolqej.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zmqhwzsj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jcizfomb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3exugzarp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bkhvanls.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dczhxmgm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xnghzhwa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jdzrrsbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmjvzymk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zkpounhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfzcknis.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3edqqkwkw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hhmtogeg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zhhrjkhi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3usdzctts.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3angxqoql.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rocaomrx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3niwhgoaa.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uplllkct.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tunuuynz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ywktlohn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zpfxjeyk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tjqjjfsa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3seellqsg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dfuugrvt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jrjakiyv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dlhjctmy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lobzmjbn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tkpgyvry.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wcfpdhba.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hpshuhdq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3fhcsmxoa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rbgfawsp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3adhkegmq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cmekzqgk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3sipfabeb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kjqpebfe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jesihero.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gzipsfes.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3srpypgdh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3slsbdbee.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vqqzgrac.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nsjqtlib.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lhriojxs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xukfckds.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fjenzssh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3yvweytvl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mgmerbol.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vbyozhjt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vzlgiuxb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kzwouqdx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hfqwjowc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3glxqvstw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nfslfknb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3okrpsnsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nwozuuaz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zubcgown.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nhhqbzaa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gpxqyoqm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3iijtyhhm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3iaqqgbjr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3esdtztox.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wlithzqh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fkdleqml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yshpnncr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ozyxoqpx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3nlqcesso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nztupluk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ambpklxr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jimygilc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cscybcya.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3fyppwejz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hxrzvxdo.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nptptvbn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tfexgyns.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yjewggwu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dydkryew.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3lvpbfowk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fufclxuy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3drvomdwc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ujqylclz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3cubmiwkw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ncokccjh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bippbkcv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3twwujqla.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qvrlbxee.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3rncbrmwl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3wgqixfzr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wilzzlxp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3gynjgaka.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lygtzgfk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lcljtqsu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfidbsfw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vgiqebjh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zwdwxfkj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3lbdkeqpi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvcpykxr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3witdwdjc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnneloxp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jencbeiv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3blycoeda.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shfzntke.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3stvzemhh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3orvmpgjv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svyuhumw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bctjrisb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kijbqmev.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mxmgrvow.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jkdeyovy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgxdmwzm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qvesutxb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fswduvby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjtmyqgq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hldtvwqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbdhwuej.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ejokzhnn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xnyjgxnz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3mxzxuwzi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jpgjwovp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qgcaanvy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dbnrzmtu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hzkmgioi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3kuxxnjkz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xktwnyvl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3goqjueac.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3vaphexgf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3phqzboee.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zsklhgja.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qfgybzmd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jwxdgncl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3iicyhpcl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fvlzxems.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hfgfkjlc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bzphzbbk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vfdxuzby.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3shcatfxd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bplnuthq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pykmefta.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zkwsewjf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3afjrbotm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mylxzivc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cjxsewvn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3thznaxvk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lorhjcox.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwycxkss.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xzdabhsm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hstfytot.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3sbaobmih.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3qgzktavi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bsyaccba.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pawyxhdb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tzbqkcan.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwpucaul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dbkwpinp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3znvxfdkq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cvpbgqxf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tgowujgk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ymxtlpjw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lezbkakf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ybpvbcbs.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3czwnkylu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rfledkox.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3twlpmopb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tcnoadyr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ninpgcdc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uiqpuwea.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3lyrqybxw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qdwkoddj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fbbhuopd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3imzxgmte.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fatoelda.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxvzpps.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3txfudhpm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rrplplpr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kgmkicpy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jnpoqtul.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ecoxcith.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3mnbruunf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zrgrzvrv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yjtczcni.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcgveqy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xoldiuaq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtcvafz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uchjilbh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gfkbvqje.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hbmmiklz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zopxpggv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bcvwswtg.html


<!-- 参考信息 -->