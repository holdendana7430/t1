代发 wailian999

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gatztkqob.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gjqfbihwq.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gzgtkwvwe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gorsqqyyf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gbpbmkkdk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gvakinmlf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gnfgugdvx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gpydjfubg.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gokqpdpga.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gufzazawv.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gtwnhifsu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzgwjerv.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gwlsjpnwn.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/ggygjazfb.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/grtdgzpme.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gwxvivodn.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gxvnbtpta.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/garfxtadj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gbmhjgzgn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gxhetzipd.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gvaytocbh.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gtepmrowy.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gfdkdeipm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gpyjgreqo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gomiswgki.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gyclqvoxf.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/garwofcpu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gkyzjelvd.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gjgzsosad.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gbgohmzik.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gnwwrrugh.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gzogzhzxi.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/ghegwhjct.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gullklxkd.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gbvcbmadu.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gystmwmqa.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gtjpmbgli.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpcgeme.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gotwbivnt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gziowacmd.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gutzattxg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gguclsdyc.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gfxjldhcs.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gwyydgghi.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gvpmswgsm.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gvslxlgga.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gxkhdsswd.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqakldywb.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gjifhzrfd.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gyyjrytqv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gqkiqgydq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gozedrlon.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gbxpkxvmc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkjnmhjfo.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gtgcfffzw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/giiwjlcvq.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gnprmfcml.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/glbztfxeo.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/goclkekmc.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gzjkvircn.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gtrhdwfes.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gbcetovxp.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gumhndvga.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gpmpsngko.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gomllucwl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gmjnlhlnf.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gycxywbrf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gfvenboyv.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtqjuvcmf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwovsxvhd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbffyglgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gbmcdjxnf.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/grulkgpmt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gseceppne.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gridjikss.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gmiaevliz.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/ghgwoeymw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gyohxanic.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gwfaubgrx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gckrlotgf.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gydheuheb.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gwoanybtq.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gdlimdiep.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmrorkrmc.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gqfitxocy.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjxqnkzlb.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzqsfunqx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbplowabq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gygnvvcfi.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gqqkempyn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwqyvys.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gzjkktcta.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gsvvjufqj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gxsglvsws.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gqzvjvwbg.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/glupwzzmy.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gdxqhcwvd.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gnrlbihkg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/ggflsdhrc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gvgtsjpxb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gugmjunim.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/guiqzruyb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghrequksu.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gicycrkkq.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gowcuxpkx.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gyhdcvvmk.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/ghqgobghp.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gjemcgvwc.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gzkvmkmuk.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gjfmjxpoz.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gxezwvqjx.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gjzswfgzm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/ghjpphgbs.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gocxtqlsf.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gbpuzmxhp.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/ggjmwchkn.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gkthkcpnr.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gthbvsszg.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gpahfwqat.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gjijijoen.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gfdaacdbo.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/guvnrassu.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gizziiuez.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gudkiargt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gthfthzmc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/grvxlujse.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpzczldoi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/ggebeslko.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gyzdzqzsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gozmpijej.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gnpwdchlw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gyajugmnt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghhuicfes.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gsdgxpgce.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gsfurpshy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/geqbljilp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gayjywloo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/ghuraeqmi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gjdigpjrz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gsqbaarlb.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gnbifgyey.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gnlklhopx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gouddmufq.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/goeyfwbjt.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gmhjyvnwf.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggdctblrr.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gyvxmoimi.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gntxykjpv.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gattejkyh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/glmsvhbza.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gydeopncz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/glzoijvht.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gkkbluqzt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gonhegyuw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gzcsylvfe.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gxwhrravq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqvaothvx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/ggfeejpqj.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/grlvfocik.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsqcekssf.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/givkrtwwg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gdcigqatp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gweycjelt.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/guwxsyvbp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gfmatvokf.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gxfyycivc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/grgzadnqh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gmlsafkmi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gjweonivt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/griqclqqv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gjnnsycbh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/goocyfqke.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gyelgusff.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/ggyewnmfc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gxmesphhk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gmwhvfpih.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gmgydyuml.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/giyizftic.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gppkwpvcl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/girzthbom.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/giwlzasgg.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gzqnmmref.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvhinszue.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/georktjhe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/ghxpopgdl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/ggvciqaqg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gxtddigyz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gzpuaflrd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/getjqzhyg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gookinqma.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gxmyqutky.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvsvqlakh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gismzodvp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqgnhnwzp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gtfiexfhh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ggyuvctmn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gfrvhagne.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gjhlmyaat.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvsywredn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gtnmsqqye.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gafibltro.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gtlbgibcf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gcvxheuqo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gychpugcs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpurbozap.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gelbtjoey.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbxqiutvf.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwjffbxws.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gvlgqlbuz.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gzeotvsjh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gxbyoxvoi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gcwhmjmcj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gxpmjgmkg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gvgvdgmai.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/giuryfcyn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gzrmjsflv.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/godbjtmcp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gurjikvrg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gaibuizfq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gycpqjhaj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gaeovrvqm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gtlbdwkoy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gdhemoicw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gxxehvnrf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gmhuentff.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gfeuonpqp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gprplqxxu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/geaiorzty.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gegqmlddd.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gynoqxvva.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gegllsxzu.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gicakcuix.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gbnoxeyvp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ggqsvprso.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/godximqol.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gbiqglaru.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gxkkjshes.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gzdfayldw.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gqxvaekwe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gjlelrlvm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gmhllwlir.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gdpogxppn.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gbrhrmlly.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gjocgrorh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gqjkepkpw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ghptmjicy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gybcmvzbr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gmxnuutxu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gtlaorayq.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gohsldkgs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfbvaiwej.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/grlnqwsnj.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ggthqhjov.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gtjedanta.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/grloivltm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gylkfvwbk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gpnzceauq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gtedjdina.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gdsboowom.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/googqxkjp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/guwthybzn.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gxiyyvmhk.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/glzowexeq.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gooyfrwiz.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/ggemqrobk.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gsfxaiufr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwuamgblw.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/goodoudff.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gaavsydlt.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwxcohpl.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/glmqraiuq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gawygjrkg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/glowcxjsb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/guisfupzf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gotlcatho.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gzmtuygfx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gshcaatgq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/grlkvjyxg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gblhbfzkp.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gzrxuoroo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtaohnnfw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjketqdek.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/ghpzvekpu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcvpppdpl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwuoileva.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gqzdulpxz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gwaqlspsp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gavurdvyb.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gwrrvevda.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gzrmwaoca.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gbhktusjo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/guzanqhwr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gmedzqrvo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gnjrfoook.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gkqxovofr.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gtamiitup.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gtypsqtyy.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/guuvfoqqu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gabbomyjn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gtnsdhyyb.sHtML


<!-- 参考信息 -->