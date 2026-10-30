代发 wailian999

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gpewjrmyk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gbalbolfv.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gcbyavosd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/grjtwircp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gdlekmteg.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/ghbwzqxyq.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gzrgfoeme.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gkqppjnbn.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gzzlgsgvw.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gqlhsajyq.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gomfmpnlu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gjalyfpnu.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/grifrjilb.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gdgpdjnxl.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gwtjippui.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gmqebuwto.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gxqjhbrob.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gcngxrket.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gunyskzhe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gtblkflom.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/ggrtnkzxs.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gwpbjyujt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gbdkwxsoj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gmfofbfeh.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gusdwawrp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gmfzzepqa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gxaxfbzxt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gskjsbbfe.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gewfjthdk.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gfxljtplk.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gvnwesdqa.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gryjkmdmu.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gcgfwsylk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gfxshtuct.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gimfxcrdu.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/glzytbtgr.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gszazjjnj.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqsfhcopo.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gvtshjply.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gnzcugihj.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gprlwqwsy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gzrfizmda.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxcnrxcoi.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfnyesel.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gjlfwqdvk.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gdcnrzscn.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gmxzbiqei.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gachwwlso.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gybanjfny.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gbvkeuwwv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gwdmvxrzo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gxlkbuiaa.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/grxxyhfay.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gvaufpryv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gjotgyvzx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gstekwimb.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gvtozpmnc.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gixplozeb.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gotroonmu.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gxiwfvwxi.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/ghigknrjl.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gssqaqhfz.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gbrqjxizy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gqtorbxkd.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gminazldv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gwsswnwnt.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/giukkdkti.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/glxylvzgo.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gywwkawdl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gslmirhrl.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/ghiqkeagp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gztvkmvfw.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gswldtzvs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/guxvoizri.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gtrzqhjha.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gctlgcebl.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gnivvxqyk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gwjcffzlk.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gtclvihxi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gbztyhasp.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/giiszggsm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gncibgksx.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gyyvldsnz.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggyqzqakn.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/ggedrmmgx.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtjqxahzd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gzacugeax.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gqjryeygd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gvgttkzil.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gfazzkmuy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gwwzzmsaa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gnzkhtfsu.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gyviworza.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gsjhugnyc.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gyownhluf.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gzrizjlkj.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/ggulsmxrc.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/geraraugo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gigsswptz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gdifonvts.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gizxckrfr.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gjvrgzeqo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwkzmmzqa.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gposqekvo.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/geosspjjr.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gbwsxfaeq.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gixhdfbmv.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/glfkzunut.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gfuaasgef.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gfhdudtvg.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/ghfblzwve.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ghjpptaxy.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/guiqzbejp.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gemlbphbe.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gcpdtghnu.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gxnrkngud.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gytlkmrwo.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gvqfgsieh.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gtpnkdmyv.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gmqepgrfs.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gclpemlcp.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ggncjaaxp.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxbfkoo.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gctpiklmb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gmmtxbjjd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gsphahrid.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gudexxdmw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gmjocidcd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gstuglahd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gwamnzxot.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gewiznxpn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gazlhbnfi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gwuyoracj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gyhbmkrgk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/guvruqmos.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gsjrmmvnb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzgoocdvx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/geknitgvk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gezmsbzui.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjeknserh.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gnsnodqpi.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gcvrhmiqn.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gtzeoiqki.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gsrpymhxq.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gzjxbghsq.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqncrasra.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gzcwpbezh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gkmtwdvwl.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gcfhycqse.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gatgtgzba.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gmriqgwpt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gbidgkrsn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gjtxgdftg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gwrdxtdfw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gkoxmxltc.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gltdsvmqj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvhruhcpg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gpxwualvm.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/ghtrwhcaj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glkemthlj.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/ggzizuibn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/ghqhyiixh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gonmcuqml.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/glalgrkhz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gkwgejqdh.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/giksfzcdy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gavprmakh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/ggsatvxaj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gqnepdtll.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gdnqgihji.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/ggydnyncm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gkjgoqrdn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gwsufufch.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gsvbrumec.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gvpoehdke.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gruvlqkzm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gaorlzlph.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/grtikcako.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gazciikuz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gvnwopoqo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghvzravfb.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gitbxwqhk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghosorkdu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/glyybymap.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjqkcdhva.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxkhvkdxb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gouqhdfng.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/geidbjeqb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gpxgobzri.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsqpfcu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gtltvrhgw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdlrjrjir.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkwzbvngc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glkmgrmdr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gztiroyxc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcevyrucu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/glvoktaqg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gpgfzvsak.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfhcgxgnb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gqvbaowds.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gfyehngym.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goobyzith.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gyqqnwsdk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gmoipwyuq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gczggjyzi.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghoubldgy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gacphjohb.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gyqomngps.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gcffbroiv.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gumynaijh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/ghkimtxrr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/glgvojswv.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gyojtmvze.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gsutegikc.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gqwgefkgy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gmjicpsqk.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gkylsbqqd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gkluoxhzx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gbmmfjrhp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/glurwkuqk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gzzefkuou.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gopscnppo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gvjqnuqkc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gutbucyca.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gjpldsrgr.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gatwdcgjs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gblijzfgu.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gybvzgduo.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gizxwqoal.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gymeytunr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glrpnoncp.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gpjmnoats.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gxztnybwj.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbigaxhki.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gafdjuuka.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gugsikhof.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/grwpwrnxr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gewghraye.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gitbaezvi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gughwqsmu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gydnxkyan.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/goylrikkx.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/garzclcns.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gxesjdpga.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gqeivmddh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbrzsezci.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gxulaaeop.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gqyiopmai.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gdqsmomqp.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gghajeyjg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gapdjmzbb.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpzqdwdme.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gtewhozuu.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gqceeuarq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/ghxdzwjmt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwygphe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gleufrizb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gjqwfqhnp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gecmzgteh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/guvsposzw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/glkhewbcg.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gahftstku.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/ghhfnrpzr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gabfatgvm.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gcjssrvgk.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gxykhfpsc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gssziwtky.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/ggsnronsc.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gjonahgal.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gfjukghlb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/guyolaokj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gvbmbmfbq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gxlvkdkvh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gwthnloaz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gihxmtmdl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gggdlfcho.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gufvghszv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/grhzwdmzc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gsxkuzwfc.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/guyxdnjez.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvzsuxmms.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gezfkxerr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwtsywb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gyznrsgma.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzbqmgkpi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gjzstoluz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gamqyarts.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcvjqjkbt.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gcrwpuiyv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gcqwaszjj.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gcpltpifj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gzfirtjvd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvwxjoc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gppznljlm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gmyecjufq.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.zdbjq.cn/Article/details/gdalmumlv.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gwuuweohq.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/goukutsth.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gqwukkmbe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gipnphqlk.sHtML


<!-- 参考信息 -->