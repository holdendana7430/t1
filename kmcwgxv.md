代发 wailian999

[U75] PHP：依赖注入
来源：http://bn.newstarts.cn

composer require psr/container
来源：http://ux.colortex.cn

[U76] PHP：简单路由
来源：http://rt.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lg.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ip.bookmarksfly.cn

composer require twig/twig
来源：http://ja.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://po.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://cg.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://vp.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://fo.asd995.cn

[U80] PHP：代码规范修复
来源：http://rv.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wk.huixiangedu.cn

[U81] JS：初始化项目
来源：http://ww.wgjwhj.cn

npm init -y;  npm i express
来源：http://qv.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://cx.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ah.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://th.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rr.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://vh.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ga.panjiajie.cn

[U85] JS：可选链
来源：http://bh.yuexingan06.cn

a?.b?.c
来源：http://au.chemitech.net.cn

[U86] JS：空值合并
来源：http://xo.wgjwhj.cn

a ?? b
来源：http://at.huixiangedu.cn

[U87] JS：解构默认值
来源：http://ya.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://cy.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://ih.wgjwhj.cn

{ ...a, ...b }
来源：http://gq.shxzukj.cn

[U89] JS：数组去重
来源：http://pa.shxzskj.cn

[...new Set(arr)]
来源：http://mz.asd995.cn

[U90] JS：数字数组排序
来源：http://rf.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://pv.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://gf.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mq.newstarts.cn

[U92] JS：深拷贝
来源：http://ku.lnxyls.cn

structuredClone(obj)
来源：http://gr.muxihuayi.cn

[U93] JS：模板字符串
来源：http://ik.huanxung.cn

`共 ${n} 条`
来源：http://xj.newstarts.cn

[U94] JS：箭头函数
来源：http://xh.newstarts.cn

const double = x => x * 2;
来源：http://bv.521024.cn

[U95] JS：Promise 包装
来源：http://yp.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://sr.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://qi.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hn.gzmigu.cn

[U97] JS：并发请求
来源：http://uw.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hw.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://uc.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ll.9csxet.cn

[U99] JS：事件监听
来源：http://go.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://ml.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://gg.szxytkj.cn

document.querySelector(".item")
来源：http://sz.chemitech.net.cn

[U101] JS：classList 操作
来源：http://dt.muxihuayi.cn

el.classList.toggle("active")
来源：http://dr.szxytkj.cn

[U102] JS：本地存储
来源：http://tj.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ti.lnxyls.cn

[U103] JS：定时器
来源：http://ui.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hk.huanxung.cn

[U104] JS：防抖
来源：http://od.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uk.lnxyls.cn

[U105] JS：节流
来源：http://cj.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://og.muxihuayi.cn

[U106] JS：日期格式化
来源：http://ki.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oe.lnxyls.cn

[U107] JS：数字千分位
来源：http://mm.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xy.newstarts.cn

[U108] JS：随机整数
来源：http://gb.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gj.bookmarksfly.cn

[U109] JS：数组分组
来源：http://mg.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://mq.szxytkj.cn

[U110] JS：数组分块
来源：http://ta.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uy.asd995.cn

[U111] JS：对象转 Map
来源：http://ue.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://eq.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://fp.shtwfgs.cn

"7".padStart(3, "0")
来源：http://iy.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://yg.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://kk.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://ao.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nk.panjiajie.cn

[U115] JS：生成 UUID
来源：http://ry.huanxung.cn

crypto.randomUUID()
来源：http://tw.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ub.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://sd.szxytkj.cn

[U117] JS：单元测试
来源：http://zf.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://rw.hahajie.cn

[U118] JS：开发服务器
来源：http://sf.lnxyls.cn

npm i -D vite;  npx vite
来源：http://qk.lnxyls.cn

[U119] JS：生产构建
来源：http://vj.huixiangedu.cn

npx vite build
来源：http://le.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://pf.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://lf.shxzukj.cn

================================================================================
来源：http://ob.haigaiapp.cn

统计汇总
来源：http://yv.panjiajie.cn

================================================================================
来源：http://ap.yuexingan06.cn

按语言统计（条）：
来源：http://me.wgjwhj.cn

Python ......... 252
来源：http://al.nszjky.cn

PHP ............ 252
来源：http://fs.colortex.cn

JavaScript ..... 252
来源：http://qw.jctech888.com.cn

TypeScript ..... 212
来源：http://re.colortex.cn

Java ........... 212
来源：http://cb.bookmarksfly.cn

Go ............. 212
来源：http://ql.yuntaijiaju.cn

Ruby ........... 212
来源：http://qg.nicolike.cn

C# ............. 212
来源：http://kw.yuexingan06.cn

C .............. 30
来源：http://ld.hnjuh.cn

C++ ............ 30
来源：http://yz.yuexingan06.cn

