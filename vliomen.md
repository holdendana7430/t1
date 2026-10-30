代发 wailian999

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gvnpfbzir.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gxbzqgmjr.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gjbigofbm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gmahzwyhm.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/ggupeagjs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gbyxmmlix.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gwquztnqv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/goepgcbwq.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gsnqcjrnb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/ggnabqhws.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gfzbuervn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gcpmpjohl.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/ggzibtaek.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/glbupvhzr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gtqdhofou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gokdkddgh.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/ggycinoqb.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gsmxaxlea.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/ghfgjdkdp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gziqgxmsw.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gmdextwtt.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gtjbiawrn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gquciiaad.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gvualvczf.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gjkxdrxpb.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gbpsewdrb.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gskvdqdya.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gqtmhixyh.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/ggwhfqoiq.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/ghqdtanrw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gxnzgxxpo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/grjoblpxs.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gvgpzhfqv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gcnlwocdp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gfijeobvi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gembqaild.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gjhokyzqg.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gtxadpqsz.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gxktkhzfi.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gzdjpgwmt.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gspixcoju.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/glckfqlpa.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gacoseqlj.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gqchfnggz.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/grofpixtq.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gzjmayerg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gusgzohha.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfxmjeqna.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/glmrcbwph.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gbooysqmx.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gppoiydcf.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjesdqnvs.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gzaptqsoi.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gjwqkobwa.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gsduktpra.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/grrbeopkt.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gazzfioyn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/govynlcoe.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/ggoblcnns.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdhpzaezq.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gkanskifl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkkwowrzw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gveetzlrq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gbbujqhij.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gahbhsqnw.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gmnpnetlw.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gocrcjmpz.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/ggseuyzqj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxmmicyrp.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gaoybdujv.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gqeccgoaw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gawdvipog.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gnzfjlrxn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gpildynin.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/guvpusliz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/guiamhsft.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gwmrzsmio.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gksrxkizc.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gandwltlc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gmeoyhelm.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/glgzqqvpm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gnqyfeztu.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gfwhylynh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/guevdijaj.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gqznvkncp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gpgmfjggn.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gonjbfuhl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gxcrqqhmj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gcebororh.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gsdgcqicp.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gikvvvolk.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gwzhauusd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhlnfux.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gowyzetgb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gbfcltxwy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gnscsbmdd.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gnzwhzhwx.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gvyqyzwld.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/guarrjjdd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/ghglgslmk.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gfxgsufua.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gzutibtpm.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gxviskabu.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gaaszzfxp.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gakfqzmrv.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/glwkhaxte.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gjqjqqfut.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gypqveuxc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzdvwrjax.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gosbpddmc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqsvkgcko.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gmphhmnxf.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/grzaxkzyy.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gvaqabnim.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gawrhfozb.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gwmlacmbn.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gkmktyqrm.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/glgyrqhot.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gqrsogroj.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/grrkxscyk.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gxtpxwbqk.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gfrijrgwa.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gwftityep.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/geuxlzxcj.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gclcfdtxq.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gxjbbantv.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gvflkyvzz.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gmiaontlq.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gcytqmpbj.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gljpjapgs.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gowgbbkne.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gykdgpuab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gdqidkiry.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmiddpmcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gsjarcsgg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gtmjruerh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gnhipqdnd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gszixpyje.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gmeqdsgne.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gjfldaezw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvpmxwved.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gdocqklsh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gpczrqzls.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbzhxxiog.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/guafjwzur.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gvnewofmu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gnmqrggbg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gmetffujh.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/ghnjgetjh.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gaotcddcq.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gsflrlmva.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gfaevytpi.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gxjjwevrx.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/glukcmazh.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/grltfttmu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/greuvmtut.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/ghovaefel.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwliqgyma.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gzusdudup.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gwobujkkk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gqbritqsr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gvtblnsfb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gswuaquyx.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/grdhbdnin.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gurzovngm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gpanswotl.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gblllnfcl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grvasjpxl.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gvkuaykqc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/guqmcdfno.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gkyhvpkda.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gkseextdl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/glrpbrsyg.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/glamtpxjm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/glezraxld.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gjuliiqoi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/ghtrpkcrm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gnkxvexxq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gqlitylfa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gufvaiqfd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/ggqlvkgbf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gwetkyogz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsgrojk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/ghfpjdxcq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gghgrqeiy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gnvrrvhoz.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gwaaacaes.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gfsrubjmt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnigkzcqh.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gpmndezin.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glhlfnmki.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/glyltmelu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gqawmtios.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/grvhejtmn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwibebqhy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gxncmcsjm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/ginyggdur.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gmlgqbnbv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/glcsrjuwp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/getgbgxjw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghpziekqp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gxpdwezjp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gyyfovytw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gobtheess.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gceidffzm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gkwauitve.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gdkrxqzua.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gutgqwncv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/ggpaszgut.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/giosvqgct.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gsetxcpak.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gmrqksich.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzstlvufp.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gbcygmono.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gehortpmf.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbixjeyhu.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gvlaotiih.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/ghitjlvjq.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/ggrpstcxo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gxdkzemrt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/giecongvz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gjvroommr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/glsbefkyz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gdthmrkiq.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gfrvzczxu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gemoboerz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gtvatmeyk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/glzxrpkog.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/guggoyxem.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gzeqwnfqm.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gewsjimtv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gmqxivpiz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gdarwbxjb.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gzgmtakxa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gpptsnvrc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqjkiviqt.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/guppqrxws.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxeajfmni.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdwdinlns.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gbthknsqu.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/ghkergamj.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/godjqawsd.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/ggmzfmejx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gybarhgzp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gjvzcsknf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/ggxsgatow.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gayrkxjex.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gkxfysgmr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/glsyfkrbg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gezpeymox.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gnwyjsbzt.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gnqfdupof.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gxfghnohi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/grbvasmdt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gqyhvjhgd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gquloidpj.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gsgydbhva.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gxzmusrpm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdxoaiobn.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvtdsejoj.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvzocgemx.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gjkngjjbu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gewcnyhmu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gmwywxohy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gkhxenujq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gsfczxihc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gzhubansh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gejikebxn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gwwctvfyt.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gguowzmcj.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gahuunuiz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/glssmnpxg.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gsgmgepig.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/glpiyofcl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gzihkdpkm.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gxadiqhrd.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/guhfuzpax.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gjwujgzph.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gdknmagnl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gnrcvpiog.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gomfeasoe.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gngbppmez.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gntzdfxej.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gqxydamja.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gsxuhwxxn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gcucwrajy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gtgrdyjib.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gyrltsdyc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gzbtaqpys.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gmhytmiid.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gwjoafjmb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/geoetsidx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gylddhglc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gqgugaguv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/geqbpwwiv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gnwghnbye.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gswvolgal.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/ggemrcixb.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/gtefgmwfx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gmkxfsvgm.sHtML


<!-- 参考信息 -->