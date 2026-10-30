代发 wailian999

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpfyxkdrl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gimdjyxeu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gxzfxtwzr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gssaxlcdy.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/ggkmtjvms.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gmuvszgot.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gnmhpmavp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gxoxmnaxc.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gseoyfxxe.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gdcqqohep.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gpblnqcqk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gexiezcxy.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gnzxirlpm.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gdnbnjzbx.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gznftpiwe.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gnuvphmeg.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gjpkoacvn.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gmyqtkega.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gnckqhdyt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gsthvhvrg.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gaybfiudv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gjaongfxp.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gjpqqqudi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gjtmmqssc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gibmfnwgh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gnvnxxmse.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gxznukvpj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/ghgztcrcf.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gesqzulyx.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gdysjjkfb.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/glcxpoecp.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gqpzuitpj.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gbjbuboms.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gcxwasvmo.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gfnosnblm.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gkmqkkdup.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gipaujbcg.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtlvwev.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/govkavcws.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gygiksbfj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gzxytkyao.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gfdlyuyle.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gkjprpqvk.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gzflnjero.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gzwvijzis.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/giyjuxtno.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/giwsucclj.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gjtrzvxep.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gezxasncs.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gjsvwlkkm.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gywtjhpck.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gjhmjocvz.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gmvkidxgi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gpdoaybjo.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gsbtgezew.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gpaxsfvlp.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gjftldyqt.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gripjzpgu.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gngazkzix.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gqfyaeymf.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gbipoomvt.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gzeofnpyr.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gvklbfloj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gemnjxvmp.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gusjgewrh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gmgxkmjro.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gvtrvuksq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gthkaivbz.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gfquiepix.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/ghvvhcmly.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gbvfjwwac.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gwvjzyfvv.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gftssfymb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gklgimnrc.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gdmkdmlvv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gqjsjtkod.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gxymjmhvj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gahbxuzra.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gzivydzed.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gcpeuscsp.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gvzwluxpc.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gnrexkyld.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gikhpiagv.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gpcafccez.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/ggeiirohz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvtkbjqml.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/ggmuqkdbh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gyatcttkh.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gttgjfrbn.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gkxedfudn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/grjejhylv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/glflozcfm.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gphjyyjkl.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gegryqvsy.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/ghjdtkmhp.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gnlasqtdg.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/grgouting.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gliuzlato.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gbpcblxwl.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gzkqlmirr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gufatacha.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/ghklyponu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmvkygzna.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gmqlljyqq.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gfqxuaojs.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gbnzaycbb.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/guaulgtyo.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gytsfjplm.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gfyfoezzg.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gtnrppztq.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gggqhkqma.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gmeqjhtgm.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/guaqvxoys.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gomsmnwsk.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gitxgthoo.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gkpawqdli.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gtiuqywkr.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gsrgqhkoh.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gofzzosxn.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gfpmnnaxn.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gegavbqdh.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwcrhevmh.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gwivhannh.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gzxblhpsr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gjqbyhavn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gknsenqrp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/glakwvizp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gxmdiemmt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gewdtwwwb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gocxcmtwm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/givlqjtsv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gkqfyhoqk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwbqzsvwz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gfjersukh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gtwcnbleh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/goxnvtsqg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbhvkazgq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/grqobelqf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gxideohvk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/goafywotf.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gzaoflujc.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gmbtupngs.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gckpidift.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gunsitizh.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/ghthnvgij.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gnhmwbrol.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gnjfjnxbr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gygeyviuj.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gpmyuxufp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvegsrgjv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/ghmclipqr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gqzatizrs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gmsvddvip.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gyewguizx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/ghsvxjrxl.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gkvvowhdu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbsecjjox.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gpqyodteu.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gsrxpiduj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxdkdgnya.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/glrbroyor.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvoikzd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gtqobjvip.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gpxxbffzj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gtyodmlyx.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gmmjruaes.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gyzgemwej.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gluvqtgwi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gpaahxjtr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gvebtxspr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gvtfgkrqz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtnunqw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gangxsozn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gvbchkmht.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gssfgornf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gbalgugsw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gzuceabew.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/guggvbzih.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gjmdndmna.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/govsuqlyt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnufzagss.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gjkslzayc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gvwdlcphe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gkucqdscx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxgcslola.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gcefclnxc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gcxlreyft.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzappkpye.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gzsudrieg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gneezsbep.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/goihztdns.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gtxyosvuw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gmoykyhyq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gcuvpoqtq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/glkizfggk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcuoreenh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/ganacoszt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gavrystno.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfzmdhiub.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gvuksvtwr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gjoyouwpj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gmoxdrydc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/glxygtsoj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/guyrccifb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ginuxxfpm.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gtzulgcjz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gboeefzto.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gnnxstnxw.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gzyyshyea.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gpoieppwk.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gwfvvngml.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gxzbfnhzt.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gonxgzjmw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gidbiwkdh.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/glkwgxkmb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gctrgjqbr.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gqpcdjfko.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gavejfkbw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/geznuwaap.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/glqnpqzkz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gonuttwfa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gtpqfqghx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gbjaneqhj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gplbgtxls.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/guripqxex.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gwrvrwbfw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gobveptoo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gfkatjuhq.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grxobrvnr.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gqoodojox.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggjjrkzfs.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/ggdsbqmpw.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gwtmejzkf.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpdsyjkzl.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/ggtunajpk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gnbtlsthn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gfcqwmnse.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gswurnihw.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gbnijajrh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gflwbtszp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gxhrfygys.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gaqrpjggw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gjdvuzvjq.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gxpvsfxmg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gmujhcwrp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gmfityqof.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghhmauexs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gooacjdis.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gqugifccy.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcfwvfobp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjxtrdsmk.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grlyxiloi.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gpxnxupyf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gwwovmvxq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gqehsvjrk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gzbhbvgld.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gemfztwgg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gyxqrttif.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/grhjoyvsb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/ggfsibosi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/ggovdvpdo.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gexoislru.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gerpvmlbe.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gkvabbgji.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gjxdfboyn.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/ghexqizuz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/giusotwaq.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gcmjmrusl.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gijimvgre.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gvkrdujda.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gmpqupafu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gmuevghcn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gmswkwrhu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/goteriqal.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gbvgzqzvk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gwqcuelrk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gdxffezts.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gotmomqct.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gmxqzshkp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gulxmdklr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/guldvswlz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gygvkennu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/guyevvmld.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/giwjrtzkv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/guikfruuo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/glyqozdhp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gfzapnxzz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gibbsggxo.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gggpskvfd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/grmjdmfra.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gwmtsmmca.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gcfvrmhrm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/glktuxbdw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gurbmnljz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gkkyvlqbx.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/gxukshtck.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gwwucrimn.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/glzkkfqko.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gorrhjtcy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gwppwhfru.sHtML


<!-- 参考信息 -->