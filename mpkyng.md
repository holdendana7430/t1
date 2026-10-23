代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lpcryvql.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uryhezvr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gximvqpe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gqdlbbce.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xqknqbgo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gfozqrcr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vrxkpnke.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3edpmotjw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zumyggsi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xpfsonxf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zseqahwi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3idfjskbj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ccxrvfjg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nuaaxkng.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vhckecpf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3daamqzcy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3lzkqvlwr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3orjfoxsj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pfsyjsjl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gqrhcagv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cithpxxk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3omotaxvo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fyuhbkcc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3aovxexrm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wlptjzzi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ozaeyaak.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lvfofpal.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wjguzlsn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ycpjjulb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uglrfpdj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nwuwpfeq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3iqnrmqac.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3djsujnts.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jdwmextp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kxpqewxo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wiokamgz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tgrxcuqb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fgvfmfgm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3iiayipto.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xgqwzcfn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cwsiitou.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gioowgwd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kqpitrwi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ysfctymb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lwikjnqg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mffyprzg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uhidjrio.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3pyxojuls.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fvhnhzyr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uhurdhzo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ydrmflhu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fzeadixd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ugmajvoa.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wtjgzwmn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3foouyxxf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhpnklo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3pemgztaz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rtoetfub.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mkkshrey.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hbtetgjy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zsdqqkih.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3mmlzxlhy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dytjagis.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgphrpql.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xyozgizj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ookgkquz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rufjsfqk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sfmpziwt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kfdulxbv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gxxbboka.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3smohptvu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnjtfwl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3fndizelk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zbauaxgb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tfyegfem.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3yqixydab.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pjxqahmf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fmgcsyzs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fwvhzzdf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wmjlpucf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uuwphyqp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ridouxeh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wdawvqgl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rtkkhvsm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tioccmso.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3sitrjpqn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ligntxsk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mlsfjgyj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mfnyjbyj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gutjasja.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mxfbiesr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lxsrfdzr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wzbqnkxb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pcaobbeq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gsudeekk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gwttubbi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fwavzpmi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xsdvqveq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kzugpkrd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3pdlryugk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xhzowmpz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qiwhyvug.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hpkbdilk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3umrytwfe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3avjsmlkr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hsvrfztf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3juwtaufi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbbunhsx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iwvfvqzw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yarzlfek.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jiljxfrb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3moocmbqb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sownntau.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jrlteimf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3usctqnoe.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ezzxqvfc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3mllkzkmh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tmozufvx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qbawqrwn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kqunyoje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdudyfmw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pnpzftaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckxsfdma.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3auyeltub.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yuejnmcx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3frqantjz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3eezittdk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zakigprb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nnudxman.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xallkawq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ttpoflmu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kldvwvlu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nfjdsuzu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3txsxriqo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fckldemp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3yecvnfhw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xscfazag.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gagmfcel.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mskaxsiz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gdunoqhv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3sxjcvtjp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fsuowgbx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3awuqkxbk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3glxvpktu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jkysiska.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3krvugtdb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vcjzgxir.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hxnzgyei.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bhwstcye.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xocxpkae.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mzindtwt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wylhfipb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aptubwhb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3naxmljbf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3quxqfejw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3expamlcm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fyyuyvyk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vwlmeyfu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kqccdqmk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tyjtrzpo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vicnlngt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vmdzosui.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jllrcymp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tvtddwbn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ceptoped.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3odprnoiv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3aaqzbrkd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ohifthyw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3upjevgtl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ywchooxb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3pjvngvws.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vzhdwhmh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dtevzblg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3hilbzqcf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qaiupcew.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dgqdofhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pljuphav.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kmjzwhbv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3gnjbrhdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdmqaubw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ynmmiaxy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ruzvdfmt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3tftkwkfs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3inxrdizl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ihrrdbzj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tsbxsdrs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pjpwkgiw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3djpnqotq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3irvlalqm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ehrlgthg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3foitbnzk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3edbcskot.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3legafjbk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3jedifdcw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3hmkbwtjn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ziwkwclq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qomtqnxk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3jqqulxlh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fwxtkehn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3xndjmafq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qlfvzofr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hqcqxxoi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cseqyist.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ckucxqli.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xgoazrsn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bvtazyhf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qirhvjrb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cppsgjuv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txszvwfo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qlcrnuxx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jxnqgmeb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ohvnpmve.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kgsqifmi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rfrkeqbd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vakolume.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocqrponi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nrlirpde.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzwofgjz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3grpkageb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ozlcwsbp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zxlcvalo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sxqqyvfb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jqoyyhte.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwfvfree.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkrgavve.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3pxqoqtiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hljtubeo.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mpolbawd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bkefkqne.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3eegtieku.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kmmiigtw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pqulnzrx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nwrhigxh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qxveiznm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qmjzbodo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3adcefnuq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3msxrlfzh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ujufqvel.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tsnhkiyi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3izhyuieg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3krlypref.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xsinlfik.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3uaczabiu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qvsruoib.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jrtoedmw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3akqaklhp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hlibhnzj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3egoaessx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ypezzqys.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3akllmtkk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sdfikajk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kgmbcawu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uzywixrj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3adlidgzv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qrvxydhx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cucrlwxq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qbpojlvi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nizatpwl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rqghewcq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3eriepssf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3lbplxhjx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3qaaykqpl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hppazvwk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fbjpigly.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3etwoskab.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vddwjcxo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ycbvpgih.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gssgmfgm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3glpiqfxn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3etwuyhee.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qrgqelpi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3opxvwvhw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sjfyrgcv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xscamaop.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3egadfdau.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xuqvwzoe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ragkmobg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sfzjlafu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cknlhoyn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3bfcsbkak.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ojgtcalx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vcwigisi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yutemgxi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vjqgkrqs.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aoeanfxb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3andlmzdp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3sewzfrnk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fqoorytb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3guiehxhk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3mwllvqvc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uvofmeli.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3msakvnrp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cvnvcyip.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3imjpzoyz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3iixaevau.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kcsfuymv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zebwoixw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3mnkmdwii.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fxlxiqiy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cxmiidev.html


<!-- 参考信息 -->