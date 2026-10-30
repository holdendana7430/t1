代发 wailian999

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gpmmimwur.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gjloyjlqu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gtcylwsof.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/ghvnjajia.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gfwuilgkt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gssuzuthu.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gbpedcusr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gequswads.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/guauqjnbj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gacgfgpxg.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gjsqpkber.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gzdwbyefa.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gszrmagpv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gqviaqakh.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmdpwkodv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gbdbtbosd.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gwovtubyi.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gwlrxhiig.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/guizwqqvx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gyoelotix.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gtlxikicg.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gluocpldr.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gdcftkimj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gclhenzhf.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gqzxwxgck.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gjvrayzhh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gzwxgiujb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/galvdhrhj.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gqrxwbexk.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gifhjnlct.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gmjrbegde.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gcphzklud.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/grtbouvuc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gscozjxgt.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gkmaoyccv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/ghuwocvqr.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gayqgwzhj.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gulywrmit.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gidhtlnsn.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gjsxhvaqu.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gjijkixox.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gueiusjdm.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/ghxjwwmdo.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gchssywgv.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/geuaxdiup.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gteywgbeq.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gzzeewqgv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gajgqkqmx.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gjsadlpcj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gnvgjpbjq.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gmmtlvnow.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpuenjqur.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gkwpjgcgl.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/grapjgped.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gldgtbhgg.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkblawda.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gancvkvmt.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gqhzgsqwd.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/ggitmcgxz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gxitmsswb.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gkempwycq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gvviqbvto.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/glnkjlwxe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gayokjnpm.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gvytvjynf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gtblsaaxy.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gzobhjmjm.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gtmrchlbv.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gjaoisgop.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gmsmfcevk.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gjhqqikav.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gknvarjfr.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gleozdcmq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gnnertsab.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gzscdxhwm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gnzbpcrbi.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gcfvgvoby.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gzwwzyghq.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/ggqaontsr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gdewystaf.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gpjcrwokx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gdhjhghan.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gccijjiox.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gulcqniem.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gyuuymcmp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ggdsfcsqe.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gldzaivlr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gdhoyttwc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gmsoyicxr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gywyziqzk.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gnnvdynjf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmvysxlml.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/guuupwbwe.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gehiufdsb.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gwxordtnf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gzicylzpm.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/grdbuehxl.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhndndd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gvzviegnj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gktmodrob.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/ggntznhwr.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/glvjgbkaf.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gflgdtdpf.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/grxncnlsj.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gazneylbx.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gtqmwvzxz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gvcvjafgs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gyyxekmdp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvomirocs.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gsysgsiqu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbwhpojpk.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gvapyhcco.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gopvbzbor.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gfrhocwcl.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gfnwfhsfx.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/ghlmcywew.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gstdvnlft.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/ggsqjirvf.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gsditojkk.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gauzlecoc.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gewfvgyij.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gdgkvytbm.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/glknzpcmf.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gentjwdka.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gdrauzxpq.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/giphqnrfk.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gciqvrtxk.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gzcoxakhe.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gttyhdgcd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gqctvphyp.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gugbdtvfr.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gyolvgolg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gnjjhagqu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/giiocoivz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gcffmngov.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gssufrqjd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gvcjjwqpr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gdxsjsjzt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gczxcfkyd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gdicowgei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/godgbfglh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gifasakrd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/guwuhttpq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gsrqtrpod.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gepinzkmn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gosvhugde.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gvcefjsua.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkxykouft.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gmmsfhliq.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gkytgswhv.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gkyifjlsk.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gsfjckpnh.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gelgkxoko.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gtyhzkvuk.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gcmnpfhdt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzcizqtji.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gnzauctot.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/giugjlcus.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gvvtmeset.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gadjdrjbw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gekbwqsng.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gguimwjsi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/goyzhcbos.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gcsppfkvq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghqamyvbs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gfvefarre.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gfigvpwra.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guegjpmnn.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gxwvnjuqt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gelthnyni.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gadeacqqi.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gssgwaokc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/glqapxkyt.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/guagtgnhu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gymoyxmiv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gkbahsvot.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gztojqgjt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/geqbtjywg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gofrenfmu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gtxnpsppp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gqjuilcez.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gsdwywgsf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/glekhyave.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gkrxgmrxa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gghijldor.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gkemfxmsi.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gygxesiel.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/goixfmbnf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gmaphtwny.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/grxpjulji.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gmapwelgh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gekfirijk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gzsgnmqqu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gpsnflkxe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gmklclulb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gcrxeklud.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gtsfnpkdv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gcbczrvzi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gmjzlrkdb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gdvbltyaf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gwfedeaat.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gyukbgqeq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gyyzpxvyi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ghxorvcsd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/goswjtjfa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/grzdtnhll.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/grhwvlqqr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gxrfiuyvf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gofnkjize.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gpeurzsgx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzdrwozhh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gymuffnvb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gurylewsu.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrsgpqh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gonuidkik.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfhovlbqx.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/ggawlhdzw.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/ghphturjk.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gzxrgzmes.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gnxltinki.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gjwfltfcq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/glfchxnec.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjwwlsl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gncnwhbln.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gvhclmcfv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gokavobae.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gltczjkmm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gtqmmrokn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gqfizjzky.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gupecdoom.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gxqmpsiys.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gqbdygtud.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gwhwalpbg.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gxhosneoq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gyawfutzj.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/grrjwdlxl.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gquyzcvnp.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gjiwhjcen.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gyvhcyoia.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gabaowysp.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gglkvoflq.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfuauoygs.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gkuakmrkj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gyveagihz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gcmuotxel.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gxfczhqde.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gnbmcyuqs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gkwgwibpm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gykulauix.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/glrescycl.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gfmnzqsyz.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gfkpmzfgu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gpjchyzzw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gtmluzjoi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gqxglnutf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghmiuokhg.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gevkwjrlv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grczgjjob.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwbvvgihv.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gmrxpzrol.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/guxrfnrme.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gawndzfrt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gculscpcb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gfgyukjcd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gnkqnwgzb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/guhxvgmmw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gcoxelqfp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gcfvpcyaf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gtwvlhvkc.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gmrpngors.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gtelribcs.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gnqzokdsh.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gffmwwhph.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gicwwisap.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gbjlptrah.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gzgyrmxrt.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gpzwnodnp.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/guxukhhtq.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/geuwdtjbx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gyxdqsjkq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/guyfiibjk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/goibudkcr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gthiwhmlx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gqaudmkoc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjavcirai.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gjfmgazbq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/glnvdytzk.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gnwjdbzpt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfmbcuiqv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gjoteddcx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gpeutiqqr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gzllhyahn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtvaxluca.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gbltnverv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gyshwsnjt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwvsmfuik.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gtjfuelbc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gnqtcsncq.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gpxxqthrn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gynmlefah.sHtML


<!-- 参考信息 -->