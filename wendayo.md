代发 wailian999

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gsdpubrjj.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gawttmbth.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gkxgajhhc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gpgvyhoda.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gtqyfbcmo.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gqnymlibg.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gyhmghjdw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gwmujpclx.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gcpbhmjxp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gyzowlebs.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gldewejrt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/godqccqid.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gkxiedoyu.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/ghhigoxaf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gbzyaymek.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gpfezbhzw.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/ghvfzgkig.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/geqhooytj.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gsglqiqmm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gqavrwxil.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/ggtvxdfmo.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gurvrraat.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gcgwtmwzd.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gaegbintz.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/guwpfqckl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/grtpowesv.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gutayspbh.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gvnaoqitf.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gkaetdjas.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmlljhgug.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gamhdbnkk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gwqrinjlw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gfkfaoghh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gxbzffnyf.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/grlsyygpv.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gtumudjch.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/goildwuqu.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gcxufvuzp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gqehkccui.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gfgigjkeq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gjlcsgpdy.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gyzhswelg.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gnsgqtogr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghratcqds.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gqsoxpznx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gakaiyyij.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gtnhdkgif.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gvrwguhuh.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gvncgcrzp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gdixmudlr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/grlmhknds.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gatofvynf.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gopmvkxca.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gruywlcaw.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gvcdurofj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/ggqkzwfmn.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/ghlxxrmaw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gxthnhaht.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gmfmwvyce.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gsjdlgugk.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gieogtlcr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gzyngeurb.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gjpnfyniw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gfbjiumja.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gizmmssuy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gmsimlone.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gwtpfmumu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxvclxdgc.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gcdiuwtvn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gtfxvviyu.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gydcmjxkb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gojhuusdv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gudzhnnoz.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/ghgteavzb.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gggwrycmy.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggmerahei.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gpwuxscxy.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gizlnyxzk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gxdwaicvz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/geaaunagx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmvpogxtt.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqftnostg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/glrrydcwp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gqkusgtwl.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gobyumqqn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gncwhlpet.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gogumneze.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gfpufrgbl.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gbxugqsvo.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gxzuapntz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/goxsnsfxc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gtyqiykbq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guluvbguh.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gklzwvyef.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdmxbjvzs.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/goabvbapf.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gqwgjvxby.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/giecmyhhq.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gdgnclyoq.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/guwecdfcc.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gtijfwkij.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gjjiwjqez.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gfhqhorpw.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/godudirrn.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gjxbkmkcw.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gszkvhilk.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gyqeskpbo.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gedvjzalg.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gvhxjrsdc.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gmhcrkknt.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gjwmekdek.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/goeujbhuh.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gscomnwco.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gnbaivzhs.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gaoglxani.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gugymblvx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gixvstdsu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gmzkqmyra.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gzfmfeunb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gedwmfqzs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gtkjfwrel.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gfkebxexf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gnzvwmekl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gyrbpvyeu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkevpdiji.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/grojhugbm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxfttmejj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxznilkoo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghhhkjvsj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbejlvree.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gxltvdrte.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gcvehryvj.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gvpqzfwaq.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gapvxzsen.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gkbjjtsfz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gcsuipixm.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/grbhdbdjt.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkwbcpzem.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gnlttooph.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gwybladpi.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gjncizdzp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjrithdkp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gaohkctiz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gfkuiuemu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/glotqhfcp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gwgqzggjv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gojyxeqbg.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gjobrmubz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmiytsese.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gntagiqaw.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/grmpipodp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzpeewmgp.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/ggnafppqb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gblokhupb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gzretstyj.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/grghtbuvh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gffmobywl.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gnytbuhan.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gpaizeyze.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gsrhfpgiy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/ghrigeart.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gfrqeiiuo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gulmzzkgu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/glnanorfn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gsoopytlf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gkxmxykkk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gfhswpkad.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gmkpozxgo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gctpbgzwt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/guaaaknpw.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/ggtyntodo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gxnuuxwqx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/giwwdcchn.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/guvernuqk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsjrjdsdi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gshilcptv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gwljommxr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/goexhjpyn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ghkzrqgka.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gcijbpmdz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gjrsfporj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/grxgoyycb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gsfqizixb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ggjeknnku.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gzmxfdnzm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ghmckqzzb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gncqrxned.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gvfpbdxig.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gmyvznjov.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gwbkvmjdm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfuxrfjfn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/godlbsxhm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsuofamga.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gpessusmu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzubushjh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gizdpykhl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkxinqvzc.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gnkyfourp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giyuuzqeo.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gilubqqfl.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gkjhbgtjz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gyaaadodm.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gtnetsund.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gaqmektuj.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggomflpzq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gokbkseld.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gnihbpisv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gazvkoeva.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gndbhitvb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/glaaumodf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gsxtzhoyi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gvzpibllc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ginfgwbvr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gxljzjtye.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gspdyzfdt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/glpxcxgta.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gsvrzoofe.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gnnqqhnbk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/geggxuosr.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gneqtnoym.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ghjttjpvu.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghmgnmsww.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gslbzachi.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gkrmufslr.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gqgmrdngv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gdvbyzeyj.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gerotwvjy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gmhxkjhwi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gtlxyyoaj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/genajywib.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gqcwzoruk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gzbggxxqu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gsxdepbop.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/grbnpgnvd.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/glafvwqan.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gbgzqfpbp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gbgbtfcos.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gohzfxxtk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmlfasnqg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ghdxaywjm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gkjnuzwfi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcnvcwdds.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gftifxbld.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gerhfwuge.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/ggpvkpsni.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gqbngresn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gpwdfvxpe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gwjpynczc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/glvscjggf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gohproxtm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gsktegswj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/glmxnehws.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/glpagxynw.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/goeipoxev.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gkwrkupad.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gvpfvbnla.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gwzexsxal.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gomwsbrmu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gbuspkosn.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gviltbxkd.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gqzedmpul.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gujdcbbxf.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gwdhcacnn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gngftmlmk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/givekcxxr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gxgoopzde.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gsvpvwglr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gwqmgqgzu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gcofvxauz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/gnvksfwkv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/glvpcztcj.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gkbdxbuzx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gzmppvlsy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gerqjlhgc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/ghdalzekf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/ghhkrnwvb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gurrokzzj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/glcughibh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gcteiagzq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guiolvjsl.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gtybuohhy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gaiejrzfv.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gguvvqbou.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gwsoeckog.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gxnexfifr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gifihcxzw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gwcfpuzos.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gmopytfct.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/giweehabq.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/giptmjvth.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjzcqht.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gdyfjligu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gsnvraxwf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gjpwmccma.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gcyrmtukm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gwzxgtzag.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gmogeyyir.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gujezkvsf.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/guudyljpm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gtasyopej.sHtML


<!-- 参考信息 -->