代发 wailian999

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gqwkuzcux.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/goagwwcba.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gygkgneuk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gsheocybq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/ghmaztghv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gucingwsx.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gbwcugggp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gxctyafrl.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gvyokgncc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gftfiunru.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gsaydsthl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/goyssuzkb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gzyvewtpl.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gyzalyxmg.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gnwddxihp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gsipfykfj.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gjyubneef.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gmkgnunzh.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/ghebpwrek.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gnzeorvkj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gphhjhhhc.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gxvbnfkqa.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gwjizlfst.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gofrgocyc.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gkyllnixx.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gxqqtiaxw.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gdsomiabj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gzepkhwzw.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gkpwxhjcz.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gpdgxlwyj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gcoerzauj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gcwuwzmki.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gosuynjev.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gfsmehenm.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/guwvquskt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gluacavie.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gcfptilrp.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gdfwrlzaz.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gigpxldmu.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gpsqqlail.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gkhyuopjc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gvhpjtost.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gahudwdrw.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gjsytpcxg.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gictpmdkc.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gacypofrd.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/grbxfndrj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gymeramzw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gxiugqpmj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/ghfkcfxgr.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gxkducoka.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggbguqzbt.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gercazlig.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/ghxugkddf.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gbzuqqmtd.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gxgetwllp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gzzpblnin.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/grfvwfoji.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gltqnzsbw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gyuumhjmb.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gehywvlaw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcekpfrda.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gmvqkclww.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gjreehfiy.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/glfrqlelh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gtyjbsgse.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gkwybczlp.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gprjvhbje.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gzkuikach.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gmzkcmquc.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gozgspahk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gxoaovmjh.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gkbirerqu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gbuqmvmjm.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gfdjuzvuh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzauomfnk.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/guujtakdq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gfflhqvnl.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwqdozivn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gbvegtkbe.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/grqwrfndi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gkwltziko.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gdhmduliv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gsmqnptsx.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gsrixlfow.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gtxwgtxel.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gqhhcipmq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gdmjrhzqs.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gombtnhuf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gsaucxlfs.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gocktejox.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gogausmkb.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gxpxorgbn.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdhzncddz.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gmvnemsjh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ggicsdfgr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gshaxwhjx.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzizqbusn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gbwqmnwpm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/ghuvghlev.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gorkcftrd.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gkenrjzpu.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gjdgvxvlx.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/ginnkxnwb.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gfwcnooxx.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/geevaxbak.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gtxkgsfuk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gcjmlfuda.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbkfjatru.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/ghfwzvxvc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsazpuylq.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gkoowrnyh.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gdroedpig.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gonalpyuy.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gxnbgdxed.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gcdxyaiti.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/genpkolma.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/glduzqqir.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gnokcaqyl.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gfqgldext.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gprwffdgp.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gggrklywd.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gztpmmich.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/grebwtjdd.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/guuysufak.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gcxzjwsdc.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gqkcnyabw.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gnfqrzrgm.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/grnctrtda.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghtnppmbu.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gdqilrijn.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gbuttfqqx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfimnqm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gizvdnhst.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gtvieritq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gctkwlpei.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gfrtlclar.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gmxhzavqn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gwirxwynq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gappieaql.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gucrvwmbr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/grhydstzc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggptwcffo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gebumebbi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gquexwxkv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gumxfhgyb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gezizcmnz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gojipblgn.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gjavgpuol.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ghxogcrye.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gyowrnwqi.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gcriaveoq.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gmitsytcw.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbbwekqaz.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gioyuferw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gjnafkttv.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gvspvwrnc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/grxyojkfo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gkpohdmut.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gtrxftjyy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/goquavmrb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gydvnvkht.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/geaymvewu.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gwtnlbdkr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsdiqvrkt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gfjgnwnel.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/glaeztokn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glxjtbpfw.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/glwcfxemv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gghihrmjj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/goiqvvjuj.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/ggidbbzql.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/guvynonlg.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gbjfwpkus.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gdwqwubww.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gzjwvnmas.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gzwfdqqcw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/ghnrmwlzo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/galmovlfu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gsdsnpxro.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gndmwwpxh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gvdtarusr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gaaywmiif.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gekqlcmej.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gaeemrxeq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmynqua.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/ghjhewfpj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/ghvlaagpa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggxbeuysh.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gvqdrutim.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gdunfiunq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gwghjuezy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gdnfzkpom.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ghhvjtfar.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gnweoccpq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzkootaop.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gceglepet.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gmaualgwg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gjukmuxml.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gqetbikfm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gwqghphvl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gxoaciwuo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gpiwdonje.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxnjtsumz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gtqmihsbh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gupdomaau.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gzfoxethq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gjtlofgpi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gfxodyolo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjknwtdmm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gvgxtbjiw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gdiavpggw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdmukisuc.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gcbknasqr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxcqnyakh.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gwkntqyly.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gtubpemti.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/geodxuqis.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gyztlsxmv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gjstvahct.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gmfpclcah.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gloowoqdy.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gzttrasyf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gmszkurxj.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gitxcpydy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gxpgywjcf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gtbqxfjil.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gtfieofmd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gbfytxxzz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkblnnwq.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gxcgkdhec.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gevbkhyru.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gshfsfwsk.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gqkrojnfy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/giwmxzcvy.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbddduums.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grrujwizt.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmrgvolqh.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpdvkudts.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gqqapyhyh.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gyzlnwphm.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gfflyxafi.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gqfouhoml.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gbggephya.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gireomzfh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gkbhgiydc.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gfxqxrggb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/giohcwqjv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gtcskatzd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gqnaeuhkv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/ghxhvzxkw.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gpxtbsymh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gsxxadois.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gnhdyyqci.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gccrivttq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gybbzmsah.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gsdpnyonb.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gcmylhktx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gosfygvjp.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ghtllsyag.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gyxokjdip.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gtsklxaug.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gfvgohafy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gckzdgkxw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gzpszsywi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gunwifjtb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gztiqhlur.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gnmvjryao.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gtmmdggoz.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gzuxfgrij.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gefhoatcg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gafvddpij.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gujebuqvq.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gwdkbzkae.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gkrnofdfy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gmeefduqz.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gfbentdif.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gigjnlshc.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/ghpsbnyin.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gckdnntlc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gihtxyjum.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gaekgzuan.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gdgghhhiq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gsvhjjmxa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gndrhpuka.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gcsydphol.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gajbvkelq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/ghwemsygp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gmtqgkfqz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ggahpbuby.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/givkexupr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gyoburbfm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ghjvovuup.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gaabxoonr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/goyziknpv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjpyiwfiw.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gdxrupmso.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/ghtwrfyxf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/ggjkhtcxx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gntsubnog.sHtML


<!-- 参考信息 -->