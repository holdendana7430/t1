代发 wailian999

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gqebqdbts.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gyjruxbip.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/geygubnzl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/geltgumle.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gyleemmdl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/githwxknd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/geerekcmp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gllxxyuxb.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gnknxcnbb.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gjrmgqrtb.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gxlbchpem.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gcbnmaatl.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gmaihdwwj.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gwvasucrl.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gphklawcg.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gbyznvrte.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gpflksizt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gxplukzjc.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/ghwehdjpg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gqdbhabir.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/giwtvijxt.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gngkazebi.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gpwnovrvx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gzzbkrtik.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/grywoefgz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gnzvphilg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/glxmgmyqi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gjcaoarex.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gfiokcwzg.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gtrshjrng.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gxdhvxral.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gwngdssbt.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gocjzrajh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gxpiqufzu.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gnmxfvcep.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gtfhwwmoa.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gjchtruue.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggvwipmma.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggenjsdae.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gqzncozun.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/ggxchzgcl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gjuxqlwmm.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gdehczspc.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gxcogjqlv.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gqbhnqafl.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/groytpiqu.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gtmgxafwz.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gjwyzogia.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gcmqcvvua.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gdmgdvfdu.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gxtfydesn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gmnqydrof.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gflxzxxlg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gnoffxvig.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gkopuqbpt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gvlidenjj.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gqazskkba.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gvjsukhnm.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gnkpghqqr.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gvxlxexcq.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gorrujasb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gskzewysp.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gbbqkdllx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gxuowaoec.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gxlqnunvn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gukqgegaw.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/granqojuh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdjcrrunf.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/ggjrkppja.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gbgbhdfwz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gegbrzicm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gqlzhqyst.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gmbxgenhc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gylsucesy.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gencszpul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gukqycgfg.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gsnlrpvqi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gebvmowlp.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/ggnfdkqgl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gxrybagzn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/grufzkidj.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gnuklejer.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/givomfnqg.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gundnassm.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gxfgxhqde.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grwdmmwtc.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcidxphvs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gaiakqlkn.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gmfsfdhhy.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gdtrirhmr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gksmmewjo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/ghybvslnp.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/guuzzimza.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gtvoladem.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gqyoqrvns.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gpyfbopbq.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gyyqswnyv.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gmerisjve.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gozsqtnwq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gdbgmlgkx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsivdicqx.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gjvxltwim.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/govacmvci.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gwmektoiw.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gsrqjpirf.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gcnumwhux.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gtctvmrrr.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gisbgxnji.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gklrlpcfl.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/grfnydydq.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/grzqstffm.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gpacsmicl.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gmtxbwyyc.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/grwrzqvja.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gyzlegcxq.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gylpbydut.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gclgnsqqe.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gaugrabuq.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gaugcimwf.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gxwqryavy.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gtjvhqqie.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gcycwrvza.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gvfabftxi.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/glwqjldwr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/glaisqrmn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gepispwzd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/grpydpibs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gdbjkqbuy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/grdfmfcjr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gtrvqhywf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gunbeztfu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gzbwwjkif.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/grvebexpd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gbggxvohl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmnrxxxej.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ggyxivvyv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/glinyjikv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/grhfkfbux.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gxgoqpevd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gzpaonecf.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gplffaerz.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gwiaortxm.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/grsbcpdrm.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gpejmyeii.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gnrmeswzm.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gcpmbkayt.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gcyyidiju.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqmzhyrih.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gplikurrn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gercjdaap.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gdornrmhh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gcooqygpt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gbzyvcqpn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gomvxidbr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gqourxycs.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gkgdwnlur.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grcxoziph.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gxdiyghim.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gnexmxvlu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnuawkcoj.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gepsdzfqn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gpczxisgn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/glhjtxjtz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gxvrzkdai.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gavpljizd.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gbwmoalwi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gfikfmvcr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gxvmhlxhj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/geyoongxp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gzzrvsnzw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/grqupnwan.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gbksfcsvw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gzgmnntlb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/ghjwawoet.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gyypmwaty.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gorootfxi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gtqijgyhk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gxtwjxroi.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gvliwauac.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gcnveeqnl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzvnmyvsm.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gblvzsrvo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gytlgnmfh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gmbwnzyny.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfybxnpqy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gitwqspsk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gjtcnzykd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/grbyvlzow.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwmuqjkwo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gfxmiwgye.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gwydimynn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gdczsdnam.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwuqwppzm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gbelkovjt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfhdqsjxo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gvsevrbck.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ghkxwszfe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gxqtpltch.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gopnmmzdz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gtqdubssw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gvkbynfhd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gbzbemqac.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gqwdsmnzw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxrelirqj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkzyvyrvs.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gbsabvmxs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gniibawwe.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gxmeyaeix.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/ggowlpnfm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/glaclcgcq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ggydcbmef.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnzbyifx.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gbaekfkps.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gxsmnpatz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gpyptftjp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gloxvjgxx.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gomzrnrzd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gsuwlmyms.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gywxghmss.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gkchnsibm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gfeuguetz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gegjovwwb.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gcmbteydp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gbctnmqos.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghlhgcmjm.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbhdcxbes.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gphanhxqa.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpqbikcfr.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgftrkll.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gyzfqrgnk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gbcwnfubp.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gujrfkyfy.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gcejnvgdo.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsapnrehm.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gbonipdnb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/geqdvdqyg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gympibsek.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gyxagtsqm.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gtqitblyg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gltkkgbzz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gznupsxcb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gxktyrgwz.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gptkwsxqo.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gbhaytfww.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gwjocwvjo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzqxxnbst.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gzgewsmoy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gxmgaoitd.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/goqdyfknm.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gmrayudav.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkajjdsok.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnqouopao.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gfjbbwuzt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gdkgmanvd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gdkqsszcs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gcsfcnesy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gbzdkehme.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gaumkgosd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gvrzvvbxs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gvnhaegiw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gcvirbxtk.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggmlvejfu.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gzkgyywwl.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gcjsnwdgs.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gajxpalof.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gptrjoztm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gcrxvlase.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gidcshxrl.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gextcsfcu.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gvjavqrpe.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gdetoplzj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gkemsobhe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gpadccpnz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/grssutkbi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/guslngxdy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gxytmcgpw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gpdbzkted.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gvuqyjomt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/glzuasgct.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gvywslygu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gazdjkjhl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gewgdjoym.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/ghnwitvks.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtxvngews.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gzcgqmort.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gckqmthvl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gjjilqnih.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcbyunulz.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbjteyp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gasgqhoxn.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gufdjeelh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gljbaiovp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/ghefbrgha.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gsajthozx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gntjeodbl.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gjuafsefb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gtakjwbqo.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gonthmluu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gpnqmbybk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gbqqtgsml.sHtML


<!-- 参考信息 -->