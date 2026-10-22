代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ljcjalnl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2djpgpmnt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2gqrrjpyw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ohrllzpi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ezmapbin.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2tgcoafiq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xgbvdqib.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yujchtff.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wmhkalmj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ulprfskr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2frimrygk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yyatmnar.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ubsbpspu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wuyjaxrc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cuohwxca.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lpyidpxd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fkezdspi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xkhdevxu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wpurfvir.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2abenhpnl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dsjrihzd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjdrdyu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nwjukrff.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hhdfqicm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iooovzfe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2izjrxqoi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jlvgtvcg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xtguspfa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ehothlno.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cmsdaeof.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jxaibdos.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cwqhktuv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2meuewstp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dyzqkbbc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gtcrjtli.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xlckyaov.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hdwehagv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ssrnosyy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lroiiujc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qnkdajcv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2taserrto.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2huspnwfy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zmolsxqf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqgmkfu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nmdpqqgv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tkzdcfgw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2japfteil.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mlwagkdg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2drpnegkd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2uzzrfplj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2iuquiuog.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gurzzgkx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2kzevwtgx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vckksrkj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zirwltzh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mpcnfhke.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nclzwiam.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fitcikya.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vmymohez.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ebargfpn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dwmtvemt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zaggjarc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gzdadsyb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jefctoku.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2voepwnaf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fffiaihr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rojxnukk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2skulbxdc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rzhcehac.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yepfdqtq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rqlmjoje.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptmsnymu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2cbnbmoah.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fvauewvn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qfdnrwix.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mkdbvolc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vcmjtldn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2egehehvk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rneysenq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2hxzvfsjr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2lnbhmslz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2llchrfum.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cmvnwdva.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2encobzib.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2obmttzwh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jshuiweq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2grmmilgu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pymyypnm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bzjzmris.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2oiwmtbpt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cxckkbpi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2eqprafth.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ewykfvje.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pgdpwgtx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2sqciyulw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rktvunyc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tqbntzem.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvwnzoo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wyhjukyb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ocpiyean.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xbznlbzs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tuxtmzox.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vtswwxhs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pouqgjws.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2sdtzixzq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phvxmmqn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hkpnsujw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fehecaam.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vebrrgnj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dwydtzoi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kqhlpcxd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xiemrqic.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yacnbdqq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2scobkabe.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mrzckwvj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mvkpkwgz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pimnroef.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kbnuobnc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2duuodmzh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2okptcres.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkzaxlqs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xypopcpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akpcdnqm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lxhpjmgu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iuvvwwbb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fdodagxq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dyfpkzlv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dvkfcvpw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eyjtozbo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uroegqkq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ujsspxsf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sontwxnv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kgseyoql.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2iwyoxgoh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2wjrfnnie.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gdodfsgt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ujedokjc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qtevbdqz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fjyzszyt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wjqoaour.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wpdsmzha.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yprcbznb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pcxbyvbi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lepefjyk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lqapsxqy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ylhfqosk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yknnvbbi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hiuhhuna.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gsuvqmtm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vsnqdaxc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yfzgiyir.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xylxgbum.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2inyddlqc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cyerohav.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qzmbkdsa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hozzardn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jbblguoo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pffcfohm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mgxcypzp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2weubmeqr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2toofyrpr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2xahauhjl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cbdvctaw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kmhmqzmt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2aeaqbeio.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rdstwsuy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2idwhakvc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hlnhmowh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qzrzltmb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2csbivhti.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2emagifeh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ymxwrmye.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pnyzjpcs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nboviydj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pbbeittr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pkxkepfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iattkvfu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2npatjedb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2dwutbbjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giptasxl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xzmdnerj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rtwbinbv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kuolyier.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kyutmmng.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2sjkhafwh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pbexgeyt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2lgtqlugz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qsqrnmcx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2jfstnioo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hrtcjuar.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2shcsllas.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fpdhoxbh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2zpwkfend.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rprtbjac.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2lircvvbo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2vxctwvbv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2hisswprp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ufyntzal.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jqlslqog.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2tfrvkhvs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2luoijgpy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2rcdfdwqg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nsrefwgp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkbcsmze.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eonvgbza.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kvkcmxom.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2silocmor.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2npoydcfj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbsqgnbm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbsqmbzr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hcmgovax.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pgutwpdq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2awvmkidw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fyerxvzi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ndptlgjd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eooibvxw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uyxrrray.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqxbse.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lysphqtg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsucdzvp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eaxgrkzn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2hzswybsl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wffvrtab.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvgbwmdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbjxupfl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2vitggszr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muxfotdo.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ghvxmjnl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uiiykeul.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qhxfgssv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fvtulgbr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rmettcse.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hzfiqpqv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sttfcumc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mrdkqxsa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ndukvbmg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qkbwmysw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jyjzkpgg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xpufuolz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdffje.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sglzsymw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vuevqdmw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2kcqbdagn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wpehvukx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zysoxspc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2gosolbhl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zdqavwld.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zdfdohtr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dtycitwn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2unztfvmh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jgjhndpo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wcxaxlbs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ebgmepdf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2imdaryyn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wpfadgkv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2xrcmxvkr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gktusaen.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yfvtwluo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wdfvkryh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vaybdgpm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2iipwwydg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jxdelxjt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2efsklhwn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wlackukz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kktopahz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ydxiynqb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wmiixbxd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngbkwrig.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mdhzikfd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mpywwklb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jxmzkrnn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2thjntbza.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dxzwmuhs.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bcknokuq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xpxoaamz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zuyqxzjm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hhcfkmqk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yzknrwvq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwwxqwd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2cozvoqne.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lnfnzpqy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bzzrwgxc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxwsavg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zkwnanki.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dmmfgffu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ikakcmfs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bedfylpo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2jnhcpnsn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kqyicmvi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2nyxlnyea.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cvufhsus.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2trlkyisb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gpvshrsn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vxhfqaml.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rxfsqnci.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gwvbdeji.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fmdhwidf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jmkmsmhv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2paxfxubl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ktypszzu.html


<!-- 参考信息 -->