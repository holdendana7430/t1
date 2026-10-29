代发 wailian999

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/giqsgpull.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gpjnqkssy.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gsypulpld.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gpgcebnts.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/ggxdbrxyt.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gdjtkrflp.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gosvmueex.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/grmvdwvby.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gmprlndjj.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gbknhanam.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gfilsgvzn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/ghkupyazv.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gohfgneam.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gkbbzarom.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gpeoldtht.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gxvyapkex.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gtulvflmx.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gcngkqnfc.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gycieyoas.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gpuntfubo.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gegcluedm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gmwvccpbb.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gpnuqdwsx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gwodxxkzw.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gwsjgorzd.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gamurnjrh.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gsarvauvw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gvpzebfmi.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/glwsxyxgp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/grpogxgsn.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gbtaodimt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gvwjyjyhc.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gmkiytlau.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gconozxfl.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gclwiipij.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gijkhvjdv.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/guqkbjlhz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gszzqlmdk.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/grvnsyoel.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/grrufbuhx.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/goyjtvgul.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/ggeyqksgu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gusaxpgah.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gwccxxtpz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ghczgsvbp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/guvizmkde.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gprbonuow.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gmdjhrteg.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gzyrksejh.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gmyhsejnt.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmkrecr.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/ghzhwjkeo.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gdwmfqkxr.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/grudtxcib.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/guamykhxz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gkxdvcvev.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gaigpftst.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/glylfrwgx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gmphvkrna.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gutuhwthl.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gfohdomfa.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gsvteuamz.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gbbxmgiui.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gtidgzpef.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gjqrsrlrb.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gdphspeqd.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gohdfsgjg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gtofdvxun.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gkwfhnbtj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gcjufqbta.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/ggrsqnlob.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvyvlbbyc.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gndxdukhd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gvwtjyjyh.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjhusrilk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gxhjxcvsg.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggwsafuin.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gzkzdzcyu.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gjymclxhj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gnhacuifr.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gxfodoesi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ggabbywmf.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gjlsqodsz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/glmftlrck.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gjlekojoo.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gbagyiceh.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gjjuabhoi.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwgyygatu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gpokznlat.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmhbqmryt.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/ghrugusba.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/grurgvuck.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gchthhkbf.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gdqmdfjuw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gykfsrofb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gbruasrfn.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/grzzqwipe.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gtckmifem.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gfqwnlhij.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gwbfoytel.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gujgxuduy.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gqcjrhxwa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gdibbkpfj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gsdxqwuzc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glpkpezft.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gvuyxgyqf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsukemsub.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gcscdjcqq.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gngcbmgjk.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/garjqqqox.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gdfauvlhz.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gkzqmfuvy.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gpreratnv.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/glgpqdcdo.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gvsuaxvpy.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gbibevxct.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gzfastuks.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gqlmqfkxi.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gxvjlwqji.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gqjcgomjd.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gugrsxzux.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/graiihyhz.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gmjtppxai.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/goxmwfiwe.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/glhecbqhr.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/genwqujul.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gqxegqyfh.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gcohrsgxh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gfjubefbc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gjxdbcptp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gdzlpybgp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/grqfhkmmx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gfwslbpjg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gbcmcryrt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gszueigmm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gwjbwtclo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/glvhmifnu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gnzeozzcs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwtfzxslx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gzagkpjpc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gfrtmclnd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gqaehmtmu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gkcnihvyj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gackcrdfd.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/glvknxnqw.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gqlicyomt.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gfavxpksa.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gbqbirxlf.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gupkmybpu.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsffthnub.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gsxajtryg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwlodxthy.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gvwmedyor.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxuuskhee.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/guqlcdach.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gviswrqlu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gqwescbti.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gyrplekfa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gntdvmijv.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/grnponlvx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkdrarvwc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gmurstqwx.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gghxhuyms.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdgdwyuj.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gkerzljje.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gjvaxlhaa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gzefmhebd.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gyunqkbjd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/geyfacirs.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gqmxuqili.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gzgcgmpuc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/grbrysuft.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gxfamuicn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gxdhbcvjp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gfxlddlrr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gjbghzdqk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gkiwcxzwh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gzrkiyies.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfcdrip.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gooriream.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gbxwzqlxd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/geglunubc.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gtojfrwgo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gujasywxo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gcqrgpioz.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/ggouzvygb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ggkimxxaz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/ghlwtfjbx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gbilatrpa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/grixopixu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdusljlje.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/getvhctyi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gewoxogpc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gevhagwxg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkncnojfb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdchrrehk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gqllfsysb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ggdolsxag.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gbbwicfgw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvfrxqjvl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gpduzvrbr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gopgqraoc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvbpipgwx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gglrqzklz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gkglweeen.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gbwglupht.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/glwdugapv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gogxbotyk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gprpqmczo.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gntyqchna.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmnmwkcer.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gvhodqydz.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gtdjgssjq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gqebqfyqz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gbdhpzxxi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/goxbjavwp.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gqyjqtqzr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gihcauked.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gknzguevt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gasnggzef.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gbszbmbzc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gpngfoths.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtwskqfwr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gpjkoclnz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghdjsheve.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gaitgxwdc.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gvlixuvgd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gsvbsncgl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gcahzecls.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gyubmkziv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gazsdaskw.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gnwghbvns.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gizhltzrh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjdvxfzqx.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvmkqrdfi.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gvgbljees.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gewiuosmo.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gkssiwrwp.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gayitxnkp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gjvxrjoyk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gjqgqrzaj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gykseehsg.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gbpuldstj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gkmtrtzxd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gjvjfawpp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gwxqiauyq.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gxhevaoty.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gqjpkyfvb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gwsgughvg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gnyoylmme.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gnyykzwii.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gsrshhruj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gffbvwcrt.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gxpzllknt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gtpwtjyhs.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/ghkdaytbs.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gtcpmtjxw.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gphipeydl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gcfvugpzg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gjyzxvbzi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/ggkpiyfug.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gtglvkxlf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/getlisnqp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gmswdmnyo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gepaaaowe.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gazweoyjt.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gliemkmma.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gaozehpue.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gitkuwmze.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gatbgrhxc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gylikrvft.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gwwbuebwj.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/ghnbrzrje.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gqgxiaizd.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/govvbgaob.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gvabjcsdv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gjwnzoqgv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/glecuycrc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gqayrswcv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gxvlhrhzf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gujzrhanr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/goiytlosz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gkutlhmky.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gmgakuetb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdmlshxzb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxwfbqact.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gbuqfebyk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/goanwaijm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjqaapbxi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/gkuldichd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gjnqokmla.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/goiukkkvh.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gnzywpwnh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gtlgeyibf.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/ggwpgvfzt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gyckswvjd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/giqjccklr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gvtjcvmah.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gmplqbuvm.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gqpydxbdc.sHtML


<!-- 参考信息 -->