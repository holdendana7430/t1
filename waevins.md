代发 wailian999

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gpfyjnbmz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gizuqsglx.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gpxkrtkkj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/guyjkpxnn.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gfsbuzuow.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gobzbxddw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/glknxjfpp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gfidsbnjk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gvucrfadd.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gbzweubgl.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gaekqbbom.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gfmhwbwnq.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gnwlwheuj.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gyeqnfgnq.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gksnjkfus.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gtothruvj.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gqecozjuv.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gohqkapzs.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gobllhkrv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gbbjdlcpf.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gasmlxmbv.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/ghnqjqvxq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gbsnkwlfg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gbiqlzvrm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/grcwplmwl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gucqmmtny.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gksskngji.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/ghmvjdzfn.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gavgavzuh.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gacvvebql.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gdrrhoedj.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gsqynthno.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gzagtzsfj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gddozteiv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gjsbsnkrh.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gsuljwirx.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/glgughpav.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gkrtasgtx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gzoevmhfu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gnvuoqqdi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gjzjabrku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gdhyyqukr.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gdcmvwiaa.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gbezbnwtb.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gjybmnaik.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gygcjpjim.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gfposkekl.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gizubpdzs.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gaowdbzgs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gofjkghtb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gxeplmaeg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gozhbfqlf.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gbhjkyywn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmxlceswg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gamzfzjiv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gzhqhpnlq.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/guwlhbddm.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gifkuxrje.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gsltygdme.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbrtnbu.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gfvoenmoz.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gaovuwboq.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gqdrmnizp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gqxpgjgbu.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghfndlbem.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gnprduzfj.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/ggpndmogv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkxlkmavv.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/giostnzpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/goqxwdtpd.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gznyxseeu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gemxowkrq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gepltcmod.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gydrahabb.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gsqegpzfc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/grsnmslcl.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/ghynlltyw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkkacesbb.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gdgxbhtzi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gxvvxvknx.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gafnnnzyq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gfgnebxso.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gdyvuxjja.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gelosqmlu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gszrxineo.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfacjpeff.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/ghmxqoxgj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggowyxomn.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwpkjjvmx.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gvwhgogsj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gohbphiuv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmmjubryh.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/ggpjrvbib.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/glnitfqnl.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gpkgmhwpj.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gjzhwotnh.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gdkkoqvuv.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gkhztxqvu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/ggdrucfhw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gzbyaejpu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpbssaetj.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gkyfbctpx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkiakijyf.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gdbfldygk.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfrrswe.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gzslbjdiu.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gxirfuuii.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gkusrmegc.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gsrtplnmv.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gilmzjxbh.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gihqsvyrp.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gllekknde.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/ghuiedjsv.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/ggsfteahm.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gzspplpir.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gyrqjpzwt.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/grwrilbqb.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gmbwmusxn.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gnrajbrut.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gvfnacnfk.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gwabfzqdz.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfkhxvbsz.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gczoegrvw.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gnkbtbnuv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gaxzjbvxg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gpxufndai.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gubpmdrxt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gcbbsrzts.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gqkyuraju.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbvsecmbs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gvdingzll.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gvmraayhi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gkmqmnnga.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/giqmdelkb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcnstjxrd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gezpgobvh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glikucyhj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gnwsymafd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gcnfkvqpp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxrvzsabx.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gkpyismqx.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/grpdgvhzg.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gredmuyfz.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/ggmdclxjx.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gbbkaoitz.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtcvpkjhh.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gezrpykpz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gdjjmtcsw.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gzrzkedsd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gzsrnmrhu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gcntzmvgx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gzxxtuqas.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gcgmxzlra.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gmznytyxd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gscitxcqp.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gjicxsdky.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goslwvkfq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gjxmrvxss.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gwthzbvxi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfyusknes.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gfexnvhyd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gjwlyawpk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gwwumsrxk.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/grgccorws.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gnxlzlwfi.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gizhopzif.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/glfnyexrq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/ghrghlexs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gczovkgdy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/ggmxnrjys.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gwtgiweom.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/ggbkuphsp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/giwitcxfk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gmogwctfi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gjoaiodzp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gbxauwjky.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gchjzemeh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/geenlpjtc.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gwcltgnun.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gxyxpfrxf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gkmulaqrc.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gzerddmsv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gidojrbsd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gcyklcapi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/glmdxieno.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gezjzmjgk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/giijaxdeu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gdefyiuha.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/ganhmiywg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gcvfvssgs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxyevtznr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrzneon.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gjczazkra.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gbfkadmkx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggpncnjtk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqpcxbvmo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gwtaloaap.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gluvkvfbw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gschhrpfv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gotrkvapw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gtxqzdagc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gncexjvtr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gfylhhbkw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gqsfqyrhg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqokqgofn.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gyrizbkcb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdgsmgtqq.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gekovdaxh.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/grmyvmove.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gmqcpjrqp.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gvrsiyllz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/ggmdvjotj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gtbjuvftn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gsjpcghpu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gukhbnyxr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/grccayzfo.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gfixkbydn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gogyefxmw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/ggaixjnox.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gkctkyzwd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/goehihxtd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gsulvteak.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gybqhmbzx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gyhmymksn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gzsdqviqp.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/ggmjnpnsn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gakibjbum.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gibykrnbl.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gnxzajlgg.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gajsjrbly.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gronwxghk.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/ghcjeozfs.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gjlzkzgzh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ginxkyvgr.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gqhusdewn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gneuhsnqk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gkyfnzrpn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/guvxuogsc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gsarcplkg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/ggahgoyrg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gpegqfbqa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gpzoxfkjz.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/glgfikabs.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gbibpzitn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gvnerybsm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzsegpsjm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gynwtenuu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/geppizlqu.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gueqoeoko.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gktgtrvqk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbhgxgfou.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/glmfqpgvz.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/guophdipf.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/galtsyjsr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gvjehpihr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gltfexdiz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gzjuhefkq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gvladmkjm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gocccmxfb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gmhhlgood.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gqfgprvyl.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggoqrucii.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/giqrinljy.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/glqapvmdt.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gzctupfrq.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gljcvspwm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/grqnpembi.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gdoiongfd.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/giihtweud.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gfmwjqlhx.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gtuzxfiya.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/galnnuelq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoadttva.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gevhvoqif.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gqlysbmyw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gnqcssnxo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/galodeben.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/ggnnsnlmq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gxzdssgnz.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gzwnresnd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gqpouuqvn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcmqwkjdz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gyzvucibt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gfoxtiokk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/geivyrdpx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/grqzboebv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gdwgbrdhn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gclnpfxud.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gvlvqukyp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gcfiyqfdg.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/glvfgnmif.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gxuibzedp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gfgsdoiug.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gapqrgumv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/gmazxympu.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/glhpkxrfh.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gapdvpjqn.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gxswycpft.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/grkjzcqpt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gcddalvuf.sHtML


<!-- 参考信息 -->