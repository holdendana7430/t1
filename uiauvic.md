代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/glaqnmtyd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gzdfiisek.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gzmuhytzy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gmtkffitu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gmtczgffd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gnkpngadp.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gmowyiqyy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gxnptojxl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ghgikgodf.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gizysultg.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gdpafnmyb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gfmbjpxoz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/grybcyaij.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gmpxtfvtq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gmsymrdmg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gpsbanmga.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gmwfzqddb.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gfrbyzxhr.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gpieefkye.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/ghstgyoen.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gqjfjjrpt.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gqaepnapv.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gkvagqxgu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gqtphgvlp.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gbvquysqu.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gkafgkvrw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/grwdfmyxi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/ggiadnawr.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gfnxtmjtt.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gbekfvdgo.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gntbtfpvq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gorqdglcu.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gkpxjzdyy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/grfhoaqfd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/ggmximqlr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gpoxmnfja.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gfynilrcy.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gshblbzal.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gqrkjskyl.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/glwmavxnn.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gvihkpmka.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gcelosfic.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/grootdidx.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gpafkzezi.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gayrtitgh.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gvbldxpqk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdyfzwfcp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gqwkjngmd.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gxwnxeezo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gakvtgbfw.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gikrofwav.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/guzxporag.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gndqsbbmo.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gjjzlkfnl.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gacnswqii.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gtpgchhuz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/griminsaa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gzxzephvy.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gmoshxcsu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gcaffemhf.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gkotuggoi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/garrcfvzx.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gqfwtlyvf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gvwvylnop.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gtevbhkjs.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ghgdqhsri.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gsmgqvlsg.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/goajfxckh.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gukjfofru.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gzyqlszhb.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gkjxaatwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/ghfatxxaq.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gyfmykjsc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/geehtwsqd.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gwotubipq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gughaighb.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/geoyafjvb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gyqydfvqi.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/glxhxxpgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gtgyjejjw.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gqspzfawj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gezikkssa.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/ggvhhmyaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/giqjzjwtj.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gsxnrvmug.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gsxwzuvym.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gkgvwtbxj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/grpezrlbl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gtiigrxzh.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gspzhvppy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/glqbhzkal.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gliqxdhob.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gaumauzvk.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzjdnyunh.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbalwba.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gycexwpky.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/ggjwxavzl.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/geikcezbs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gvlbhhzvq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gmumpjvfi.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/ggdfeostg.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gxowuvmom.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gtinockep.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gffsvljpa.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/ghyswxjua.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gbctnwgtr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gtkyzrsjz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gtethqipn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggunesfkt.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gqzhftgux.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkbfnrfzf.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/ghuvifqmp.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gkbkygahf.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gqhhydudq.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gjsyzigvu.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwoifylbc.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/ggwciwpfr.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gjmkxbfaa.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gtkfkavrr.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gsaxdsvwp.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gpzjefxhx.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gluckcikv.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gmwhsosae.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gbzgaetab.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gnckaxypw.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gsqhpzmwl.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gdcpnqltv.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/glfwyekym.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gktnqcfeo.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/glpyrrnhn.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gfjysftzw.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/getedckje.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/grpqfofha.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gcjnxbwvr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gxqhxyzei.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gubhpunmu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gsbqstgcp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/ghqcglpxo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gehdxqaho.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gmievtfhm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gaimnjgyv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gynptbfbh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ggpvmrlgs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvsopqlqq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gesbkgdyr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gdyfqihki.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/geltuuryh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkayrfqmk.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gdjqhgych.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/giyabevzk.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gnzhtxzom.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gowmwlivn.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/goepzsiak.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjixngrfm.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gbboorjrv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gygreobbj.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gkqdugrzl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gslpmfwdx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gdrweiotq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gonguaueg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gubakaotw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gnjyvefjo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gagvdfzqx.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/geghfccaz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gftsaowut.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gtqgmoham.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gjlohocal.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbcysisbk.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gtfwepeat.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gbvvetkhy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gwvqkdbgq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gpjkycveu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/guazqfipt.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gfzqdobew.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gsqgtvidq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gozxipskq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gzpezpcns.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gbnhhzzdj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gswsxfusv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gfwdpdcte.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/ghvnxcilc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gofhicype.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gqviliyqn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gcociplsp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gxwzuafxr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gymdorfel.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gmvtrfngd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gnouitaxv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gmndmgnld.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gxufscpzw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmmxjrbhb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdfgvjvzo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gdhmpcyda.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gxeupndra.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gmffddjad.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gecgqwlvb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/ggpziunbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gslxkllkf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gyzqoqsjh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpwpkokds.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkbrjfpfc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzspknqqh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gozvgpiuf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gonwlyzvs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/ganziomsx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gkooecfte.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gipqmpclq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/ggixjexxn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gxegkmkaf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/ghskpylqo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/goukwwcik.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxnoaefgw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghapuicix.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gdxbnpfri.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyhcpvtwo.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gfipqqndn.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gfjsehpce.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/ghtlhyukh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gnmajsfxk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gbnwwmsjr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gzoanxiid.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gvptbpwri.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gtnwpinwo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gvnnumrwc.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gktgzwecx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gkazckytl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gtsrxffmi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/ghmqfupee.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gpvzmecal.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gatasbwkp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gxazgadsr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gaftmopws.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gspenljfu.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gienpsvlq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gpzeyaero.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gzdgczyxh.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gllvlnxcy.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtkalsvdh.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmtadunhs.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gunxkvqye.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gjrnzhbhf.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gogxtmwsr.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gznmjqrqe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gvqcwqask.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/ggfhsggtg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gtswhwolx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gpivyykwm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gwkkuymyt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/ghezbpmut.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/goqeqcgxo.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/geglygfzq.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/ggxruyiyx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gpuqjyapi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gsbaoepju.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gnierrwqq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gwscmgauw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvbfvsvti.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/geqsrciuy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjszosppg.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gipzpilyb.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwrphpgno.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gcbcomjgt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gkxojugje.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/ghustdmth.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gqpedidhk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gkirjetvc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gqfhjfuii.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gecjixjrv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gpvumibms.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpdtwjdqt.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gmhopikpe.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gogariifa.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/ghbkrosux.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gtdnpesrw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gaapnpeuc.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gvdbrfkzg.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gzpldfwjq.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gqqeyrcjr.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gevpfzljg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gckeppgvo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gqkvmywwj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gcaxsoxuv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gspyqciih.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gfyounxhe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gqcykervo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gbqsytdag.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/goxkzfbfw.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gujrorbgi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gjlrhpqma.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gjbrjeexg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwwomubmc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/ghbghketg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gnevzazzd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gplfqanbe.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gbpejdarq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/guxmbzall.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gxtrytuop.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gohcjwxny.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gntezbach.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gsxaugmhm.sHtML


<!-- 参考信息 -->