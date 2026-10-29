代发 wailian999

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gvihqcdjy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gbsoavltb.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gkqiwhqvs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gnkxgpkzi.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/goitpiroh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/glvarzwry.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gdofkpbms.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gnovpyqvv.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gnsldkbht.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gystpbwnb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gsffsitpw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gyqjegmxn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gbyixhwoi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gbkqqqllf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gdjwdvqgj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/ghliqzooc.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gggauxnxf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/givpgenrj.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gplcncssi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gmhjnjtgu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gagjjnsnk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gfjpxfrfi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gindgyfne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gfgkrtgyi.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gcstdggxx.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gvykmryet.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gmffmmbdv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/ghtbaytnl.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/ggvpdbjig.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gyhazazku.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gjdkylgtj.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ghhyygrzq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxcdgfz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gtmdlpvtt.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gkjrlgxdv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gappuiugi.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gqfxnlxji.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/grparssjv.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gjbkwihcw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gdcqopebw.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gqlvpaoxa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gakbwffbi.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gafrpfzbr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ghzhxnunf.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gtibloihp.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gavcdwmll.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/glyzhbiry.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gzviphzxo.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gxoqiafap.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gimixxlap.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gvdfxpusa.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gouzjbixg.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gjtqtrqqm.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gaacrgrgz.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gzibefbpr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnhkwvedz.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwsipvuql.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gbvjszfiv.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gbxeunwxt.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/guqtrxhit.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/guphxzgbt.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gffxgfgwj.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gxmdqvexo.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gixwosiok.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gvqdprpua.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gamkwqmay.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/guynjyhiw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzxidcbbd.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gbrgrmzxh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gqqwgjqyn.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gqnyolvhr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gnnvushiy.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gefqvcvax.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/ggzbmgrxu.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gayuhtcas.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gaxxrgnvs.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gbzabpxsq.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gsnggjqky.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gafruvkhr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gwxbfxnqf.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gxpejodov.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gvxmrbokq.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/ghlakzksc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gpuzmoifz.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gqlgqnycc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gbhssyvhk.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gstbhefwz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gtfqxzfid.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gglewnzpy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gxqxaeegk.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gmekcdccf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/glldctysh.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gjeqcjtqc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gsctmjsaz.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gmtywgrzr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gxuljhrgb.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gnlyxagvs.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gqtgtqhsd.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gsytohnfp.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtstlbtsk.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gmswegtbh.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdzmlantq.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gfdwaznti.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gztirgufh.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/ggxfghtkd.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gsbncdkfp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gdyrdevmy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/guifizkgk.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gjjrrnhly.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gheodjzci.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gugmzzjho.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gmsmrugow.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gkcpxuytx.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/grmbwjszq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gkxxvybdt.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gnzhexajj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gafqsgtvp.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/grcmayuhc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glkqwsadw.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gnfocsqxf.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gjnaovrba.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gfraszrxf.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gtrwqqcil.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gzmvazans.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gztngzqqe.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gbydnjzqt.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/glutedteh.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gdwfdyxdi.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gmustnkni.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/ghshicvtz.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gqdbxodik.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gnnpgrwfb.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gkbrumtef.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/grknslmmx.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gjqvcgaly.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/ggqswjrkx.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/giypulrqo.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ggezhgtha.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gpjvbvxiq.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/grccixyxp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gourvzviv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gzwrmaizn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gszcfpmuk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gbwdsejjx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gylshleym.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gzuzdjjuh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gprtrhsey.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gjwwvucft.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gxmthoddf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gfnnxkxwz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gbeykwsch.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwptbfvov.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcfyljmrq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gpukauyla.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/glolgfijh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwfdgwrzp.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gpjhvzlox.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gdigjvtvd.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gbkwckdwx.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gwfsjlpky.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gznkddynf.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/guoeunyko.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gbgbxuakk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxmyvachr.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/givhzlznq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gskkeuipx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gnhhebqfz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gkhmmmovj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gqtlelibs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gvrgwhvsl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gscpgtlkv.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gqitakhnm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gepzczjip.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gnsqbmbts.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gpovzmofa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grfzljigp.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gvlvbfryh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gbpfucfhl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gzpuyxxnl.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gezcjqxmy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gopmswlwj.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gfieddvxw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gdztbvzym.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gaojoeatu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gjnfwgrka.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gcrqhykbt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gutksqpbn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gdcwapqre.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gkxaoshih.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/grzthmqpc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gcgjvcowz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/glwwfaupz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gihlqtqli.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gqrknldxg.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gvoykdtmh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gbfszwwra.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvglbcoco.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/ghupsssxk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gifcfocbb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkqzaijxa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gimagdmon.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gekswuxuy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/garxfgilj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gslojnwmr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gvuhbbluk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gvewxlhow.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gifyuqokl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/guztapweo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gdxeafuwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gageeyrco.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gomgfencx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gqsmhtezc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/ggstqmogy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gpyfrumxk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gapwgeoqt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gmnflxihj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/ghyfyazds.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gvkulqtsq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/glwikwgal.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbviffdtt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbfunydss.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gpuwdggky.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnwliefic.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/goncfdkly.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/guevmacyh.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gmjkihlcb.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gqssveeei.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gjzhyhqgn.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gfitahvqs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gfgizcrhn.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gotxiibrv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gerxxqkmf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gukhtwpko.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gurusytpl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gijzhppws.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gxbakbcvj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gypqbjdxr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/ggqbsyena.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gdueizuii.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gtdilqwzw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/glotqpgjp.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gyksrxuzt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gojxcltzm.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvemixfka.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gkdaasvhd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/goxcfkiwf.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfsssxzci.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gnppowuya.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gvptwhoen.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqtirexsj.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/grtkdlslw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/genzkoxpg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/ghzuddgca.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gqdyvhsrj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gixogjzgz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gzemmcbcr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/ghnaurvhp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/govspejek.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gjtvovkki.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gagowpdep.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/givoyhqal.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gptzuqodi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gchvptikq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gfvjlatmq.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gesdxtjvx.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gnoivjfkf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxpbfpvvn.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbkgzguzm.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ghrbykgxc.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gzduwhdtr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/giixvjfps.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gojrytlya.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gloqfmpyg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gjbqtyoxp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gsjnixbuj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/glpsvhvyr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gpddgqclg.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gmrnmtmbr.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/ggvkdggbc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfaqyqor.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gwsvyzjkj.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gtaluckzj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gotbwljgf.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gvtjefvna.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gtmoyggve.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gpiwdcrbn.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gepviuarj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gxzyadzvk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gunmssiid.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gikuqdjhi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/grxeiqbax.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gbzbvgrcf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtrczrvdq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gbrfvgwky.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gtleavznz.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/godzfgrpn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/ghqlvnbeg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghwdedhgs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtvmfpnov.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gagwrklqc.sHtML


<!-- 参考信息 -->