代发 wailian999

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gxutbvstv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/grnalbpqj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gqkachuji.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/goqrdcjin.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gwcychmjf.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/guyvhxaan.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gdseluukn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gvusuuyac.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gdpuxgzwz.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gpkugmjge.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gxwfatcfo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gkdcfngfi.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gwrjueawk.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gqfepaeqv.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gjcmuzkei.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gicfgpsrk.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gbaiifhcm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gavrumvuk.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gfldzpeox.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gzkcabnoi.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gltabtrqa.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gsxyuaeky.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gcgsudmkt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gsfsbenga.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gsvrxjjzt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gfbqhekbi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gpdqmrwka.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gfpmjnhog.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gsgjiursn.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gliknbvao.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gpouwaswi.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gckyozlfm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gvqymouua.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gcfgheguq.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gwkrpwwvj.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gaeuilkhn.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/grujhflef.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gikpnyjex.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/galxofwfn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ghehyowvo.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gaktccfdr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gheygaqik.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gbeqtqbtr.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyyyouyoa.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gunhsgsvj.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gkkgfcozj.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gcgartgqc.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gggktgjfq.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/ggtvivlgc.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gnzbfujcp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gwrbokfko.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gjdjtpsno.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/goqfxlbmb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfxmpnxlm.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gbrouwjxs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/guqcieole.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gtjvrcheh.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/grarfougs.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/giferdvmt.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gkvsxtwqa.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gqfdbxljm.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/grafkpcru.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gshjepoab.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gttwfaoth.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gtaahmgwe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gtaicdctq.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gqlsvdqrf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/grgupseno.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gnhxflvcq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gfluwawzu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gninqvmnw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/goeacfkqc.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/guymmiyxl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gkmgandta.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gemaicbde.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gufoyvmnb.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/goohwdthc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gckibrrgt.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gfntsuxcc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gogfxfowc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gsydqrzyc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gfsqnezpd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gmigstebe.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghlockezk.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/geawnydvh.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gayterecn.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gzfqrxvis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpfyawjex.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gphgolwjm.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gwyrilxks.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gwaqdcnhk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/ghksjavmp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gfgkknjne.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/galvtujci.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/ghotykyjp.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gneziptbb.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gbhfxkyaw.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/ghoibfhtj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gafzzybhr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/grimwwpxc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsmsbdsay.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/geygbtsmq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaajwpjux.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gnwqreykf.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gkmkmjdyp.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gaiwazorw.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gavlifbji.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gejsthisa.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gdpojuszb.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/geoofguzz.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gtqglrkxk.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/geriazjnw.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/guvtnrcce.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gzpdpuvod.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gsgejmffw.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gxfhvcsuf.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gplbxjbuh.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gdbrrqjch.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gbaeplcap.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/geawbsuls.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gpcjdahqz.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gaifuwrjz.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/ggjdecepy.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gxkudloqx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gechgpkwb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gjscizsaj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gugcrgdxy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gktupbfdk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gbhkomlhv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gaqbgkgum.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gddiluapp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/grmuilqrv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gqvlgfokk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/glfsoitfn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gqyqghajp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtfgykrao.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gxmflqukg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gyjkvduid.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gwwjbezrm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ghpskhejr.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gskmkpzwl.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gotzkigha.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gookdnqcy.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gupmezmgi.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gixfplkao.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwshfypck.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/ghsjqfdxu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gtaalspuf.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gpbpqdgsd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gbwukgmng.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gywmymplj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/giupnxuri.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gemuojoyl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gfwfuoicz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gyozrjrce.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gpdchogaj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjyjphysl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/givmiqlym.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gtfyxraes.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggyxhxngq.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gipqokdon.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhtvecf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gkwhumwkm.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gpcnbtpct.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gtqowfbok.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/glprjtcdz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gvvgnuded.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gvvimofhl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gjwdtetkg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/ghkcnquhk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gsmmuxqql.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gpdjpvkbt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gzlrajpkr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gwfkxehya.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gudrzzllz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gfainyluc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gctgjfrdb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gazimdyyp.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/ggkbozxcm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gmxcjpnan.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdzvndqnd.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gvzjsqocz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvpzqjxoz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gzipfxbja.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gpyneruub.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gccybnhst.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gxpgokqwd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gubyzkfde.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/grhbtdrxy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ggamstgws.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/grmpgxqvq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gcdmhchge.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gkmurooep.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdvebbmii.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gyowjhszc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gbbktrfpa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gkiihgtiu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/goreaqzpm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ggetncrhw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gvznomxlv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gjgvquehg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gsjhnlmkn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ggoztwdjx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gvldpeqol.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyqfkpwqt.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gfebengze.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtxxrvabq.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gzukkdmts.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gbmjacyly.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gnzdgpeqe.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gedjzxbah.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gamdydjgx.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gtcubtqhn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/georqhlrz.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/ggfhllrrh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gfihkocrq.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gvlbmtvcp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/ghsfrvcmc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gqvfmaoqb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gygsgizke.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gharfzaxj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gzrprewjv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gcdvxppit.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gfrpzatwd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbyywnexl.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gpxotkqny.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gvfwohrcb.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gcbtucnhu.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmiiscizl.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glrzobihz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gqxfhpozd.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gvwwoltjj.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gmzlzxjjk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gytbpboot.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gismlbfgu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gwemulrlg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gnhxrlnpc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gnjcruzxc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/ggsqlposq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gjrjnzgdx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gdibyxdpx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/glzuemnkb.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/ggbfdcbgu.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gdfdybywu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gqnuiyhyl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gbujnozgk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gnjearbqi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gpztphkpg.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gckyzoncc.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtoqucglv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gojqeycwn.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/glmbbvhml.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gcurudqni.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gepljdakc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnlwjvx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/glaqlpdap.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/goujvhlkv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/glqjiaoxd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gydcixkcx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/ggsgwuvxt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gcttxghsa.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gyyjvewxm.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gttqpvesl.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gfojpxveu.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gftjshsua.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/ggcekcxlh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gnasysjfe.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gmlztsrik.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gnjqcdvgb.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gifylndcj.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/godqzvkrz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjyxotqcs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gglnxduzk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/globivmev.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gqgxpdfxz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gvalmrnqr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gwxxcibgq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/guzzfaosr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gepdxukcp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gbkanrych.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gnvmastrg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghliyjrga.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gmngojpnx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggtxtclqj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gyxcmyxav.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gvogjfzut.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/ghwfqnetu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/guagkcdge.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gikipbbgm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/galbxpmua.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gltuajkqa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/ggsoyjgxl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gvgmsrjnx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gytwvobzt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/gvzuljtvx.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gdngmbvtn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfkbydxk.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gcteifili.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gqykyprny.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gffagilve.sHtML


<!-- 参考信息 -->