SQL ............ 90
来源：http://yw.wgjwhj.cn

Bash ........... 80
来源：http://ae.panjiajie.cn

Kotlin ......... 15
来源：http://cx.huanxung.cn

Swift .......... 15
来源：http://ko.shxzskj.cn

Lua ............ 10
来源：http://eq.jctech888.com.cn

Perl ........... 10
来源：http://eg.muxihuayi.cn

Scala .......... 10
来源：http://il.colortex.cn

------------------------------------
来源：http://eh.521024.cn

合计 ........... 2106 条
来源：http://ll.jctech888.com.cn

按章节统计：
来源：http://sj.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zb.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pp.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qa.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eo.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ua.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://es.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nn.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zq.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vz.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ho.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://px.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zr.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kx.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zv.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dh.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://za.shxzskj.cn

Q SQL 专题                              90
来源：http://gf.haigaiapp.cn

R Bash 专题                             80
来源：http://dc.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://ft.haigaiapp.cn

T 其他语言补充                          60
来源：http://wq.szxytkj.cn

U 高频实用片段                         120
来源：http://xh.jctech888.com.cn

------------------------------------
来源：http://ub.nicolike.cn

合计                                  2106 条
来源：http://jl.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://zl.jianghongdianzi.cn

使用提醒
来源：http://ie.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://jj.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kg.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ox.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sb.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sn.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ev.szsharing.cn

—— 文件结束 ——
来源：http://gn.bookmarksfly.cn

================================================================================
来源：http://ce.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://tv.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://hv.asd995.cn

================================================================================
来源：http://jd.hnjuh.cn

【收录内容】
来源：http://hu.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jm.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ef.colortex.cn

SQL · Bash · C · C++
来源：http://oa.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yj.shtwfgs.cn

【使用说明】
来源：http://zw.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ot.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kx.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kz.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oz.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://un.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zl.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oj.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rn.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kw.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gj.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rw.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tp.huanxung.cn

【文件统计】
来源：http://zw.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://og.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://hr.shxzskj.cn

目  录
来源：http://wr.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ll.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uz.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uk.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fy.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jg.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ve.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gb.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ah.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kg.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ua.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ti.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fz.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ch.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mm.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bs.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ni.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wj.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ge.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tr.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rd.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xk.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rs.jctech888.com.cn

================================================================================
来源：http://py.jianghongdianzi.cn

A. 基础语法与类型
来源：http://eg.wgjwhj.cn

================================================================================
来源：http://nk.bookmarksfly.cn

[A01] Hello World
来源：http://jp.9csxet.cn

Py:   print("Hello, World!")
来源：http://em.521024.cn

PHP:  echo "Hello, World!";
来源：http://ed.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://ge.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tb.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://ol.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://qr.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://tu.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://er.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://pm.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xs.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xu.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sa.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pl.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://dw.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://nk.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://tb.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://py.chemitech.net.cn

[A03] 常量定义
来源：http://mg.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pb.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://zv.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://my.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://yc.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ul.gzmigu.cn

Go:   const PI = 3.14159
来源：http://uf.szxytkj.cn

Ruby: PI = 3.14159
来源：http://sz.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://ub.haigaiapp.cn

[A04] 判断变量类型
来源：http://yt.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dw.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tu.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ns.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://lz.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qz.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uf.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ey.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://ri.chemitech.net.cn

[A05] 整数除法与取模
来源：http://xs.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vz.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dl.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://om.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ij.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://fl.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://bq.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://oi.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://lf.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://ly.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://di.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oi.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hq.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rv.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://um.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fy.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://su.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aa.muxihuayi.cn

[A07] 数字转字符串
来源：http://oh.lnxyls.cn

Py:   str(42)
来源：http://jw.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://kx.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://fz.jctech888.com.cn

TS:   String(42)
来源：http://oc.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eb.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://bc.wgjwhj.cn

Ruby: 42.to_s
来源：http://gw.jctech888.com.cn

C#:   42.ToString()
来源：http://jw.nicolike.cn

[A08] 取整与四舍五入
来源：http://vk.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qw.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bc.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://es.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wo.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://on.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://va.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ue.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yq.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://dl.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yk.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cm.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rq.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kn.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vw.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://am.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vl.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yk.bookmarksfly.cn

[A10] 生成随机数
来源：http://cq.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://kj.nszjky.cn

PHP:  random_int(1, 100);
来源：http://am.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ao.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gj.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://xd.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://en.asd995.cn

Ruby: rand(1..100)
来源：http://fe.521024.cn

C#:   new Random().Next(1, 101)
来源：http://up.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://om.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://tf.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ct.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kr.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zv.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://hc.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sd.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rz.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xb.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://xu.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ed.nicolike.cn


<!-- 参考信息 -->