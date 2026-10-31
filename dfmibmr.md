代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://rd.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://bj.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://ya.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://jo.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://lf.chemitech.net.cn

composer require psr/container
来源：http://vp.szsharing.cn

[U76] PHP：简单路由
来源：http://cw.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vb.huanxung.cn

[U77] PHP：模板渲染
来源：http://cc.bjjhwx.cn

composer require twig/twig
来源：http://ml.hahajie.cn

[U78] PHP：单元测试
来源：http://rl.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://sl.nicolike.cn

[U79] PHP：静态分析
来源：http://kb.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://wc.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://qe.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xd.yuexingan06.cn

[U81] JS：初始化项目
来源：http://ek.nszjky.cn

npm init -y;  npm i express
来源：http://la.szsharing.cn

[U82] JS：package.json 脚本
来源：http://zu.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sy.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://if.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lz.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://no.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ag.shtwfgs.cn

[U85] JS：可选链
来源：http://yu.huixiangedu.cn

a?.b?.c
来源：http://zw.hahajie.cn

[U86] JS：空值合并
来源：http://vc.nszjky.cn

a ?? b
来源：http://mw.huixiangedu.cn

[U87] JS：解构默认值
来源：http://mk.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://ph.newstarts.cn

[U88] JS：对象展开合并
来源：http://ie.bookmarksfly.cn

{ ...a, ...b }
来源：http://ox.huanxung.cn

[U89] JS：数组去重
来源：http://af.shxzskj.cn

[...new Set(arr)]
来源：http://mh.newstarts.cn

[U90] JS：数字数组排序
来源：http://hg.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://va.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://yk.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ac.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://dj.gzmigu.cn

structuredClone(obj)
来源：http://ym.panjiajie.cn

[U93] JS：模板字符串
来源：http://tf.shxzukj.cn

`共 ${n} 条`
来源：http://vd.bjjhwx.cn

[U94] JS：箭头函数
来源：http://yq.chemitech.net.cn

const double = x => x * 2;
来源：http://vc.nicolike.cn

[U95] JS：Promise 包装
来源：http://sq.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://vd.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://lx.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dr.haigaiapp.cn

[U97] JS：并发请求
来源：http://rl.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bp.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://ow.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ew.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://pj.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://st.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://kc.jctech888.com.cn

document.querySelector(".item")
来源：http://qw.muxihuayi.cn

[U101] JS：classList 操作
来源：http://wf.panjiajie.cn

el.classList.toggle("active")
来源：http://eb.muxihuayi.cn

[U102] JS：本地存储
来源：http://ld.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qb.gzmigu.cn

[U103] JS：定时器
来源：http://rm.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pa.jianghongdianzi.cn

[U104] JS：防抖
来源：http://sz.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ce.jianghongdianzi.cn

[U105] JS：节流
来源：http://es.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kr.newstarts.cn

[U106] JS：日期格式化
来源：http://qv.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nr.yuexingan06.cn

[U107] JS：数字千分位
来源：http://jn.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zd.shxzukj.cn

[U108] JS：随机整数
来源：http://zz.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vs.wgjwhj.cn

[U109] JS：数组分组
来源：http://gc.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://pe.nszjky.cn

[U110] JS：数组分块
来源：http://go.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ou.hahajie.cn

[U111] JS：对象转 Map
来源：http://lg.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://wq.muxihuayi.cn

[U112] JS：字符串补位
来源：http://jx.huanxung.cn

"7".padStart(3, "0")
来源：http://yl.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://ro.hnjuh.cn

s.replaceAll("a", "b")
来源：http://fq.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://rc.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kh.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://uo.jianghongdianzi.cn

crypto.randomUUID()
来源：http://rw.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://mk.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://wm.lnxyls.cn

[U117] JS：单元测试
来源：http://mn.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://oa.shtwfgs.cn

[U118] JS：开发服务器
来源：http://my.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://qp.lnxyls.cn

[U119] JS：生产构建
来源：http://wz.gzmigu.cn

npx vite build
来源：http://cx.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://xx.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://tc.shxzskj.cn

================================================================================
来源：http://hb.nszjky.cn

统计汇总
来源：http://dh.bookmarksfly.cn

================================================================================
来源：http://bb.yuexingan06.cn

按语言统计（条）：
来源：http://uy.hnjuh.cn

Python ......... 252
来源：http://kr.nszjky.cn

PHP ............ 252
来源：http://kt.huanxung.cn

JavaScript ..... 252
来源：http://tt.yuexingan06.cn

TypeScript ..... 212
来源：http://lt.haigaiapp.cn

Java ........... 212
来源：http://qp.wgjwhj.cn

Go ............. 212
来源：http://gc.shxzskj.cn

Ruby ........... 212
来源：http://fp.shtwfgs.cn

