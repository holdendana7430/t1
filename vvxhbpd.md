代发 wailian999

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ghkplhtbj.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/ginodvhdt.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gazupvjzz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/ggdxhwezu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gzlqsvosx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gtfeovzyn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggcfoqlsl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gebrarbmg.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggoakxzpy.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/glmkqinsa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gcbrglpfr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gfkozonpk.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gushwxdnv.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gcievlvag.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gksmsgqus.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/guhkvoeye.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gbythfukq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gmggxlgbv.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gnvieafhu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gfvygpjak.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gganiqdlz.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gdcwfuemy.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/grfvcrpad.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gvkagxcpq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gbenqhyhh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/glhmaggpy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gsotmfbyi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gdrygkmlb.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gqnqzzivl.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkxtawu.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gtkzebrld.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gybkdolio.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/ggepeqwhl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmwnfawv.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gkwxcgopt.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/goridfrjh.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gaqlczohq.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gtqbbcmzd.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gxvmqiuwa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gbcjixgyu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gsxroajgs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gpfbpfbqr.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gnqxwddat.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gwspnvxcw.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gplvsmeuo.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gisxjkacm.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gbsnpianu.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gqztmkvvt.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gzyhasddj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gerzgzscj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/ghugokbsg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gntpnaorn.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gzntiupuq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gdpzisbyk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfrswqs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gqmrvvjsy.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gchngifnx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gukrxldzu.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gkiytlylz.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/goteacuxy.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gyuyzomhl.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gltpucyys.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gwrgkshyz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gszitqihw.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gbebsgckd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gmmnexmfi.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gjbptqqnt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gzeunvneg.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gvzzwrtqb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gquavuyyn.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/ggycnvqca.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gemtcmvlt.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gcfkmjjob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/geoqkerbh.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gzzwynlms.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gkmmcsunv.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gsxtmvpkn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gnoguyymy.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gpuzytzlb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gyepiliix.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gsokjgruv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gpoyypvkv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gkherixzo.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/glxrkhwtb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gktisxzmx.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/guqrffzlt.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gysfqoqaa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gproobrbh.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gnitzlxut.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gbxakamcs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gascdkwel.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqzokfqaf.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gygsjfcuo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gozxuugeh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/ggwkpvsej.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gkicgttze.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gupcvvsbd.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gysutnkbd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gljdaftir.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gsxqhvsgt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyjvwqfth.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gqitwquja.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjsjthtxu.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gqlyvhawn.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gqoobrcuk.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gxexdrpfo.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gmgtauedl.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gpqkhkywd.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gbeljjgso.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gxpufltic.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gvcjpujhg.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/ghwxqzxbo.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gpedrqfir.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gdzsduobs.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gtjocbegg.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gykmdsvgg.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gfxjdlooh.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gejsonemu.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gcsoqzdav.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gveobepcy.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/goqnyclwm.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ggwyjxpay.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/ggdzhfkea.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gwjwqjbzu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gztdwkogi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnjkmaund.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gfwmwrvpe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gqawrahgz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gbjwnhkzo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gkclbmvbq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gvrltoyjl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/ggdqkxsmx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gfjtgfjvy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gxuvryjpq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gjybqfnjy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ggjpbayih.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gxfctqqgo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gblvlzhwb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/glaayellt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/goesbklcb.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gwpnlfick.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gklchjamb.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/garpmbugd.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gfrtqvwnn.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gyfpmctaa.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gbouwuknn.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gstlxctmq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gujvxadvl.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gmrfxcjjh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gnwojgfzj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gsntfkjgw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/grclmueme.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gohkwodbr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gextreoux.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gntyqdabi.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gfgmbdwnn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxmehaocg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gtpvckrtq.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gjlhsuxlt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpbugynao.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/geyldkcqz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/geiquaxxw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gzzhabcsu.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gkbfbwlcc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/goxigxcbx.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/giwjqqirf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gqcdqsyox.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gggndhutj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gsnjriyee.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/ghtervudv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gbigfrmay.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gcewyghzr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gdbcvemxj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/ghjtkcqrn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gbzcwnnof.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gyfreuxqq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gusgmfcqy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gzmgohpbi.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gxvpaqvoc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gkcuccgdz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gcueoajcq.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gavfejwah.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/galyitbxb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gvsbixjcy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gcrgjinyb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gybdigvyw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gzctwsaed.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gtvkyfrfy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gapxajqjq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gawqhdtrm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gmbansvex.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gyyoxboqe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gtefcgeim.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gttpvfyla.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gotqpdzue.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gplpfcumr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gjxikvcib.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gzrhweywe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmzykrhof.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gwxkvivub.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gnkjhyydh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/ggalrkprl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/ghhywkwdb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gpgntgyhu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnzrtgixh.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/glcojzapx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmicorbby.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gqfynihbn.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gaaktsmmq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gyzedrytp.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gafvaietn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gloqqufwa.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gjzilrdyo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/geomjgxvs.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gjzsenwmi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gzcvcmufa.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gsvrveueb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gtywhgtul.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gshxmybpt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gwruezbsy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gqmfzamwt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gurftebke.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gpiflpwst.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gmkeshwcc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gculbnkxa.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gkvmgpcao.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gjeelperw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gyhlymrbz.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gjfkqtphy.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtcliyazr.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gibtxilwm.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gyhqsivld.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gijjlvklg.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqzllhabu.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gtvocyeqt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gqhcioqri.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gwofzwdwa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gwgzxyjsl.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gwbmtjbdf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/ggndhdmgc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gjznugneu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gdjftyvvu.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gkentvvwz.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/ghdpuvjtd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gfhvgwimi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gxsgxpbwi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gpmflycmq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ggqnwsnom.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/geusoqbmd.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gycdyesgi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/grkrbjdjq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxrmdbbbz.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gkkrgfdit.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gwaynqrgp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gmapftqjn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gjulqqapg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gxgninygx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gtjkhjprn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/ghksjljmb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/ghhdygqui.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gtcaacrgq.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gbcmsscgn.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gmeyratid.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gdrzpyjsy.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gghhxnzvj.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gdjymqnhi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gankxzvam.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gpssvxied.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/glyptxmdi.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gkcpjqrpc.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gohtfwskw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gohsfjclc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gpinosofj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gyhohbinc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/giseqyxpj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gdkgwltnl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gxcyyfzfk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gonhupniv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gytujsfsu.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gsnzhgnrt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gfvjucwrp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gjcbmvczv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gecgoufcy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkkdlcybw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gozycwhuv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gmobqfhks.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/grxmximbf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gqujwfrdw.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gyeggfvuo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gxaybifho.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/golzrdszp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gunklamip.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gsnroptci.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gjhmznoyk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gujzvivqy.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gjqygdrts.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gixalodrf.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/geviyvykq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gqzpuzjlv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gwnodhfkc.sHtML


<!-- 参考信息 -->