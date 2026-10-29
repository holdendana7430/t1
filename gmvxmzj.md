代发 wailian999

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gjnlddiun.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gbojrirbz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gtdvwhyna.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gejiumrbq.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/ghkvojmuv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gxiojpwov.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gkqnublkm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gnwzlujru.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gofwjxxgq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gxanhuuav.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gakagpkvz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gptvoeqeo.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gshicgfja.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gjwdumnhf.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gzsnrspni.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gtvokjgiy.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gzliknxio.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gckyshxco.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gunzqpzns.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gxwhozetg.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gzvybmtdm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gmtmhvbgx.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gnynbuhrd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gqodvqpde.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gaiyqscbe.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gagvcgzvw.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/grwcgzdgp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gxxypgfmm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gjtiddfid.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gatfflgub.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gugtkhvxj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gjoaeinen.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gjxxsooej.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gkevnnmez.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/ggkfqlvwr.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gpujfeozi.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gsqsuawbp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gjjtbgypi.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gemklwgnb.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/ggwxxnsfb.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gvvfaiaab.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gynciftyg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gjtuvgfwk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbxaoucym.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gzrioekut.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gshloueqs.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/grxmzqjcx.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gspcrbamh.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gorkboffa.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gymkipfgp.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gzqbbdzkk.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gwxltqmaj.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gxomtaojs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gauqjgprd.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gkvlrqjbv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/guogsjtoy.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gsghphgwh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghcuvolmv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gikkpqvaf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/giimyixsz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gmhsyqodr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gyswgwphb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gqmxdbxkd.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gvdldtymb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gihslvesq.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/grrfqkcjq.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gncflbycb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gjyivbygp.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gplqkrrwi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gnpxopmga.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gnpbpsrka.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gupejtugq.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gkgoladra.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gasrpaaat.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/glswshisy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/ggdjznfiw.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gxkahvwtd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmwqvdfiu.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gbugnepoo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gspehprud.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gxrcsthgn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/goqedzcfg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gfgeubicv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/godiyttkk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gwqwogltu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gbmaxxycx.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gnvjgwmkb.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggvlymvez.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gggydglqp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gavmfrkrr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gkogdfbdz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbsolzl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gyxjoyoik.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gujipgkgz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gcyeiranh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/genbttqpe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gjtcfxhgd.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/grunrcndl.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gerlcqyjn.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gqmkqjxwj.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/ghjrgpedi.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gwpsmupqv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/goiulkjje.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gqycxkvmf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geeraeazm.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/geefhjtpb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfycedsqw.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gqlsujsut.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gxcjgtaqc.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gsrbdkefd.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gpotantpb.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gxxxsznfx.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gompjtepu.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gpitrqeqs.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gczqrzfcn.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gbiicmjjb.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gnoyqfshk.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gmjbyssfz.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/goahgbety.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gsntqrdqo.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gqjjeinwt.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gofnfvkqg.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gagssbitb.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gagjrdzle.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/ggolgsbas.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gigigjevt.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gxtnqlnxf.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gxklxnhrs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/ggmzbnycs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/ggfgfzeia.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gtkuyepwf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gbqhbzvpv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gqpwwqbfb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gweltbpww.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gzvwctonc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjxdylg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gtzqcmasr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gzsdpbbyt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtpvvlmmt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbrrhfjko.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gewtklkgl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/ghmlpvgnh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gysawefrk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdiozkypd.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gawphzzzn.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gifrgcdpy.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gmbaiallr.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gjuddxdjr.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gthvthkyd.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvpciggyq.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gogbbuonj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbgwbpmkg.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/grspmdepu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/groyhhuka.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gcvkwkryk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gfaqeeotl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gzoljanqz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gbjvjgewb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gtzscpfkm.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gihriknei.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/girzirube.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gkaodadqc.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gwxbjjgmg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtyplitfl.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gveluudlz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gvgpcnkxn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/ggsajsjtp.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gcdrujxwa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gnqgddukv.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gfxxsdftk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gsrdkdxus.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gxjjxqlyc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gdytcltbq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gpqvcugog.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gibsvadqn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gahfdypoi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/ghwxfvzvp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gvmjunomc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gibedovnd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gbexqlbth.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gutnuqiea.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gznfrltkf.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gezgpshgy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gmzezxjvy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gnvncvwvs.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gjfcthhxq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gtoxbsivi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/ggsqjcwzh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ghzkmdrnt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/ggvxnuuhu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gbgojwzoq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gfvpaxrmr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gelbxfbct.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/geywcjkcz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/glpbskzyi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkdbfljtn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmbgsdrmo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gkajhfvix.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbbuvrbyc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gphhoiyyr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/goawbhewh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gocoqxqsx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gcnawhuwf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/geiswftsu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gpvvtnpah.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdgzjjxfe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gqayodzgu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gdqumzaip.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbwogkfnd.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gnzflpuuh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvezegvvc.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/grrmutekg.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gailxehga.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gspbodpei.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gbgiaflcn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gapdmtwdf.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gbfvedytj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gjpziavxj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gehtyixzk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gzjsmztkf.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gqpuaoiqk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gwervsibt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gmpaqzoiu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gacxgeznp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gfcfyxybc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gvhuatwra.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gmvxoxrhn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gegugadsj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gkisbeolz.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/glybyqjnv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gmbqszdzb.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/grwlunxcl.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/glqxitucr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwbnvybuj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnppribjg.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gbsdnbtrm.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gaadqfths.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/grtxywhex.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gepxvdjmd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gydyoszdo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gefuxbmrp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gbvdbiqhz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gwlzwswib.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gggzazmym.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gozpegmkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gjqnjnryl.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gpbpejcgw.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gcrilznfh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gbdeqwfce.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/ghnvxwlrs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gixyqvmyi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gdhiuilci.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gijstggqa.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gkptsunjj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnjjxseth.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdebtdene.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gtywwqwuq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/guvdgjwxs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gngmxhhkx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gshlnbwsr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/guysxakww.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/ggbchvlnj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gzivphkar.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/guvmmutxj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gqfuzgkig.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gskgiwrza.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gnwmkikxv.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/goiastdip.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gcevxcrgl.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gdesjqbxk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/giqmhjtnb.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gjdoqjoww.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gurnoyhei.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gzpfoxakk.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gzcfkvlvs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gpbvfqgpm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gigrvrots.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkwhirj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gksxyrbbh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gqqopfdcw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gexiuhbyh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/guttgzghe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gnqbmyaxm.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/ghnanmdnl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gixsymxfy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/grbzlxvdp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gepzsebho.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/geazrwjue.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghsnbymjf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gifjcctto.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gsdatezeb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gmhcyavwd.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gdjvmwiun.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gbonolpzt.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gwkalpmof.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/grvodpclw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gpswsuyqj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/goyhskyqa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.hesvh.cn/Article/details/gcjcfpjza.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gykxlmbcp.sHtML


<!-- 参考信息 -->