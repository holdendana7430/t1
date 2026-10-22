代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pdujrtfo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aqufuvxz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dbszoznc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wpdjesji.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2icrqabve.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2heirfoqa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdhhhmhs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2bnuajcyz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2oedbqwbr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fifaohhf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gxwhvlyo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dmsphfyl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bireuvpv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fquygxgu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ebivjtwo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vtjbaous.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zqnzfnzv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bdrjgjyn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tddvuosf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gsddzxfx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dkvggbqb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lhqscmce.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2pawqvuax.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bnraebwj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fmvypdzf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tliobhzz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rkvryfbo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2naifmrtn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mehwkypu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2dawvyags.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2hhokiqjb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2chlpormo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2udmbehbn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bhineziy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ozohvewj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fesubcgc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwpxyu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hcdbojty.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fzasesut.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ddcnqkzg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2inbfrlli.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lqvxkdue.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hsttrjhf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2heqvaunp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2quooakvi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kaqgwxcj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tdoakoaf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fuetjccb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vsghggvn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nziuincp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ofveinlz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cbjrbbue.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2houxtljv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2llmcuyii.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jbsuyrqo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kftrkayg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2druekzoh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pfgejvod.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2onthtvze.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mgulzuxw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sdloirqc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tvqzjxya.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gyvbvtyt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gjjyrffq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hatdyvpz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2elcftpam.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2arztwqes.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tycoknvw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kjlgdsnk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2syichvxb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cmyttgeq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ofebylux.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ltdsfiga.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wwrgefaa.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2shcjeokg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2rmqftptb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ruvgicsc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xgntiocb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jxscfuom.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2krvdogmm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jliksger.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nzvpckjg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2jmcfwovj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yirvlffl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zfetqiyy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yovshkvx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jfdqjttz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2spukvtwp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rqwwhjdm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rnfkdhse.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rdhetkqw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxfzuq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2waxnusxr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2iplbtzas.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2yzgkwajn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qjkvkdtk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yxotuzgi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vxrcciju.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wlyfkjki.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2daamrerw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhuvyejs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mgrnuaal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkjpmmws.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fdqawzlr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hslklbcx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2resfetlt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vtuuaebv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qrejyovk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wxdvljli.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nbwebtqf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ruxkgrqq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vwlkycnw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ltqcfajq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pjnsaymz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2apulzlec.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gmszfykx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jnuojkxh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gpsjisqh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2oajiubdi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bjfetjst.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nwwqnkiz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2movrycfy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rrgwaejx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qdqzijbs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fnsoauew.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jnlelgiy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nzhqqiix.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dsludbkx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ukrfoudj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2txscqawd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2itphxtfl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2autjjjrf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jjhjgjfl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qnreroxu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pfusiqas.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2alwxunwl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ltgpzeuv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2leyndtnm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jdswivqp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tnolmjuo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vofuepvp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ijiwvxad.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wqswnwpt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uwswznfo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cebismkf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tqnfrueo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2dfmwojqd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vsnvecxg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2yzmpnwkw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uczygnnx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2bvvubnvw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fbuichfk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2wsbiyjdi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zfuylxih.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2htfnzqbg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vjtbvvlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtkfmahi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2gqmfalfw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tygjsdyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjckgrto.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xaeihcnf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pboaalff.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zrksaifh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2faatzuew.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2watozobd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ghbknsen.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2luxbmaii.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ojixvuyk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pmqeqvve.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qzcihzii.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hghufnsy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2nrmoemfu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xjuhtyzy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2txkdtocn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2uixhoulo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ehjrqyor.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2vmjsyygt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ogxqagsr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qfckfrjv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2lncvbibr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hjqqdhvw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rvsrpdlo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ldxbuamn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnjilvim.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rkredlzk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fybyveky.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dmkzrwwa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgpqugcc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hiddblzy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qbgqwyno.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2smhjtoit.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gynjowkf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ijymjjsw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kssttqhi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sopznjum.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2utzjoqaf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2whqrtjgz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cnnfvtax.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwqqclco.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2nuzzuyhp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvtwnarl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2brobronk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ulmdvbdc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlacfhah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phyecnor.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2spltpenj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqpnuikq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dmhoqerh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ickducpt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2olohxjjs.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pweiffvq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dbabwzbk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hzjpzbsg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vjgtnjff.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ebqbhhia.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vojzynzg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hvkouqpg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gxrdndmx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2txrmwhfm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ojkzipyb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tzjcytwh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mqnvtsar.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2uqibjbbs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2sinyujmt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hskusqos.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hloozdzc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2rmqmjgsa.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2elanhesz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tsvfctai.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hcujspeq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cgusjtae.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yudxshsv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cdxfpbqk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rkdwwdeq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bwadkrzw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2tohhiltx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcoejmi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yetuxive.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vvjbomyn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vatrtmdv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2kimmasuc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2mypzpcvt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pfnmufvj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2monxuylh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbuxnkcz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pjxkvgfz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hnflftuk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rgbnppic.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vbsvausw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xyzucsvh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mxcvqbxd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uybouync.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pcfmwfmw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ncketxzq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cndukens.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2stnbexts.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2yqvhdunh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hgwcwvud.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtxapob.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vuaoupuk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wnvubdmw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2kxkrbedv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2iwjuxbul.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdimrqq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kkwupazy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ascnijes.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bltygnfv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2czuqnjxb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2mzfmnajn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2shbenzrc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wctkhpdu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzjbiuo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nqwvmdtc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qfiilkbo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hnaukbva.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rogmuoqi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pqasenld.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2fhatfrxv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ptttklpv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vehkafyo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sqchnjnn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2saikplsb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfqchxe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mgvvkaxc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2agpujmsa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vvepvmdt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kesniecv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwuwsers.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mastgwef.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2khiskofd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jpvsezyh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ngndofxy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wahkcuiv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhkqzupk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2heosgmqf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrkvmqu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2guzqchaq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2oojhdsnd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mrzchbha.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jnzpcrgl.html


<!-- 参考信息 -->