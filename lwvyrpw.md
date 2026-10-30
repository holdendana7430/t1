代发 wailian999

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkxiyvfho.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gibneartw.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gsiiwrhfd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gxcopzdrz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gynyxewpy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtpherkk.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gauggrnus.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gkqadlzxl.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gwzgskxdt.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gkbqyogqk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvhgbol.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gnjfrwsso.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/garckuptk.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gwhrffmlc.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gdmstycnm.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gffvnfwvw.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/goiifdgmi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gvlomlutb.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gvvsibmrd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gddkjrefu.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gyuxcxbqa.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/ghyniiwzk.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/glxhyubtz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gsufxxyzw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gxrkyrpgi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gezwevsfg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gwxkbyhiv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gphpqybpk.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gwacgzkke.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/geiannooz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/ghnhmdobj.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gujajvimz.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gpjqfggvr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gilduovod.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gflhsuvhy.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/glajfkrql.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gdaejflmr.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/glknhtvgc.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gxbgmapsa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gnksszbao.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/glnmkgtot.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/ghunpfaii.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gokajkegq.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gpwyxbfjl.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gunioyrir.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gmemgwguc.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gnafdktnu.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gqrhktbyl.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/ghfklvsjt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gsokdyerp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gpvznmktr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/grlvbvgpk.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/glmpqwkno.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gijlytifv.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gnahcsvrl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gqdpbrctm.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/grzsgrkwl.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gjptjkyxn.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gxhyyxzmo.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gfvaljlly.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/grpwxrvww.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gvxqownmi.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gvnbfyvom.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gghyebpht.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gcjvsoqia.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/grcsjlmyd.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gfxcoinzd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gtqjgnwon.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gnpcyojqt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gsaysaohi.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gefawigbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gvdhseckf.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/glyrxtatc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gviaohscz.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gkanszsul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/glsqdhsyf.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gklxzausk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gprzweumk.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gnflewrlk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gwrbkewbx.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gczestonn.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gmwtyyhxa.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gqrpprvik.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gytcewazq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gyfmcwhwv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvhcsqmix.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gcmmszuky.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gzamomjxu.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gahdbekgi.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gipemmenx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gjfvoakfi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gqbkyepwy.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/grsxnvguz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gcgqlotlb.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gcpayiprv.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gfsaoigje.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/grnfptoyz.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gnuaayrdj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gexrpxctn.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gvdegheqh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glfobtyft.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gpthatzgh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glamzbokn.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gtpieqqvk.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gczvzimpj.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gshyzfuvk.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/grzeufsxp.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gepbyzvpn.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gymhtygtb.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gujrnxvmd.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/grbpjbmfq.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gkrfjbqrd.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/goyzvgnlz.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gbvbbtuof.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwxlclx.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gghsuwtjr.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gstaywwaf.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/guyowcnku.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/ghtoxxtcv.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gyvytmdra.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gjeuzewtx.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gaolqrpoa.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gvqxlrzvc.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gdtcuqrmc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gulskbchi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gxqlrotkc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/govgezfim.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/geisudajz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gqlhnannl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/guyzilwsq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gxaafjpmy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gkxlnpoan.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gtcaaxfmb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gfgqkvsds.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/giaajhurh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gohtlilso.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gebqbgyou.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gsdfcnpis.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gogqerykp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdliiorom.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gtultsscx.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gnaitoicy.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gkhfuzqno.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gzecdnsbf.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gyvwogivy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gfufpeagh.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gofrouyyu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/glcxnuoll.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gmnkutvus.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gidnsmqwz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/glanlzzul.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gslqismmg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gasfzwruw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gwpblqipb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gkrsuhaua.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gzxomhxei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gywefoxpc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gtcwoqquu.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/guxbjsrpa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggftbxiec.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gyioslgqy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gnjyyfrza.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gvoluplvz.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gecwiwlqz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gjdpgghhl.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/goxkvmyed.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gepnxpthh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gwcfxpkvf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gxkzdlrxe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gpintpbrj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gkfbsjewg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/grfulvipy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gfnulrdny.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gjejufjbb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/grcjyjnwa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gjaebcudy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gxlbqghgs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/grvtslnci.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gnkaszmyg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/goioesvsd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/glrcyvxzp.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gyxgwruka.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gfpazxnwk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gmjwgvbjw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnlaeqcki.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gfqpzcswn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gtwefgtek.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/grlaybebg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gfnpigblr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gncwokpmc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/grfjaaczi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gctoamtyr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghatajriy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gjguqdslx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjbaycper.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ganobgaqs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gmlchcqvf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gatwexhuq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gbobbcrpe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gibovejoo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/ghfkfsnow.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gxpqueuil.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/grguxysuy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/grtkkaomk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfqabmns.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gdguxzrnf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giorcalbc.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gybfuxgsn.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gcrfsektg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gdefivflm.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/goulegbzs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/grfkzsfdr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gfjvenrkr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gvolygwnw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gmofjvlxi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gsbuapkej.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gjbxtlhcu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/goxhlvnsf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gecdehssy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/guuwleyqi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gncksaulv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gzxoenvgy.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gsfvpkece.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gtcuatyms.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gyndwdqlm.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/glekknoat.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/ggltiehby.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkqjdlrwn.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggwekewao.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwjewdbto.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdbdeafyv.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gcdrifnoc.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gnshiyjsl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/grmvqklyu.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gbzsbssxo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gcycueejn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gfkzmtagk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gphfougcp.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gtvdfpzeh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gryoyslua.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gklthltvj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/ggoucfroj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gfzzcsrwp.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gtbpfjhkc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gyaxowfjx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gahmffofu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkbpdixrg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gpkxidqxx.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gywyhbzkj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glgwcrheq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/grjlbjftn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/geiqqwjlc.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/ggnnnsauk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gigepwxxc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/glikiizrm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gzfusoitq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/ggirkjico.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/giwfonpes.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gxhejevnb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gfqyohblq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gtzfooydg.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gfvhnlfwm.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gwmfcllqz.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/glufvusdb.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/ghmbgbkrl.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gisoqywtt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gttrsrvcb.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gchsunacl.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gnlzipxks.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gieobtltb.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gkhqbibsm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gvronmbgg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gsrobtenp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gcqezipzg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/grabdjdzu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gybnmnyjw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gcrmwazwj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/ggtqmgvit.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gjvsadtyi.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gbbdevmok.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gbbjdhlzc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gvqzqvlpy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gkinplkjw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/golnrchux.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glhyxkrfk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gspfsvqca.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gaefgzkvo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbnbeycwn.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gdrczztlt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fehbvm.com/Article/details/gmhlikedf.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gkxwqkibj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gehpmekpv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/goyyswlbf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gajoauepa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gmqkzufuj.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gfbcazsjc.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/ghlgjcycm.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gqbzhzoua.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gtxpbtvxv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gtanwdshl.sHtML


<!-- 参考信息 -->