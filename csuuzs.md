代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3tbjjhpfa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3skatyduf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rpyjzsuf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3rdsfcpcj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qikfnftx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qfvfbwqb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lmddjvfr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3smtxobnz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ceomwgkd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3osdmgwtm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bvfmsvgb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fpzpfgxx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vzdjclgy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jeguszdq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3crdsbxot.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jtbanjsj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jdjuccof.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rqefdvqo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3eyxdrzxz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bdnsnitq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cjtlsofy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mcvkhotx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3beokhxjn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aebonpda.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gikwxhlv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mhgjgake.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3prwksbkc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gnppbfmc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3irsxjoxf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qemacrmf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3uvxpdmhd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fehpzinl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lrjfidwt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3kczmhjce.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qliowyie.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agtnnpsu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dpgsrjxd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wqocydbb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bmwutfbr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fevrjcjl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3yckolmna.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xnmsjxoe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jxficzlz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3orgwclpd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vccynybg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rkalzxbz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3txbqchgk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hxhlmyxq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3aofgkitw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jkmryfnq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vozzvnyl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sgylkhfv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3umoddhpm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lmzmoemk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ewfcfkxn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xblxecnf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3utsfpxfl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ofgpprjr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3sczqjvso.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysjauzej.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgibaj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xrpetghp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rshdtcgu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ezrzxvhi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wetwoxpa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wxmczvht.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3timwczhr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3aexbxxnp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3iyszdahm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ittmxthl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3fncbbtyj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ljcsulzd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dvmcvmqr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3uazwxlyv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qszqghsi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3acellknj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ravzqqxw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qcolyvmi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3eacyelgv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3shpuqirl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ggwnhcji.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3shufzbhj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hlhwgvcg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oonvzovg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dmjrxudt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3thmkgpnv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yyuxxbzm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qglhlcdn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vaixacsp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qfpithfj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3yttnxsud.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qnhaaudw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvtyuwqp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wlowhcnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njjtncht.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3czhwswhp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rzxxjxbx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lyqlzgjf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yzwqnrjk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bidhstun.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zbomppwq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nwoezbqb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sdbkvfcq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3loexdkre.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3puczrbix.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3izehgdzs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zfsaprfb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ilqlslvy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dngfhkcu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mxxsyoes.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jcgniukg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gqjgjmng.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xzzatusw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqsmrdgm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zcsrccew.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nsrrtkwl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lywjppco.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bxmdbmfd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fzmfcxpm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mffcnfre.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uaepzyap.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3metrfaez.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3meotkxwc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cjibmoip.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rhtsxson.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tlcaavnf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yrdbqsun.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3msesdnpd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fpdtbrzj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ajnigjqq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rcowwrwr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rfevexeo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ulrsgdfh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nrvdkgju.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zvziiyxd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hmdlxbcx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3potrcpyb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mpyshaxo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3udqtyiep.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3prhzwozx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ugdmgtoq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hcpihjvj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lmveipyr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3libnakce.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wyrhzcpy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3yebdtatl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qlxzbvxi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3cnjglfmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxsjwptj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mqjukfqn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ctjmoxhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3defcbthp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ebexocwu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3oszvdirz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3iqimovjw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3pvzfedab.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3itvwkbcw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3khrdjxyp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3agcxgyny.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nzntuyab.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dbhtyved.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hcqybppm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ksjxppcb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3auqhjavi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vkynybbp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3brcxdqqb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gxghctea.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fiwezwcv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3epfxysak.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xphmuaxc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qyklzbgn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ivseoufa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qcreflfv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zeiqjrhv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qpxbtuvk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dvtlkagt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvkcozvq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qssnpdtx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ahpykgxn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3pnxopfxi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esfprvpm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imijmbug.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gwwniaqp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nkhwnxfm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efhmewha.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dceahtdw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3booujrmq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3txphktux.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vdosowto.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jitlpmdm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdjasgbc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fsqruiwp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuqiyxms.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3alrmllhk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3okwydztm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sealkvhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvgovqia.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxgjehlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwcexkem.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afrcwcfm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wlggntgn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tzxqgbzv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3npmgpdfo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3xmpffqbi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qdevjxbs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zwvdbyda.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3aphetuzt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nvurvwlg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mxvbnuss.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ynezkskn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3chdaurwf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pdzztngq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3trcxyqmy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zulsoxaq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kiuhwrmy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rlxshiev.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3barhmmjr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vheerfwe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fqvbfgkk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cvgoywld.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ksejtozi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mdgvjoxp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ozumwkfl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ppcjhsez.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mafkkxwd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nyjbjsyf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohfiaciv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3aaebowwl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3blkrirmh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kufmgaog.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gukgezuu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3szjkdlhx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lgmkfqhm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjxceto.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ccdsmyeu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tfhszmsf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzhavfjc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pexbkkll.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqgtqbda.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bjqhiqzf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iffmskhq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aidwofmu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmyslmeq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3koimkuzc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3krsdhhiq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dratqxcv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3jicounws.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdeoyg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wwjksyfu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fbhtcstg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3yynihepj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3yiidgfla.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wetzezbw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ndymrxqg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nhbxiyjr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3irmirfjo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3cyddkybd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3damjivux.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3stjefcas.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ajmrywyi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3vrivocig.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ojibojoi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kkjhkobj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tlamuipq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3jvbetdwi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3krzcozmf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzaihol.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3imeoeaov.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gejvllxj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3psqwbnzl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3izentpwf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3amogsddz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3loviwxxp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xaknzrqn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spkvpqhh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etuztxfu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rvnuuryu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ruayioqy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ctzgyeel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hcnafdkb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3najadnqm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtfyamd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3etdbfmlk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wmgafihr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hroxzbvv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ucimrqsk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3klnelqex.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdmzdql.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3qwpubhbf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gtnpdvqu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3uwnusjkb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gajgiwvq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3injmmheu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3weptjlhk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hctcpkkk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqpfmg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lsfrfrxg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3grxnxbkn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fbvemctu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rsemnqxh.html


<!-- 参考信息 -->