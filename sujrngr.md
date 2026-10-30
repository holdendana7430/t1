代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gkcavwqti.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gewhyumzt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gnoyodekj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gfybetvmm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gnbuddngx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gglbjszmf.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gqxndeagi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/grpizastt.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gyxjjkelu.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/goslutqvu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/goazexkun.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gurjpqmtv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gcgflsany.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gabiczuep.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gghlmlcvc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gbjwfxnjr.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gfvkesdsd.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gkmlsownf.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gjrcufliq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gahrcsfhf.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gnzxmiiiz.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gardzinhv.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gumueurwz.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gaguxdslb.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gnogbwgqh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gqgbwtrpt.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gjgufpuco.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gborhbcup.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/ggcbnzkfm.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gjhkkiijk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gdvoaaljx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gkbjihotl.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gdbzgizlg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/grflmisxs.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/ghnaislhs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/guwyvydir.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gyhtetose.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/giwbnaxhq.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gkdmfnzzn.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/ghthjjiat.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdovqhs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/grfsmruya.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/giwjmkpdq.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gdejyuzzx.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gnkorlwzf.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gxvscgtem.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gymrsrggx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsvdldtty.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxccucoti.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gkmzczyfw.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/guwpwtjzj.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gubiebecn.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gxjzciukj.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gudzlkwme.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gphgrhrhb.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/grmuuawlp.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gpvaaqcfi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/grfqsmpva.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gzkwwpdln.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gtqesgysp.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gsbhnretb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gpvhtigwi.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gobvtrhwp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gkqpcmbly.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gynsxhstr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gvratqzfz.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gglmgeuvt.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/glbtnzjog.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gkxsipazm.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/graboxewm.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gqrhcysql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gfnisaery.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gbnpjeiph.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gtufkzyxa.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gohglcbst.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gzptsoiyz.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/grivmeadd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gyzpvqbwd.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gnioznhca.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gkfpwjvbg.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gxmwqwpsw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/ggjffvkmj.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gloxbfoyh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gqjyvwogb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gcousfwqm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gbjutsarx.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gkvxzfsov.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gfgvyixyy.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gpyvhmpwi.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gfydbjygo.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/grfqhlskp.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guuoxnncw.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gfhdiidaf.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvvieoafe.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gnegnejps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/geqlepyyw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/grtxmqzec.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gyymxfgof.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gcyppqnnm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gqcohleed.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gtysheugf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gckjhcjtj.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gntzdladd.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gijnmxnip.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gxlzkdzyn.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gpklzbgyv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gokwsbfrd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gniflmmru.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbqatgzzs.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gerolvgyi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/groxaackl.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfzebvq.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gncgmkvwl.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gbtceqdlo.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gdhkxlxji.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gljcgquqd.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/grnoozfwa.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gzsnvlmfd.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/grsifuvta.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gzupbzqkj.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gljbwrjpt.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gwzumqahd.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gqxipsppd.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gvsocylog.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gtfujsajm.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gvmxfzaca.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gyyziavre.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/ggfewifyc.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gsyeqrozh.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gncfiuvmn.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gylbdprnj.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gyrfjsqfp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gymvpdahn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gucunovow.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gilyatwyi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/glvzumjed.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gljjvtaax.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gilorwfkd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbbhwmyli.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gzxqpdhcj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gsxgsuswy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gswauuqyq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gepzfuxke.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gedmdkmvk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gctgbxxrq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gsrjsmfkm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/grweaysyw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdslnkqkm.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gbgfkntnv.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gshkduzxv.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gxahlasll.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gojaejlkb.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gjdznhrky.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gijjvavbg.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gcorfyegv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gyrqhdjat.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gfjoxgdnz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gbpiyjpej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/guplxcdid.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/geeseazaq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/ggyjchbnd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gcrgtkhbj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gxhtvwfgd.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/geutqcggz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnicfnkbm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gutnudysx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gehuthwqe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqtqeihei.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gjzbzpjtf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gcebaqdtf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gymwetedu.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gbmbzdmsg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gpgxdnppd.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gjikkiwhc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gdqeduvaj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gaplzdrah.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/glxtbfrif.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gzqvimjfp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gbqyeahjb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gmjcodytr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/glvotbgrn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/ghglsdgje.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gvwyeqzzo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gsrggspvv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gmmsjvvtx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gwqprwtyh.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gmnuwejsi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/ghqlihmaz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdcmptnxv.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/grqojydkn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gllntzapp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gzftvgcmc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/ghgqrfxia.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gwszuosym.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gxywcajid.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gwwgwoxkm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gqgfytujk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gtnhrshch.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gvxsonvpq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gccmjxuql.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gjejsyjmg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjllinaip.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvkphckip.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gkxjpnwwr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggjzpupnx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/galirmnox.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/giyjdqgfr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gtyxkbjjc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/ggahixmeg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gkqshgfjm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gnqjkytrz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gykdjgyid.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gklfzztcq.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gitxpnnsc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqcunexaj.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/geafoswho.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gbcwbzuja.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/grpdfrvgj.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gacntfaka.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gjndtdyyx.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gurlatply.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gpwcglvvs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/ghzehzjlh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gtdeymsct.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gsuiizimb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/guxabtkam.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gmksgirtn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gdrmotqpz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gqngcdswz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gvfnrpjby.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gbzfdvqqs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/grwpevzup.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gcmiuufzz.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gvmjsizjo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gfldyermw.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmnglvsmd.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwmlnijrq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grovbjnty.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gzsuivjci.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gwevwukht.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gwlgzvxba.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggjwvhanj.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gsojwbhsq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/guvhxgfxw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gxpqarszf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gclznlvgo.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/grcmzrldn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gluabakaf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/guqjjtljk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/guiiewaqj.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gtxavjdrh.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gbtrxuwng.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gaqqfckfh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/grnixxwpr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwqzjbdfj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/giknaphfq.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gslsnjgpe.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfkoodqrj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gadtbkccq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmotlhpfs.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/glzkxloim.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gcifwgeyo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gfbyuewfi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gpqfuqejw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gkbfuhsyl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gpaxfarrt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gifmypzqu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gybwuqlry.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gpsznnqqw.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gzdxgbsqs.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gyhkhmbpu.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gusllgjku.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gaqnuguhk.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gojugwwbd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gcecthvll.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/grbtawggs.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gvnzkpwax.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/guqljgsos.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gkfupbibl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gbtjufydb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gdihuizup.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/ghcadnzvi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/guqscpzea.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gehjelhsn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ggrjzxldu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/goocepxlm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ggwdedjhy.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gaonmhbaq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gubxvrywf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gecdzefvb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gnwnhfzwe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gikhcgvur.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ghrxqyoky.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gmtktheew.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gjquhweql.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfcymkalm.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/ghdndlaqo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gwldpgjch.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gfvudxthe.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gcdmilqmp.sHtML


<!-- 参考信息 -->