C# ............. 212
来源：http://li.panjiajie.cn

C .............. 30
来源：http://it.yuexingan06.cn

C++ ............ 30
来源：http://ax.wgjwhj.cn

SQL ............ 90
来源：http://wy.huanxung.cn

Bash ........... 80
来源：http://fy.nszjky.cn

Kotlin ......... 15
来源：http://jm.huanxung.cn

Swift .......... 15
来源：http://zs.colortex.cn

Lua ............ 10
来源：http://fj.jctech888.com.cn

Perl ........... 10
来源：http://fl.shxzukj.cn

Scala .......... 10
来源：http://rg.nszjky.cn

------------------------------------
来源：http://kg.jctech888.com.cn

合计 ........... 2106 条
来源：http://qj.szsharing.cn

按章节统计：
来源：http://rm.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ml.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ww.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://em.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hh.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cu.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mh.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qp.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wi.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ps.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://td.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hn.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zl.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pk.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nq.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ui.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hd.shtwfgs.cn

Q SQL 专题                              90
来源：http://qf.wgjwhj.cn

R Bash 专题                             80
来源：http://pc.colortex.cn

S C / C++ 专题                          60
来源：http://ss.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://qi.huanxung.cn

U 高频实用片段                         120
来源：http://rx.colortex.cn

------------------------------------
来源：http://sw.haigaiapp.cn

合计                                  2106 条
来源：http://tv.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://fx.bookmarksfly.cn

使用提醒
来源：http://od.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://aj.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pg.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vr.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uh.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kn.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mu.jctech888.com.cn

—— 文件结束 ——
来源：http://op.asd995.cn

================================================================================
来源：http://sj.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://ya.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://so.asd995.cn

================================================================================
来源：http://id.muxihuayi.cn

【收录内容】
来源：http://oq.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xo.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eb.huixiangedu.cn

SQL · Bash · C · C++
来源：http://zw.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cp.huixiangedu.cn

【使用说明】
来源：http://eo.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jq.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jx.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ha.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jh.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ha.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ns.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fa.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sg.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ej.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sy.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xq.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fh.colortex.cn

【文件统计】
来源：http://bx.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ur.hahajie.cn

--------------------------------------------------------------------------------
来源：http://yv.yuntaijiaju.cn

目  录
来源：http://ps.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://oz.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mt.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gj.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ge.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dc.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pg.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yt.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ti.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jc.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jy.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lg.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fn.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vj.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xr.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ce.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tl.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ni.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pm.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mv.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bb.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rn.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gp.jctech888.com.cn

================================================================================
来源：http://kw.shxzukj.cn

A. 基础语法与类型
来源：http://uw.yuexingan06.cn

================================================================================
来源：http://ve.huanxung.cn

[A01] Hello World
来源：http://rh.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ns.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://ew.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://qq.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hh.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://da.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://pl.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://wi.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://go.shxzskj.cn

[A02] 变量声明与赋值
来源：http://mu.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xf.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xt.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ek.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jf.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://ir.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://ib.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://nl.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nl.jctech888.com.cn

[A03] 常量定义
来源：http://ag.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hx.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://da.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://zc.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://wy.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://km.panjiajie.cn

Go:   const PI = 3.14159
来源：http://fj.shxzskj.cn

Ruby: PI = 3.14159
来源：http://ja.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://dl.bookmarksfly.cn

[A04] 判断变量类型
来源：http://ui.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wa.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cj.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ts.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://ah.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kg.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wb.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ex.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://pm.huanxung.cn

[A05] 整数除法与取模
来源：http://sp.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rt.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ro.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xm.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jy.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://lc.521024.cn

Go:   7 / 2; 7 % 2
来源：http://xe.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://mh.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://uj.huanxung.cn

[A06] 字符串转数字
来源：http://kx.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://ih.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://il.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eq.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sj.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://st.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bs.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hw.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tz.panjiajie.cn

[A07] 数字转字符串
来源：http://er.nszjky.cn

Py:   str(42)
来源：http://ci.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://bu.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://xt.wgjwhj.cn

TS:   String(42)
来源：http://gv.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bx.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://zr.nszjky.cn

Ruby: 42.to_s
来源：http://my.lnxyls.cn

C#:   42.ToString()
来源：http://xo.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://br.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gv.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kh.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vq.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bz.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gv.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rx.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ga.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gn.521024.cn

[A09] 绝对值与最大最小值
来源：http://ib.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ru.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ou.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nv.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jv.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mo.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pr.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kv.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dq.asd995.cn

[A10] 生成随机数
来源：http://lh.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://tq.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://ht.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kj.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mt.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://yl.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ng.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://fs.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://sg.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://ld.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ct.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fh.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ls.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pe.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://qb.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fd.huanxung.cn


<!-- 参考信息 -->