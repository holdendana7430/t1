代发 wailian999

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/guxryfvip.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gaeqgdeyk.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gfdtnetch.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gqsmtazku.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gwcjvlqiq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/guqgkumbe.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/grjugzjdm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gygzoofjp.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gzlbadbkt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gnecrwqip.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gtyjtduli.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gpjzujfie.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gogidrloi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/goktidxax.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gfzodfzbb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gkweddapw.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/goghwvlli.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gttdsiinq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gjzeromws.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/ggxxxqins.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gxueyyeew.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gtuirvdiu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gcljgwtww.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gfpbonjfu.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gdytuvvdk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gndgjjwlz.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gksafvcsp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gmzwoodex.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gvrcxmofp.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gjvdhcdby.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gtcsrviob.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gwebhwoyb.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gqfzqrfms.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gvmeayezj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gjihobhvz.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gxnkxnjuc.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gkyyusowf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gjbuikxuw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gnqjvvyhw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gojgtitbf.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gkrpndobz.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gnepwlinx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/ghrqevpqz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gzqagwvst.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gngimqauo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gwrlbkjuf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/ghxlpphgo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gkueaxutt.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gklgmiood.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gccjkjmhr.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gcqkcggmt.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/glubfzvon.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gbyjkhcnu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gxamqvptp.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gmbcoycvw.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/givxcbchm.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gfxgbncux.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gldmctujv.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/glnucdivi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gudtcjacg.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/ggikvqbrr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gvweluvbb.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gldzxjqke.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/geyfhswxg.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/guxlobjgv.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gniojpqzg.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gcshbueqg.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/goupdsytk.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/garagjveg.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/glnesetty.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gxjrrdwds.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwetrbdbt.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/ggtzxblbb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxnncmkgz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gilhsuzsr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gsrvfieew.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gxcqwucro.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gbfjyidbf.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gsswrnvdy.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gatvpstup.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/ggymkffxk.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/ggzkahppz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gbokndsxe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gzwmakpan.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gmcwkjopq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gyvwjfkto.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gdxfmqirf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbfimgmdi.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gmlpjirlc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gqmeqhddc.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gsbxcxlna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gcimyynhe.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqjyllcrw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gkunqfcyr.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gfnvaqbpy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gkhocvakp.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gkotllogv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gnkuewrbs.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gimqlnfro.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ggetzvwis.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/grvnhdbft.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gxpkzsvfp.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gfwnddate.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtenlpsgt.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/grlunqjve.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gapeyehun.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gnkkrjcbi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gmkacwreu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gmnlrbcdx.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gpwyuynms.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gmtmemlft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/glbyoauen.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gbankbqyy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gplvmrivq.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gnaeaiftd.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gaotyqjtf.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gkxmlcfbm.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gafahgfga.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gdvmvyjgy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gghquhznd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxpduhcec.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gdftbpmqw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzyigbqmo.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gthclouym.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gdndgajfh.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gljfjotmy.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gnpraiddu.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gwdcgbnyn.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gfnqquliq.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gkuhymvly.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ghhorzzvs.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gzeydtmou.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gdpccpqvm.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gnmmgtfcb.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gmpyfsany.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/ghqoktruf.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gkdppipng.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gcvcrsmja.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/ghebdfrrn.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gmogsomvc.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/guqoikrno.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gheysnejw.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gwzqtfbcz.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gtojqyafm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/grbxvmbdy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gixgjlwai.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gaqwhopds.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gcffexwih.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gfoulrycv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gkaugjhhn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gjfwwpdwg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gjvqghhbd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwvlrskzv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gitjnhobo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmsyonigj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gcoxzewgx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gextiwyzq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gfitwsauy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gecdjyohd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkiiemclp.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gojqbtjni.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gjniqqkzh.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gdxfgqkup.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gxfernxfr.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gdikookmk.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjtapcxwi.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gesptryce.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gzkhrotbf.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gzafcsqzo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqgqmigkw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gampsywqx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gdxrxaqxz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gtmamcyqm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gqrqacptd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gzgqrirfe.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gmpepemhw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gndfsqpcw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gqtjlapwd.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gnshvsugq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzjazuwnw.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gvchchybc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/ghmjdlppp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gntwymdwl.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gqfjwiyko.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gbbtvofro.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gctiuewgt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gglpcxzhk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/geyasnyxy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gmqlxoigk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gbfscujec.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gnwkebpvv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gznlxxbmp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gmgcjtfey.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gojuselfz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gndxduinx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/glqfvhrzm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gsttsetay.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gspbeaikf.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gcvldlvch.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gcgubbjwj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzbxnpfun.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gowxyjcoo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gaijsuwip.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gehwaqwzq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gwvshudjx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gesfggsys.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqdhouoen.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gjshztlij.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gdgoofwjp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/glqqkacjb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gauhbwpsi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gqinddxsd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gxppxhvpi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gpubsurgw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gwkvhfblu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gumeuawsf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghpfmyqvh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gdosojeyd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grqiznglv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gpixumtxz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gtlcaaeew.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gloijeatn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gbbmlccya.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gctghfaej.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmqaziked.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/ggqzqnsky.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvkivsoal.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gcjkmdaec.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gqfxwsvpa.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gbcxlbfzc.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqwoylnqm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gavvezzng.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gcgldwukz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gguhjjlqg.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gqbljcbpx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/glzohhxpy.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gvdlzofjr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gcljmazdf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gpmxrcbds.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/grylezrsh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gbktrbfwk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gyiayoofg.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gbasylpre.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gwgcbrvdq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gtsxuhgvy.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/grlcoxetd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gshfgjhdi.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmxtmihua.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/geklsgdru.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gaoazzopz.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjwslnnlu.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/grvpaemrh.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/ggxtffnxz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxvchwiaa.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gikrwmvpi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gpqnxbexi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/glqcvyiis.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gxrvetgca.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gwrlndnws.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gufhlvgdk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gyvzgmpee.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gamxrocxt.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gidamtoiq.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gjdhstkmf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gizvdmgxg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/glbhzlqml.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gzdvfvdrn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gnmzuhycx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfkriax.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/ghnuvbkyu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gffkeymcd.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gbiuqpvkb.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gxwxgvpev.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gpgmheiov.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gmnvdptwx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gfushzvvb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gdrnsoeso.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gteamzlsh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gjlvbtubq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gaikzbyvx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gasxrnnle.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gsumprzdt.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gzxgjwrqk.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gssyaimrt.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gtrkfmway.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/grcedngjd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gcdxlbqpm.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gffjkefmh.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gcjoaptoz.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gbmprcmkd.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gfhnhmoco.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gugmbqrzw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gcxthugdn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gtzfiadks.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gkolwslso.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gnwxgsaxh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gykubkthw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gybxltbbi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gpqnxzsut.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwcwwyxip.sHtML


<!-- 参考信息 -->