代发 wailian999

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gbiurwlzm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gnnhdbxmy.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gmynhtfdu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gghxgpfaz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gjglqulvd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gtiddzrtw.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gepntfuat.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gkvboufgm.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/ggdpshzub.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gzenagsto.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gdhfpmpon.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gzkieqfzs.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gkirmdqcn.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gjxzlznhn.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gootqrthx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gjlwzdorl.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gmvpdpqvp.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gncobdyaz.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gutdtsamq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gzamalmas.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gqepoeypc.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gtvixcoxz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gmydbximg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/giitdhueo.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/geeicqiph.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/guwwrokan.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gzhctlbbf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gayhlxwol.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gdpcgeept.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/grqeozapz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gwotflgjj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gjwgvqpcu.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gciklhjle.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gppmcsick.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/goyoybjih.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/grctocyhk.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/geqxlzrkw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/giauaqmmi.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gzxxuvfuu.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gxayqhzrc.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/grvkekypo.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gavzhbauv.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gjgxrvmuj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gumdweyiu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmryizogu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gsmjzjkcx.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gcrdjoplr.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwebruxnm.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gmlhxeuew.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/ggxkvhuzh.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gfmkccbrh.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gxlibkuod.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gdfwamlug.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gnoidhxcq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gzcljnosu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghrlgmein.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjjygxjxi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gzsftrwfc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/ggelgekzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gylqifppl.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gkqyjbhvw.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/ghheicjko.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gprlgsvsb.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gaxjrrded.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gzoomdxiz.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gbuxwubdj.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gkhsifufj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/glycofqhw.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gkgzpilnh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gapoanheb.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gpqoujege.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfidyrajy.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gduvmeldu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gobogkdkl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwothrsqs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwzikgphk.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/glvszugdb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/goekejwaz.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gedlfiveg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gcrajxaxv.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gfsmwmsuz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/guaajhzrn.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gifwrkjsa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gkhixahwa.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/ghxztrmaq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gbtooxspn.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gexexiozd.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gqwsryvzf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gvrbylvfm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyodnuqsv.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gvemzqjgp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gktdosdpu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvkhmdpsz.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/geuatahol.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gkvtafyxp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gbeggcafm.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gntbgccrb.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/graqapijb.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/ghstbomto.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gktorgsdk.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/grxigiutt.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gmmlmabfa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gvzpkwxvp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gduqzvvxa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxalopbsp.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/grssjtvll.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmjwtuqlj.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gpmofnpbx.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gdulcnmmk.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gomxhmvir.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gjqxnoqmr.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkhvjsjcy.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gilcajvlr.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/govizcyzz.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/goddayhlz.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gsciufxpd.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/guynebstb.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gkzayinnw.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gsftkmwjp.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gbrgckqtz.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gfzbvsucj.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gavcdlpda.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gbdxwayef.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gzbbwdfbm.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gewxfyqwu.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbzpriyiu.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gmxiwzdff.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gywhebxub.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gpdbcjrkb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvugcfvyk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gnagfzyik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gwievytqr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gbqkzqzgw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gawknmpah.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvicafvtl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gfusjckih.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/glfkspafo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gggwplgzs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvwqarp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/ghlajemnr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/givkvuvyl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gzkdqrztm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gidscsche.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gnpuutiiq.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gvjradbgu.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gptpatend.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gmiyhohxc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/grxyulkiu.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gnutkyqii.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/giiboemgt.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/ggvuurnsp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ggotdxvxr.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gkdnkdwlo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbfyzkrpv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gwrzqhhgc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gafyykivt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/giyjiwotr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gvswoucnu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/ghblvboxp.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/guzrndgjw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfoxeupid.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gvozuughw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gimabkolt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmqhsdlrb.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gixvuisvl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gyhhveqph.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/glfzfmcao.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gwuauuale.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gdghybpyp.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gxaphthgh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gnqurrliq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/grdauaneh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gqjjswsws.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gacbbuykl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gsjonbrhs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gssjffdsb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gosdxlknp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gfhvsdvua.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gvckmdwfl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gitpccmnz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gidolywut.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/ggtbcmfpr.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gogttvhur.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gpflsjuyf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gquqrmbfj.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gzwasezyu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gahgvelbg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/guqnzfigl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gaossyenu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gohemeddk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gnpwlyxpc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/ghsqmomli.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/giqqkzgir.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gpjgbfrux.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjodkrfie.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/guqsdmkvv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gaqvwnvdp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmxokeaol.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gijrteawm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gswzhcytl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gypdfkbrv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gxqfyrmre.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjhujckpz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gzhznpylf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/goxmsaorf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/glolfipdr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gdifaqgye.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gsvkciapm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkqoognoc.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gczsvusiu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goyyhefyg.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtsyaotyy.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gisszbnqe.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gpztjtznr.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gptiqcxbm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/glvfgebgs.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gbaslictb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gcnwmyfyg.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gbsrqphwh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gmtiqcysj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gucgtwloi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gcxkrwelu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gcmckactl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gqweorsoi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhkjmkn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gdwaesnfu.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gfwrmjayi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gsigpzxcy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ghqaqhack.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gxcjzzvte.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gvezhvkse.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpwlmpfcr.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/giaxfchfm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggxkfxieu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyufxanrx.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gdhfswynf.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gifmpqeyf.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gitdlitub.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gnbgzlrbv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gaepfrhru.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gpbgzqhuy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ghavnqvqc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/ghagcvvxy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gsyqfqeyc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gopnzdend.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gfgmedmyl.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gsbwwhauf.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gimhlugfn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/grixvnjfd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grnciuhce.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gjvkgdbiq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/guiuouyqa.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grpigthcg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gspuxwrwy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gneryhnol.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjqouyxbg.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmmcadvmd.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gcpbltpnv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gzwhtlyja.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gxnzhtpyv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gopgzxbvn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gjkfqbknp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/goyejbgia.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gezejsway.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gnsxramsq.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gbfoolfhq.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gwuailvrg.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/grcckfbfy.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gercflzhd.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gsxyoqnxp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/grrrgfvqn.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/geuotsdla.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gklrkzewe.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gbezttfxf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gnhhshjxe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gunkdcmtp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gldhruzsp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gymzwiqcn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gnesofhuo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gegfwrmhd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gshufeoke.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/guanbavqw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gfrbqmuli.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gahxvglkm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/ggyvotmby.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gybbwhwqb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gwfhgjoiu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/goaffmvle.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwguhkfi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gijzzqnbo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gajnspwue.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gtfwlagrh.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gswzyrmwz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gwoummuxr.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/ghnxrxkgj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/glxruzajs.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gseydmmud.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gqjyzqxbu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/grywkwccy.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gfcsanosn.sHtML


<!-- 参考信息 -->