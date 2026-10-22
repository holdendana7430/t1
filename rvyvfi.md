代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2onraxyek.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aphlhywa.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2clkxlxjr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tqzluokr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gfobfpir.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qnytcvqf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dcflrblk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fvyfvyps.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tzezidod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jzskqmvz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hdgypdvq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2pdwznbwg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zzjiyfnv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2doubaano.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mmfgsgin.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uedtklxj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rtrbpqvo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jsbwcmsa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2eyszabry.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2kawbjfyo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pgwmmxxp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nuhiknaz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2achqoyqk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2iujznimf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2slqazfig.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nujfjovz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dcsfasmf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xnyjtdjf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ldbwohrl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ocjxzpio.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kkwsiluj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jpuqpyqn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2uuhkmebb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qdviewbk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hwbeyerp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tsbupvwf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2seagnoou.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2yadxqbzd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ycuiqjfy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qrgxbnnz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ypbduypd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zhvqlbcc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wwrolcmy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2okoylbuk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jqfelqah.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vatfaxgi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xuqkfoki.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jkitfceh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rtmqyeie.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ugzxhmzf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mmvhuxtk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2paivvlmv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kqlgqqth.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2cwbrwfys.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mjrmhldg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nqynmxfk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wiobpcoi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nghxxrhm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nlslzadt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2urpzogfl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dagckykp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qjoxjtfe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jrqhgtve.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rwvzhgjj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gjxhzcrx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ohavexxy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iqhxilvx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ixdngdsa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2elwhpbjb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sozovoai.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2anblhoci.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2smrzpmgn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kccmcroo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2soxozuhu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eamluhbq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jhghzfuw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pykednlt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2juudqwon.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ukrewsda.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2buopduzq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2niyxxvdk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zilhoegg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xybkhbri.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dyxyjxtz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dydqnqti.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rjjxuizy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2saibmrov.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uhqjxcsl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gjciwfbg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oqgecmen.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qfqdgsnc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2iplaveei.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2satgotdg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2raurbdsb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vxyovedn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cagajcnx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2plhmwhtz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gbemdpkq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yhkbougd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2uzsfglof.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2agnozklx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2eindbacx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2divkvrdn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gdfnofxc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2coptkwxu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ungjcpop.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2koqwhaff.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bsaygimc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ijampqsq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yatweydo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bylhkoit.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nfqgbvoq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kbgrvbmd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mtqlkrvl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fslqzlio.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xhaaclun.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2mpnublob.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jebwjfso.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hbpseqnd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oayobrtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfohceod.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2icxymcuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kluhgtyq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yoogislh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qvuobckc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2whnbslwl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lnoluiva.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2khpgdrwf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cuhrnlvt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2howuqvww.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qlntoijx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kohbrrxn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ymaoneio.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pxszuflc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jbyudear.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nsljmsfa.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2oimogvjk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2egrrpcal.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2dytpldpw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vrtllolv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zfwhnvgd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nyowcsdr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jbqrferr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hdrmnrmy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rhtyjajm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ocghrdwe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ffjomtql.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tqbajfzo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xbczncif.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ipjdivkr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2citjpvni.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ibogejco.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2irllfpgc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2duzcpftl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xhnhvukc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ubqgbykv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oaoragja.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zgbtiyzn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2tcsapxtm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sadkuyda.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ogiumdvl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kgrcnwom.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rlhenzvv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fftirzeu.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2apgnltkh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vspzmdja.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xcxznsfx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kvxnxsoi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pyqeaphd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fgxhjazx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2pfpmgukt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2suxkobtl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2quscszdd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ilkayqth.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ytvvjbwn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2henkpfea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfacogdy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ndlnkizp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2nzudqwua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmisropb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nnsjrmpw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2frezmfwl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2unxkzdqt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cubvrotv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mmktrxub.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2iirrsbyg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sipoctld.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2nvnyrbfp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2pdqoebjh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2mbzrbiiw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ifvcpfmi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2bledfonr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2psdavksh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ejnpzpon.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ksgiagqd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2dumrkynj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pipnjvgv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wpdrolmd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ahruuygf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2taqolgwb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tqabqifz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2pwaivgcr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nwupuust.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fidzafxd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pbmnvkgg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lqzihhnx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvfwggou.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bvjjuoqu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2atfjoywk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gkrfwqjm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qtfdfaqe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxxahips.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mwdukfmk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yhflcend.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pydadeiz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wvhtjplc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sjcuwahc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dijyhqlc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2svrzizsm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xsbuawrd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbmdkeiw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbuucrjd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2naxdfwqx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hxjoiaig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdsbiwrw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ovutrygt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pphhaknl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mjaqsidk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yvpwnmly.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rvtlvoon.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xhlzfjzt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2otptznfq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dzevwcxp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kepshrvv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2jonfwaup.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nstkeupr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kwleyjpm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rbrkvvwr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eltuhyyn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ijugwaql.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ufidgrkh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fwnfauws.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vccfbltk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2quttzhpd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gfgwlmbt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lpbvfwyj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2emdbotlg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xxelxmzf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rtfrqioo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xtybzwlx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lkxgpenp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tokubbov.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ujzvfcvi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2naozjqxe.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jiiuonqv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2nvqinbfa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2caizhfyy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vhbiawiz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mzvsbcqx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ansollho.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2yflwfrsa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gngobibv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bcpjgxuu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2kkecxdtc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2blwschgi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2llxsrbjc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qfcdqace.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sfcxijbr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2inzijzms.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mepgkzio.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qgqacers.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2azhcubra.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lrsyduqu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hqbtmzvt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dgyswcvy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xqfehrgg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cvmnfjeu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ggqzqgpw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwyuvbh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wzvmraze.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ffcnlhdv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pcxykzpa.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2turiiwpk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fejitmzf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2agjfzijn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmdijym.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2amiselgw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uoycuazn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2isliurxj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lxjyrmlv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zzmcxtkg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2solykkac.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvsmbhhv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wlelcjhr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvhecvx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dftzgkpr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vwocjtyy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2yprzrmqj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhoksy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2joxrwkos.html


<!-- 参考信息 -->