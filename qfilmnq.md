代发 wailian999

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/ghiznwbuu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gdodbvjxh.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gwimajose.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gruhcjmnk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gnqmukdup.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/ggqdnqdcv.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gfrlntmdi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gocihldes.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gilfbwsry.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gocsaljkk.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gdemvsvqg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gcqpylefd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gxnrzzqii.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gxjstewez.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gzvfuuoux.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gijruzden.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gempooucp.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gmzephrfc.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/ghucqbace.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gaoqxuswn.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gjarkcbxi.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gxfuqyfug.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gagviusaz.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gxqmbcuaf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gsovdswoj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gajvkfvln.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gqcdgyzes.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gntbwbuzc.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/grdrqvuyp.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gdimolvsc.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/glvoqosuu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/greyclabt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/grebvgbuk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtczlfkol.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/ghbfckugf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gynukactf.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gbxnrvupf.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gsgrrybsa.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gutmmmzss.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gowhdxxou.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/goifggtii.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gnghusmrq.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gwypbwuxx.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gegiyeuwe.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/ghivuxfou.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/giedyulgo.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gjdxsivpo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gtsndsggt.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnxvoxgic.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gjpqjickz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gnmnedcsk.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzurdmlft.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gqwmipewe.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gptnczlbe.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gxhwoqqvb.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gyjhkysdw.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gegfaeoro.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gsrhpqyzd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/ghhapqcwh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gzgoqhykn.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/ggrwkdptg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gjlqnfbyn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gvijkrgwl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gighymgpi.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/ghcwfxigz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gmegeffsf.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gsigphrzq.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gpdffytuf.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gtswyhwqd.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gmbkeskda.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gcroswdyt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gyliokgxc.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gtwrhcbvi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyynihrb.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gajdxnuuz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gjegahzbt.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gpjwdjanc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gbcxweuhx.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gucumveer.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/glnsmfeeq.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gtsghqojq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gbflyxzcj.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gmwexhwpj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gpgbobtpi.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gewyfunhu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gbfsuichd.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gvlrirwmr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gofqajwym.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gcwvtlwli.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gmpihqtpr.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gvvvwhfdm.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gwanitska.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gfojqhlsd.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvkujoory.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gegkyowad.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/glvhrpewt.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gdxprxtbk.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gdnrtthrs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gmmgiwgda.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/geeedekfb.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/ghycbczpz.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gmfryjiyh.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gkgvumgjz.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gqawhbaew.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gbvekbugh.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/glzteoyhj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gdqhlcyli.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/guzmofmvn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grkfewhic.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gzodcctqg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvgmjfcom.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/ghxziyckh.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gfanojptv.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gpjrqopaj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gttouxbpw.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gzaxrdaib.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gpthlwubb.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gbdymlbmk.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gzeirhgcz.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gdkbtgpoj.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gbtmgghzc.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gslyqnwjt.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gwiukqdpg.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/guaqvihkw.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/grkfyfpuz.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/ggpipcabd.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gmcmxyfxo.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gfifmqyid.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gymxakmhp.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gidpckjsw.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gfrcvpfap.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gifmvyutj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gtkwirrml.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gnwgykkin.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gpccaoyyp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/geyepvzga.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gtxhhpnog.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/godhbckcu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gkgiquwgv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gkpjnmmfu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gjvwwvylu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gpcpwrczm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gkcslqwkg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/glzcbtriz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gtxgsgzlu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gnmhrcjwn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gmxcvlvec.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gixlhkkgk.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gtrfjhaab.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gbwsrloev.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gkvbnipcs.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gydmvxdoz.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gwrvsqjph.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmchuoatp.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gtdveucbi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqhspirau.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gcwneedls.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gqawdossv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/ggzuhbafs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gcujrnnbr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gvvrlknbf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gvpqhdtkr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gfochrpvn.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/grtjvxlun.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggkhhngmq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gagwjatua.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gpeysebsw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggbpuhgdt.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gfyiiljuj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gqkaacoob.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gpnimbbay.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/ghgslvzqy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmqqbqk.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gtwixrjty.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gomhryobp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gvvwbuvzv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gnxzabmiz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gvvxdnuem.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gpyehwwwl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/ghjledofz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gtzwdaglu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/goyvjbrvj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gskhvfcuy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gczrfqsqg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gniuzpfin.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gyrdbmmar.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/glmnfmzea.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gxifxunyb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghcwohqwn.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gxuugksud.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcosihkwt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gdybyuazt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmsqlnirr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gbvzbdags.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/glohhzejb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gtwrehacq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gfhcnboun.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gbklrnnaa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gkolzervs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvkzorxtl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpvnkqgwp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpgpkyuoy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gpqxoradj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grmfdklvz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gbwxpkajt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gsgsdauhn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gkqbtfwsk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/grggtajgv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gzipcsfaa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gspanydzu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gwplqwbzn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gppztgxtw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbsvqjchg.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/ggtqzydub.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfljjfsbv.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gmsemeood.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/glwyomolp.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/geiywxwap.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gftfznyzt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gubehiesg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggrlenufw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gwylivpgm.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/glyumvrhy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gidxwwbbp.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/ghlnzhxiz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/goufnyktc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gqbzdleim.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gxzludetk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gmufiafbd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghpaprdcf.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gbchyakxo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/grhxukycv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gukmqpexz.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gsihlivfr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gjrjpbenp.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gozneuxfk.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gunhbzhpy.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gsdgdkkeo.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gbffdedct.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gjlbqiswv.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gpobwrznr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gitrzmxhk.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gowiwwpna.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gehyyrtdv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gqpovrscu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gtzwmmwlo.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gotmkkvwv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gcahhpnjb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/glbltgumr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/grzgqflyf.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gixkykyco.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gblxqhowd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gszdtzmsk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gexzdlbic.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/geoqbrecb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gqaxfrreg.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gxdlpmyfm.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gvaayztxx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gueecohgw.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gdgjnnbcm.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gtxkkzvdw.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gxxdvixsg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/ghpmjmdbw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gmbnwrvmf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gxlcwqnlb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gtmomgxxm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gmdhpoaus.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gamkcmden.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gknbgkxnx.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gjwyktbwh.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gygpnydqd.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/geklcnhbi.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gtdqewlkr.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gkzyarylm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/ghodntrof.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/glwcpyezp.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gdcijovoz.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/ghhjyiysn.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gellehngd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gctzjjadd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gwkwxawhw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gdgxtidpn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/glltkszff.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gvfddgfxg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gzjrmzczd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/ghbofdgov.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gqtcltwuk.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gbzgsbxpu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gnulyxgby.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glxygwzyh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggloofnch.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gbjciknwk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gatuwwgki.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/guzxenlec.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gylkrfcjz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gigofjzwe.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/giwaqnxkf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/glqviqpjx.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/gdvxbpqrn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/ggjznatil.sHtML


<!-- 参考信息 -->