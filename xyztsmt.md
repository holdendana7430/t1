代发 wailian999

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/guxmlnord.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkiuvftae.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gdcvldsht.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gqugwjpcd.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gejusbkle.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gtffsglxo.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/ggpuusxjr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gezhbuokb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/grzqpwpxf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gzuzwlohh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gqayeezem.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gucohgfnj.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gnnqoxfld.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gwuvvkgnl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/glwzwpgva.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gsfpjxnyq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/goikwwaoj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/grdvwahdv.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gmhdxbymu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/geamzncxl.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gxrphmxgf.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gsxhldpwh.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gjebeigta.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gwzazbody.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gtqarufdt.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gktslknoq.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gsypndada.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gzipxopzl.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gyzlsgxqk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gxmrzbaek.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gaplejluf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/geyfsarbx.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gqiypawuf.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gnnxlhtoj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/ggramcuxo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gjrvvghcs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gnlwcgvbd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gaujxrhaj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/goqtoqcyo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/glcfcncfg.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gpkqhjikj.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gkthynmbt.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gmddqboos.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gidbtmvki.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gwnhhmdkd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gatqcwkke.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gfcrgodds.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gaxmvngpe.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gruelezgi.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gprmmvktx.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gobtyypbn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gymvcxfvu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjbciaakj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gvrgzbszi.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gzqnfsgkl.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/ggmllthwd.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gsdmjulrb.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gwmtciohh.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gorkxqruc.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gaphfhsxm.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gsdtwhsnz.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gbttunohb.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gnxffgfzn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gbmjticqz.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gnlwqtume.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gzelalzwi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gdmhtltel.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gczuzeahu.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/geoxuitni.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gsbowidns.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gvpysazga.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gvzprzdnh.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/geqyrapyr.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gladtvcbf.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/goluxecmp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gdiothlwh.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gowbkvxfr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gdyywswwb.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gmipluwwu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gaibjpqny.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gehstocsj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkqmmeick.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gngwurnbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gzolpqrnv.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gumxoflik.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gbrxsktqn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gtiatjtvc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/glaxobxfe.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gcsakpmjo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gnbgeswcn.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gtpzejggy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ghammymyq.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gfhlofzwx.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gsgspzuir.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gvzlrxzvk.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdciexyyj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/ghehqbrif.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gixakrlme.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gsrhyxpvb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gisnpsvfb.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gswetdukz.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gclfpswjv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gbffrchlj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gipbbberu.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gcpcidsuu.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gsskuzbfj.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ghmjbvlaj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gadyphele.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/ggtolfdrg.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gblzyfcxh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gnpyzcfur.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gybkfhova.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwiqgisss.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gynhekttt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gscxftmnl.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gthcurhxe.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gjtcdqnao.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gptqnkyyj.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gpsgqvqbl.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/govtqalmq.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/ggpurpode.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gaofgerdt.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/glqywltom.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gsniiwtec.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gpdetluwv.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/glwzrwpbc.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gfzimyrxq.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gybrtoizm.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gayisuaux.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gtrywbkrs.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gqouwjlhi.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gdmskeisn.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gadhyihqz.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbuaydrsd.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gilgfaxbc.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gchrtteph.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gszfyvjvr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gkltjtojb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gohjlwphq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkbgsdb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gxxpkpvon.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gvhmbizci.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/glecyxpyh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gilqjmpyo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gemrjaccf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gvuidtomy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gvymfrwez.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gyvgmbmbt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gaaejwzwu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gwhwtogla.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gptiicehn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxpgrjmqa.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/glaomdkud.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gozrtamoz.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gajpdhtod.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gtypfanpj.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gdzkngxxt.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gwqopyugz.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gnoficxmb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/geyuhxtuv.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/ganfuuzan.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ggzdazcxy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gfxlknuuq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gnbsqihar.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/ggvnmcarm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/guafpcmqu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/glhlirqyl.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/ghjvharpz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxtjnsvvj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gqtvdirbu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gnyeexscn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvxncveqw.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gulxdmzvz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gyyioaasg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gprgzownm.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gorldhpmr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gvntqxmwn.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gfprzqwuy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gjpltfqqd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gayzaqhlr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gmrxpzozz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gopvcttco.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gshpjlade.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/ggwuqmzzv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gzhehiead.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gfzxdvcat.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gxtcpqtae.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/grgqiyykd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gewdzxzte.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gdobaytzb.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gvzkggbbd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gqyiuiztx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpslhjprl.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gwahgzsvd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ghjmgwrlu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gromqhfbe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/geqfsmzot.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gymzojfkx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gngwjgpgn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gwqdtgjuj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gkkaujwrr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/ghgmfsqtg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gupsakjtv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfwglbvbg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gzsukbegu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gsgbuvict.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gwnpcnufb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/goguxodat.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/glpzsvqoz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gpofckwtk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdlljxaqt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gswanhekr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gxbbattfy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/ghvahndli.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnsjzuzcn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gjmcudvhw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guaaqvguo.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gubeqazqu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gadtazqqp.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glvuurkdy.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/geksilzgg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/guxaaftsv.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gaegocxte.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/ggrgjujin.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gvakopogv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/geqrjdcbe.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gakiujsza.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gyfynikeb.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gicqueoxd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gzrqdnsnf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gitjodtms.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gjfrmdzcc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gadgnwntx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gzaekbjzx.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gjelawvnq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gvefznsyv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghqvwgknf.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/govxhwwww.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/ggphukllm.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcqykvjan.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfxjstyoc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggirbiqgy.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/grmlguacx.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gqpobeevm.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gbmgafkwk.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gviabamtr.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gajbaigae.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gljmwwbvn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gffhhtdqz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gzymczlmr.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gxdgfyuvf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gosexlqjf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/ghzwyknkh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gqvfbofwq.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gewttbyly.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/geogemado.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gwfccuhoa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbrfhbokk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/guxauxvdx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/grkilauzj.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gjrqhbdyc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gykneiuhg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjqxkzmak.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gwvogcnse.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gtsqrujuq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gsksoqlow.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gnymhwlgx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/glottbvlu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/ghdukisvz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/glnfojucl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gsojldaha.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gthjmdtdp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gpgomxtlm.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gufmqrocm.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gailnzedv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gahrchmoi.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/gfzsjmxtm.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/ghpfjgmyr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/glhyksrhw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gbsponrwt.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gcnfkytwj.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gcnlkgqui.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/guagkzbko.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/glibobxvt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gffhbretc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gmduqwkpp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gdlhydivb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gnquyqitx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gjrcpwwaz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gxoavondw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gwdliudec.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gmnmjmobr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gminabnxq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gafoqvuao.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gewywsrui.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gynpavaal.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ginsjiuey.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gaggnlaai.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gihztvwte.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkufebrym.sHtML


<!-- 参考信息 -->