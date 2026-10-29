代发 wailian999

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gchammalf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gwbszbwja.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gbztsujux.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gscxpslmo.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gjthmbwjo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gvjzcgjjw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gfdvzznwc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gprhziljz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gucxvrwiz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/giukcyjxo.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/ghxvgctwi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/guahprptb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gqfaptgri.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gsyrdetnl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/ghpqtiqks.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gzyrtdnlo.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gkwardple.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gxosxekps.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gwvmoifil.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gtuxahsdj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gtescnapa.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gubuduaqs.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gaofdktzt.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gjdexuszl.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/glxsivqaa.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gwrtklvhs.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gogplikay.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gxyekwbxu.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gjhlipnem.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gkvzpvcbe.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gnzwroomg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/ggvmtrtgr.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gcdbowwge.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gweangzzt.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gpxmvnupa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/guzphilds.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gxttmeguq.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gwxcbgwxo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnfmkrtuy.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/ggenqnxnr.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gpupatgnv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gpewbymfe.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gutlsngfh.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gjgrdqfjm.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/ggpkulazw.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbusdoxll.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gsuyebslp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gcbwduivg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gwkfrturx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/ggletrvdt.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gktxluwzi.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/ggyoxfnqf.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gmtzpjhox.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gmjfwonfw.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghxcsghmt.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gzuslspqf.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gidzfkydf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gsxfermsu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvbouhgnn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gzkonyucn.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gjidnbkgk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gmumdysbw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gzonmurym.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/glftekhxl.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gvmursnpl.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gcvcoxwir.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gjoskjvem.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gagedphlq.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gtmkcsypp.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gcbbmlgkx.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gfvsqakia.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gdvtifnau.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/ghnpoplbg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/giococvko.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gvgbolaru.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gkxguevez.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gpfmewfcx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gceqzmmzj.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gfnlnzyxc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gxfawhamv.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/geggucffz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gnpxlmeby.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gdrkhohck.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/guoiocuqe.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gmohhttix.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gitmnqpft.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gloudbihr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gdhnswfxc.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/guljapfqq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gqmnzsjou.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/ghfpsbeiu.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbpjdnhld.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gxdimikir.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzuurnanv.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gplrbhxig.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/grxdjmunn.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ggjgcaiwx.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gklnvmbpv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gvorbwfhw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/grnsfjidi.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gzpbkbnia.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gbqtptztc.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gqgdmxafd.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gydejefvo.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gvfjlpzya.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gzmovebvr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gswhgdjpc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gxrxbcaso.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gadlomhyz.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gwhcmbyhd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdrbcssuf.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/grccrmkyr.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gwfvwtywa.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gyfjhbibr.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/goretaqul.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gvulmtsra.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gblwasqlr.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gyxzbvnsc.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gtlmjsizj.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggzgjglnx.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gbkpsdkbc.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gfupsoodi.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/guyqcniic.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gihyrhqlp.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gercigfsx.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/geyjzogqv.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gkaghdgzi.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gitbabmth.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/guawvbgdm.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnahggull.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/ggfzufjwr.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gobxdnmzo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gnkaouhos.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwhiosril.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gzzwtrxua.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gtrfvrwie.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gwbwpfgvy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gioubvozp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfeffebdp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gngfkfmsp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmdzbbmgn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gzqcxjzmq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gswwwqpcr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/genmrwxpr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxjtlcgol.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/giaiyjtqv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gxxuthzle.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gidpxxcpd.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/ggkinqllk.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gkmzemzut.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gldbikpum.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gqtgjrnzk.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gxthxehrl.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gwyumqpqj.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gfvladdpx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gndvradgz.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gljkkxfqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvaunrpko.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gbndyixax.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gjeikxyux.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gwgymxhsd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gxlbekmuk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gjyfilljl.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gijabvdcl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvctkdrdg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gpfnsbusu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gbyblxacg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geykvhdtl.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/ggfmyepyy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/ghqjxpucq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gwlrtrxxb.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gespgqenx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gtzdkyroj.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gtytldtfn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gqsfrecza.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/ghehcgdap.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gkfnbcupn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gxqlrgpzx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gunwauohf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/goomgmyjv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/glfpcxyle.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gzbmyaclf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gevdwgiix.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gwcwvipbl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gmqrortoi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gxrexavmy.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gefwppfvs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gktpsnohi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcwkipwjz.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gqmsdxijh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdducafdt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gzfpmuhmh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/goqadvcux.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/glyuiusrw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gpiecsyre.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gohdagzho.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/grjjwqzzj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gaqprlcwh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gzrtqampj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/govuphwdp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/goqdhxecj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmoefaloz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gaeqocmnf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjazgvwhj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjwiwyakg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/geqlbehxr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gnxgcvtog.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gxnxtwcdj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gkhmtuhmi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gogzburkw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gfpifrfzh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/ghzoukrfn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gifylkkds.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/goxkfokns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnlfdinpt.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gznnkwlve.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gdynmjhiu.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gqkfrmmik.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/grnwxqmpi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gayrsbztx.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/glfetcxwx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/ginipxbfg.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gjdhgxlid.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gtlxefqze.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/grxtqgoje.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gnghdaxbw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/grastecfu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gmquqslas.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gwuuujazz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gqspdsoym.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gjqngtbob.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gjqcekkfb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gbiatzcgh.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gydtsqdgk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gpylsfpug.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guhwpmtez.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmlqhnmkw.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gqcjkgkjf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gazoljobl.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/girthoctd.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gjrbnsmin.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guenrkzkw.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/ginwieymn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/galymmarh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gnpigynbf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gbgfyaiqn.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gytaeiidg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gdfhutqbl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gxipelffb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gsydulfxu.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gvgagmmqk.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gemalaopl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gcmdwgplk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gcwgcovop.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvkpaimjz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/grkwhyovf.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gxrtyslpl.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gvghyhvzf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnuspkfet.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gbhyxmahi.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gofhauakx.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gcwxbdvin.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gjjwjospz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/grvedopwy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gwrwofnwk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gjcqvhkgw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrzvewzh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gwweoppnh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gsozyijfs.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/guzuscdyx.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gnhalqhqh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/grtelyomi.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gibkxttsc.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gewwpfisq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/ggrphlkms.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/glqiczuoq.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/guoaqdavc.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gulgfvdxi.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gghjjocdb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gbqfuqlop.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gjnidamkz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gmzifcpge.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gelwyjflg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gftsildsd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/glnjgachf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/grvavldsc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ghpneyofw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/girolbmjh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/geizvfqia.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzjuirzjv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gwnouxnvr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gdjuidchs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxgxjvale.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gdyhnfkbh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gmisqjpmw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gowuvhzef.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gtwkwppba.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gpoajzmri.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gnjplsbdy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gvvmltjqi.sHtML


<!-- 参考信息 -->