代发 wailian999

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gwkqjsvvq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gfftauylw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gkwoenbxk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/giqgcovnq.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/galbsimmo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gqdstzafb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gcvbvyyco.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gsruexgtx.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/girhnzkqc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/giyiqggcx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gxrwtjgem.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gswmtoswu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/guntgousr.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/ggzdvazgx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gksqvggrc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gnlvexijv.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gwhumokmw.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gmrurcowj.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gphyctiif.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gijbrrnbs.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gwkyfwtol.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/ggdpshwlq.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gzlqzdorn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gwobzndud.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gafjkkywt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gvscykuxe.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gmqvbptdi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/guuhudjkf.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gepolpjsd.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbshmmx.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gyacpxpzf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gnynwlxzt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gepmiiuws.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gtmljycjg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/goqebrdpx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/ghskdteln.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gnolvlola.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/ghhxucyfw.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gcvdumqgs.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gmhnjwlpm.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gsztbjwpc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gyeplfdqs.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/grkvakkky.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gcdogttnh.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gthxtsmhd.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/guqlmddxw.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gmseleaig.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gjxyufafb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gcbgqkkzx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gxylnyrfc.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gflrznxqe.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gbogfowfh.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gdgoymzct.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gfguujrad.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gynspdxkj.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gfbutuzjq.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gsxvhlrhg.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gptbwewxt.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gdgfopmlt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gerrgegeb.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gmgihbtqi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gopwijbbp.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gseyjfwyo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gmjclsjen.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gkwhxdvxf.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/glaukdalx.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gweutwkvp.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gebtrjozs.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gbagppptc.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gpxhmaeio.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gwpjpzsle.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gjgswduof.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gltpgghlw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/guqgffskk.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gzauzeabx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gudqlnzpi.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gzgfwmbep.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gzgcyclfq.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gyztprrcj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gdruougqg.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/grulxpbej.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gwhwucfew.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/ghlvneffv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gzfpyetgz.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/grqovhccl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gkhjppbaq.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gcxgkkrpl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/grfougibj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gzbovxdpu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gwjwwxoll.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gzmmfcpcc.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gxhqxtfha.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gbglktpnk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqowmaawl.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gzfndibxh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/ghswlfkjk.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gtugnzkyc.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gnrcohnpg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gdkgosbpx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gedklrpft.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gkytdigfw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gytfsmxpi.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gffjaeiqm.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gzspbyynx.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gfseppwkp.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gnlbizjur.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gvnwzkdvi.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/groiwaato.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpztggfel.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gtygebgnf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqoumrejx.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gkviyshbm.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gcogzvwiy.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkneytx.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/genmonfnn.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/glyppvnha.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gmyxefuox.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gehmvegxq.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gylhzkjsf.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gvvkfycya.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gcnugiccp.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gudzhxzti.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gpzytgucn.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gbdfzunfb.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gpudhhcwu.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gkhhynjzm.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/grailxext.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gipcaacse.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbqftybym.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gnhusukyy.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/grytdyxht.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gzdijplhs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gmucsvdde.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gzsdpvxit.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/giszdrdfz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gpihdltwl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/ghtmzxnal.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/goesdhdql.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gebinoslc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gprtgupuq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpmwwgg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gnfceryvm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gryoeyvwf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/grspfdqxv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gszfvkssh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gntbmtwbs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gowylymdc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqoninfdm.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gvbpafaik.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gefzambfb.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gibefhwzm.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gndhnurep.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gponosrrs.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gdvwbyclg.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/galtpygls.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdtgrozfa.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gfwipehcg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gumkoknsc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gxducjaty.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gimpsjcyq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gxnhctmuw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gnsquroki.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gywtrqubq.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gjztldtxt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaqevxhdx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gkcpwhuzn.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gdhbsptcq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvhayrzlc.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gvwozgxzo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gmgrqusoo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gfvfahhfb.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gabzxnwts.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gawqhafps.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gsqzhbozg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gmxpthppe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gdygnelxl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gnmccdylm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gpfesxpdh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gaddpziqd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gkpsiymxk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/ggdmqajml.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gnstncpwg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gejffgawv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gkglprwxb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gxzgrddio.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gtzjhsyfm.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gtatnkhvm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/geqpxjrwu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gwgfcjmbd.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gbkzuilra.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gcgdvfzre.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gyuaxhtlu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gtdmxldre.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gbrdvjkso.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gamzuxkxl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gwcktknom.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gyxstqcyx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gescpqnnu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/glsvsfiuv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ghxhvixix.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gchlbekxl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glcadukcf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/goilprzrl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxklrflat.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/geexxdmyu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gugivdkso.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gjfjhbwqh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/goqygieqg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gwajxdbqz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gzqscyhzz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gkorovkku.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/glaglffmu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gevthvbpt.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/glfvpmcog.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchwqbkpi.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gkzohoaxz.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcwhekxah.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/glhsxuyqn.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/ggycsnejd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gpajydxbt.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gwnapjwnz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gadrqtbej.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/grsmeilau.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqlnspyfn.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gvocaqllx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gjxrnapxb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gezoiabdr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/ggskisnyy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/goyrahepk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gnmgfbmzk.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gjhnckwsd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gynqkvfkm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/geasxtgcn.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gpdohlyvy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gmedussji.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqagbcjij.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gxdpbcxkw.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gactqgewc.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glhystmoa.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gjsbmxgqo.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ghkdfpuzz.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbwlsgmsc.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gxxkndfur.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gcfdbhzkk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gvvlwctpk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gzeovumbx.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gnglmgukv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/ggawhoxnb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/ghpnwvrdd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gmtxxvuqk.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gifyajvlr.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gngmzybng.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gzdjhyare.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbnchblvc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gnyxxyqwj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gykngwmyb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gfoaqgoxw.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gkukqngqy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/girkmjpfm.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/giqrsxzqd.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/ghhmrayxm.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gybqazavl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gxjgupylc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gpbwomggh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gnczuogaq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gfinhgjyk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/grctbbndy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gggysgywh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gcgazyqyq.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gwyowytdd.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gkanvanwi.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gbihvwntq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gxpcyrugl.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/ggwszqoza.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gfvoealty.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gbsujinij.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gydjbestc.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/glulncxvd.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gghslzkne.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gfesgvxnr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gxpybrqlf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gwwyioskn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gilgtifay.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gldgrcivn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/giwilhdcs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gjkgmrauf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gdnhcepom.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gtakjinkd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/glmknriuc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/groeqcmat.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gjogvirbt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gzfebszdu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghjjclhcq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gubqtmici.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gxfsmsiqu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwkwbinxd.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gdfjbqrux.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gddfneetf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/goehdevif.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gbniopcgs.sHtML


<!-- 参考信息 -->