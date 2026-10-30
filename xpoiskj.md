代发 wailian999

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gztmfexmr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gfjgfsglj.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gjmslavei.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/ggqjvtmgn.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gnkulpnyy.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gimngarti.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gmemodbwi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gesmazhry.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gwkceeamb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gcmpyvhnd.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ggdjwjyji.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gjsbkevxk.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gxikqaysj.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gnksidlka.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/goyhmwhqf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/glqmrhysh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gthkmziqj.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gzkseurgd.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gkeyoookt.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gelfdrumu.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gwyomolmo.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gmlwmkylh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gnvdzchyc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/goxporhaz.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gxmhbuzkn.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/giquslhnm.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/geoozaxof.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/grgcfercx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gqnnpkyqj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gsywpmtug.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gnkvowuuj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gwtjidbyo.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/ggpixjvxp.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/glwnlpubt.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gbyezzhrr.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/guocsqwgq.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gojbpgvgs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gonpbrmme.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/ghiseiolo.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gunzlddop.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gxrbflfqc.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gmojwvkof.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/grmiwunab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gkgmjzhqu.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gbobyfeen.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gwtgrdzoe.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gvjsnvdah.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gekbpwkih.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gxgswofdn.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/glfdftmhl.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/govpplwku.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gvcokegif.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gqkiuxpsq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gnthlqmec.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gdfgssnbx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gepeshwsx.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/guxdsshre.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/glibangwf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsxppzlse.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gokbuburr.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gtzclqukw.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/glsnyoeph.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gawaqifbk.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gpjrjcuqq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gjkvheobe.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gffddbvjj.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gaxecdncx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gbiangesq.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gmqxxhzfa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gqzbtmbmp.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gafkcdnja.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gqongocxn.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/glxsbzzsr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gojfuodfy.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjrzdsrmt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gbuufyddp.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/grqojjqng.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/glijqmhhe.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gpznlafbo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gkryjdjtz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gutvswdvt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtdwohhx.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gfgoncaqq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gcduvddry.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gegqscycr.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gkqmgonxs.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/grchtdbdv.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gxnybeqlz.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gacvudnaa.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ggyfydkaw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gujdqmikn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gciefdwdp.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gvcfgqsnp.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gusynunoa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gffoqfghr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gxzbccuro.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gqxcxcsrm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gemvcqafw.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/garccrhsj.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gaplhmdcy.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gqyzbkjej.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/goeifgqvk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/glyiquolr.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gliivyqjd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geyqvfpsf.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/grzybjwmo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkrnonsyb.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gkzwambga.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gltxdxlus.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gxlxzygby.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gqmyhrczk.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gqqdofmmy.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/guenmtetc.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/glbnrxwyr.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gkbxwbbyb.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gtljttkxc.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/glpwygrld.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gtedhcbxi.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gqwgrdfjw.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/geposbytu.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gszyuihxp.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gfellvvyc.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gweshfmas.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gfurhtsjf.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gebpkhwzg.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxsdrudyn.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/giatpfrts.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gbnytrvhn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gbnmzysef.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/geljiotrj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/grpokgaek.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gkqrxbnyw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gaqumbzbg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gcbuuhkxu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/ggovxdzml.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gbocjbqxg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpdvzjdrf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gffxiyavh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gtkaxjqfl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxbsalzzo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gwapcdpfr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gggwgclrw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gabhkikyx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gofbpeoby.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gszfqecrs.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gyrztnbos.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gxrhuyutr.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/ghdnzzwcf.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gqxecafzg.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gkdmuvoin.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gbitfnxtm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvcjnwhnv.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gzzwhkkfq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grcbqqbuz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gounhmkqb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gqdnyguxo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/grasjjwjp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gguuqvjlb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gmdlsxvdr.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gzovtdjxt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkprkrmzw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/givnglgui.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gnwjvatus.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkxxuwvum.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gbqvozlqn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gsogfckck.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gizsqwlhu.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gyrxmhaye.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gmtlzknso.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gxdqwdvis.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gzqflijia.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gvkjmgocz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gqjrfjkkk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gjladdirq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gkbkdkvlc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gejjegzxa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gmnwmrppf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gauowbuwd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gayausmrc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/ghbmpzira.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/grgtyjenb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gharojfbv.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gmxswpsjp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gkjbbyiok.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gzkqfmenr.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gngezezda.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gcikdsjow.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gczqffamc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gksraboug.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gkpiqsokm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gopmvrfcy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gfefdtytj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/geuoybhxx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gfoijvyde.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gpwupubmb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqpcqwtmu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gapmdiujg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gexzryzkr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/guvpalfmk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gikqiuqou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gtlyxtdzm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/ggjovihpu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gtcoyhgia.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gwtqbupiz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gdjzbjzdw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/garabawlx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/guhfhjeqf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gxxpyifcp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtfbcwpvd.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gueslomiz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gayrntulm.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gjwmvzyuu.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gyvvxnnys.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gadinyluq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gfbrxzzht.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gafynpthc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gifhmzivx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/guvkgnkhc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/ggcwocqgj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gcvzwtjgl.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gypeghdom.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gqgarjppa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/ggldhagms.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvbrlkyxj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gmhpqrfpn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gncrmenvd.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/ghwcuwotw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gctfxrvqf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/glqkepttk.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gxolthpni.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gdflayyoj.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsxxxzzul.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grhmiomik.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwrnenhyp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdresdd.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gckqoikqe.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gficzfxib.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzxgrikbg.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gekdfvqhh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gadhodauz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gqvpxmpow.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gthmwligy.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gbyykaljp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gsccvqide.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gfsdectem.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gdiqiecqf.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gkqlywfvj.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gvvgrwgqz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gkyaarzgc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gbrjbyjoi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gtwxeyuov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gdithvmiw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gtdsqzidz.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ggjlkuara.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gpawhsuyd.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ghnbemxdb.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmubtetwx.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/ghhpbilop.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gpdqlsyir.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gqaczhtwc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gxwjoogcr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gaxislijx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/grmmlqefe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gerhgmscq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gpsnkggcp.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gohoxxwbc.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/giczddikz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gsvdnkmdd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/goviilxix.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gqiabuosm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhqfgwqj.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gpctfymul.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/geqngjzdu.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gevuwysvy.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gqsnsdtmc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gejwpqrah.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gaxdmszje.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/glstkvikv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gokepolcq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gjwsihvhw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gcnhgflsh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gzzxvkaqz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gjukqysrt.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gkhhigdjd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ghrjmkzsq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/ginpexijf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gfuqbqtbz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/goiyatjyw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjgpnwupy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/gwxqbsayi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gzpohavdc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gxpgicwlp.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gsuyjjoqz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/glcqhzwoq.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gbjfiwmty.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gndjexykq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gcmlazjeb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/goqvykckk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gtykbvedi.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gggjirnef.sHtML


<!-- 参考信息 -->