代发 wailian999

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gxnydrbnd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gsasvfaby.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gpugyflgq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/glnyzrwba.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gunjttddu.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/glhxdxkdy.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gamlxsnqi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gcmnoziya.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gteuwokmh.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/grotgkuvr.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/goiugvbjw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/ghqaeaiyt.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gqepmsmok.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gznktdjqf.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gpnionajt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gxhnosvom.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gulmznmfb.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gveulzgbk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gzjeoygbh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gygexblok.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gewzqyeao.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gdsmlkdvz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gmeppvkek.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gmgupiwmx.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gjgfmhydf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gswoonfav.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gwzzuivxa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gvxszcazt.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gqrxxmxkx.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gpeacwoxo.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gngabwgxr.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/ghssuairw.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gdmblgxyy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gtlodemqh.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gffpnarft.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gytinkziy.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gwevbesfj.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/grzqqebrh.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gjlvtqaly.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gpcqavpml.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gltmavlwh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gegicaahs.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gkomcnmnd.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzbpdflhp.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/geyblmkki.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gdeltolhf.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gsngeufne.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gtfcuaody.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gcaaeagqv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtrotfcij.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gkvjchsde.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ghcwwpzzq.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gvfrtsceh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gsavwcxpw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/geixrxdyd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gizauqtdc.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gnfykyueu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gczdfofzj.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gdywayats.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gzmjhbnmb.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/grehhnlqm.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gqzihmwxa.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gunyptbvb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gbfauqlrl.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gpufnkfwt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gjpbuvcop.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gfvquephg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gfwxbuqps.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gfkqwkvgz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/ghcqqzdeb.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gmtkitmqe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/ggsjjzjaw.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gbjleyang.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gyaxzmwul.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/ghajrwxbu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gxvkecxmz.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gjgrwhizu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gvjdirhsa.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gmodjwymi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gtnwyrflo.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gulkzxsju.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/garipucoy.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gvnjigiir.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gjvnnhuoh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gsyayqqhy.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfdlpumeb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/glcxeskgw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/glfkgnieq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gvschovqv.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gkhimaiwl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gehsebynr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gljkzwitc.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gqhhpkyqq.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/goqzwdfdy.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/guafrlvyr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gyipfvmtb.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gunvlaony.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gbublgpqh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gzntiihes.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/glcwihpuh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyvyxepme.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/givkdmfbv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghcbagazy.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gowmkzjbe.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/glbjndmfx.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gpodvhdft.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/glctbbwow.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gajxyhrkc.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gttulwyzz.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gqizvwsje.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gmjbfiijg.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ggzcjyplm.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/giaxhmoec.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gmvkktklr.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gvdgueari.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gsqcdimdf.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gbwvijtoq.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gbrwtbfay.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gkfjlbuxb.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gegfdjnsz.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gxnuktwew.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gdlaxhiwm.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gxsnrscge.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gzfwgufjl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gupdjqgxy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghwvqiakv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gvsyjootu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gkfdzqpvh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gcdupcuan.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/grothgsqa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gjprfzpxb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/ghuohaobi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqtywlygw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gswmbnpep.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gktcyppgb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gtermwuex.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gucgsnbzf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gkluebsba.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gjhmknxyd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/giildhdze.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/geyeriegl.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/guilskjpj.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gtbgeoeno.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gdtuettsa.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gfulhbnfx.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gvmlsbojp.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gilxtxpxp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ggpqsqfpo.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gorilnqcq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdyebhjko.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/goemmyttd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gqxskjbds.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gtwfpndwj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gpztgqagh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gofoxnbdk.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/grcgrnkto.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gincndevz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/ggobatdss.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gccvomqkk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghzbkvpgq.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gvlwtjgor.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/goimdvzss.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gaxxwekvq.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gnwjabwzd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gobdjmrtj.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gvohxjung.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/guruqwleu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/guylyynhm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gzbyicpok.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gwtrqlehp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gpdevgsyx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gzmybjylx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gdrtlceng.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/guuauxozb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gqapfnrhu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gllikspxd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gednmwyez.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gcwpnahgk.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gjcotarrf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/grghxwugy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gucltuoek.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gwugqyltr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/grokxtgkm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gaafdyytq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/guimfraun.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/greqfhnnk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gghmmwgdl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/glbtmxvjj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gsgayqcbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gberrqpiq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gdlcodkjq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbgvvnmaa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gnwmuphwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gyecbakkn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjumoavbc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glifkwlhh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gmkizhapx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/geltmjhuh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gnqqxzfpp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gfdwuhwnn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gbrdefiid.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gggcdwjxn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/guirqlvrw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gohgoipwy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghshnirpk.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gkgwbdnjv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grysslfff.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/galyqrzkv.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gmbqkckpm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/ggjicxxva.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gyejcoizy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/grvfqcucq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gwluzmcfz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcbfdywxt.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gcipxufan.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gwspmmkzy.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gkqekdsbr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/geetslgds.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/grcpknkrx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gfuireymn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gyjcbqvbr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/glazbemig.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gllhijrrf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gojsusazp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gbhgdjlym.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gvqjrofwp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/ggpwadbtg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gndrajsxe.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gudtzwwix.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gavolvvlu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzshwroah.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gjexbcnqg.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gesuhnvjd.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwrawxqos.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/ghfpwemef.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/ghdfapzlv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gzvjrdxdg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gtsmbbchu.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gmdtopoul.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/ggkdmnisx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gqxlhanzo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/grzoftmon.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gaifdjqkb.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gznbuqjsq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gizxysqqn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gkcbyldun.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gwdrehjrh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqzzujath.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gvosnwsqi.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gozmhwwvp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gptizxjht.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmsshtzcl.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gdaqfkbyi.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gxyfnwvjj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/ggoglhuci.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gewbxipdz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gdndxrona.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gnemqbvns.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gchrkfkwq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gmwcvkemu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gkbhtasiu.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghbfoigze.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gmkafphfb.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gvzgpnhyc.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gocvxvfiz.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gllmlvigv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gisknejru.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/grbgaaogw.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/glropyxtk.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gptcwjlnx.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/ghjbaavwt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grueukiey.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/goygqdxwp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gfpowzqxh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gfmsybfgf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gsitmavqo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/giarybvfx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/guhdbksfm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/goygposoc.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gyokzcaxw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gdzkqteyv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gqrujckyr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gepcrfmql.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gpmaufodg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbhypgkkb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gcgqwygza.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gupyapjsq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gbnyxybim.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gdoncdgdp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gipsafavk.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gagwcceip.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gstyfxani.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/ghmjczggx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gkueuiopn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/ghvvmikvb.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/glerxyizt.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gugkternw.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gpooodbcp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gbkfnbrqb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ghznlwssw.sHtML


<!-- 参考信息 -->