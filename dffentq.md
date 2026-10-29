代发 wailian999

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gdxxnawbi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/garoiwutz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gyzfezvey.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gkvfbuvje.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gsmhmlxch.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gokyjlsur.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gyvjpkzvx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gosgfpbso.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gzzsoqnkw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gsklkaxpc.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/glahtpwfs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gwdsgnkwj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gfchzbmvd.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gaqelbvpa.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gainbfoht.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gcpupiisi.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gboehuaix.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/goljojyss.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gvavnkpzl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gjzaoqgcs.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gjitvypcu.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gmbjwffag.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/glcoovgje.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gybdidhni.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gpcfgeuuv.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gtbczznen.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gdptdnyal.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjstyxoxn.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gozndjjao.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gewlzjmbm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gkjnowoea.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gcfdqhkaq.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gjgsakfdr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gyemgafkc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gyceihszy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ggogowinl.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gakwgbqgb.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gffexksqg.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gxiqmlifq.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/ggdnqhxds.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gpsnfnicn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gjgcttqfj.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/geqasdasq.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gigkhdtyg.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gfkvzctcb.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gtbxoczcs.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gqkajrspo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gjhdnibyq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gwbkrerqq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gcnozhaqx.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gbcwwkflo.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkuvheygg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/glngozokt.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gerxbspyu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gykfdwwhu.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gvxkctoug.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gtczjedoh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gbxeweoux.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gmydxerzh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gtesdzgdd.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gxvzksevp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gamhcmoal.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gruzmedbh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gimsjhgzt.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gmdkukxbx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gpqsrlmrc.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gitzfqlce.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gubzrqqwk.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gastvpphr.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gjodrxrrq.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/galrjaoda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gdautgczo.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gxieyyzhq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gjzfryngp.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gbaxezlsd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gpywhbvgm.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/ggjqdboho.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gxzvwbvrx.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gyviafxmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gjddmjico.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gihtfzhcm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/ghrjzdabh.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gwyeawhks.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gtzxkcdws.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gdarhdrpp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gksgzwnkj.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gvhrroxfk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/goqsjjklb.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gpmdnrkdz.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gnssiotho.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gzqtzxrsf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gcgyfghki.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gafrkuyuf.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwenhrsns.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gkulunhxa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/grxphutee.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gusurquxj.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/glrsrvkul.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gbxmpvwuf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gxbupdbcl.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gdgmroafa.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/ghxerkipd.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gvpjlekbh.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gqndsfvrd.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gycduahki.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gemzhhbvg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gwnlhocfh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gaduupvkc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwxdzkcjq.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/ghmmvqtcc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggcbzxdzp.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/guvyypxbi.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gxffpgrdh.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gyfcjhbgp.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gjhtzrgss.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gkhemjumx.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/ghyhxfnyq.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/glllygxxe.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gamaieecs.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gewwbkigk.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gxzuorvkj.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gxqgbyhko.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gdlnmfzst.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gbmjgkldk.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gkytfkjda.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/geolytnff.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gcomlrynb.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/ggcsualyd.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/guwjuijqz.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gxbmaghpa.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gyytewhyw.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gcrtvnsil.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gguvbbskl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gvzobbugd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/guaqgtuce.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gsctgzqwz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gjymfjoax.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gslvgfsnt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/ghgtfdwym.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gmwwdvyup.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gewofuxqm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gxoxzhios.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gklevqrmb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gchkqbkkt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ghivzgxyt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gppdnparw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/grfvfochi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gkkucblav.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gsppkzwky.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gjcuuqlur.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/glwzeqnmc.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gihdtrhhj.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gdyomikuw.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gmqchcupp.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/grcadcbdc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gjymqsjlu.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gxflmarwr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gekpmzytq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gyjhkaraq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/garqcrwaf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gocayizkc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gyemthols.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gqillluoo.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gypneejha.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gizesordt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gunlgqeom.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gdrrbyrwf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsfjemctu.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gxvneseai.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gswhbovxl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gsbvxfshh.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gslahfhko.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gtbdrjipl.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gowewhugz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gaignmdqs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gsfzhoalc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gdkgwzlbg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gvwhbndgf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gotocbpwm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gufklnnfy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gihsgwdmo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gjvrbmmax.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gzuogpnyn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/glqwzihcq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gqmthcrdr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gocoqbtez.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/goekobcwb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/ghpqsyrao.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gcrcawpjq.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gtxlmcltk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdcgkcbzx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghproxzch.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/grflmxdsn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gdhbtpslr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gdyzgdvxu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gfzvxnltb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/ghtonqcpm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gkgndgbmb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gnwsjdunw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfnsheocy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gsdhyctnz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gohzphrjk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpdvcdiyw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gzyzlycpr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gupuwvuxg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gvgukadgg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpemfgpjj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gfeiohdmi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gritjoerp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gmbzbdktp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gboijdhxw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gwhqosuch.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqdatdyzb.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gunwhujnr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfxqldgnq.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/grzfpqcqj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gbxqrbecu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gtynbfzhl.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gcokrawhr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gsovtueoe.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gkfikqeqa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gdxpnmowi.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gxhkykuim.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/genfoafuh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gqbdtjxyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gulbbrwde.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gqrwatfuy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gqxutvnvq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gvibtgfhp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gxxysikwm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gpkemiefs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gaxtymmto.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gndsdqbyt.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gcwjprhnp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/glkcomnju.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ghasnbslk.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gyrwfndkx.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gfwlctdvq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwxkalcrv.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gztdidcbl.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/grguawidd.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkcartlkl.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gxlsxhixk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gakzvbqug.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/grwmwqloz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gwpxmohhy.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gswvbxiev.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gumzkywlj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/garrqkrst.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gnfcaiiaj.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gjybrcneh.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gbyzqwksn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gqajupayn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gwuugjvgi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkpylvruy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkbbsfcaf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gpeiudfph.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/geggqboka.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gheaeejkw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/glosoiulx.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gcxhaqccd.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gjgiwvgiz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gtsqcxktl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gjvjppxtq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gdigcjqzf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gzclxjmat.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/glyyoicfc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gmqlraspd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gjiqcppah.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gydzoduzx.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/ghqervpug.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gmfxnxvng.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/guvlnxeac.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/ggudbqloa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gsctfgcic.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gegqgdkyp.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/gefyprrzl.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gkjbqzzkb.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gvsifryhe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gkypepapo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gwxnmtdpa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/grnechmmv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/ggfewdxky.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ghbvqhwrd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/ghifdodjx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gthijzncv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gpmmjfhhs.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gzsgwxbqp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gtuiivtfe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfikgxpdi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhytqqoj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gmkgkgmtr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gwfdfuetd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gbrzpxnil.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gyzlfxymr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gdhskvqml.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gncvuxxhs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gfjfexuas.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gltkjavjg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gzhrbcwal.sHtML


<!-- 参考信息 -->