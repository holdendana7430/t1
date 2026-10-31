代发 wailian999

[U77] PHP：模板渲染
来源：http://px.bookmarksfly.cn

composer require twig/twig
来源：http://am.szsharing.cn

[U78] PHP：单元测试
来源：http://gi.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://kz.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://iu.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ee.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://nt.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rj.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://fi.chemitech.net.cn

npm init -y;  npm i express
来源：http://rz.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://wa.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ng.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://wx.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xm.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://pm.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ea.colortex.cn

[U85] JS：可选链
来源：http://ho.shtwfgs.cn

a?.b?.c
来源：http://bz.muxihuayi.cn

[U86] JS：空值合并
来源：http://cp.muxihuayi.cn

a ?? b
来源：http://rl.colortex.cn

[U87] JS：解构默认值
来源：http://fm.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://rt.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://nz.huanxung.cn

{ ...a, ...b }
来源：http://tl.gzmigu.cn

[U89] JS：数组去重
来源：http://vs.bjjhwx.cn

[...new Set(arr)]
来源：http://xp.shxzukj.cn

[U90] JS：数字数组排序
来源：http://vg.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://wd.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://kf.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kz.shxzskj.cn

[U92] JS：深拷贝
来源：http://dl.shxzukj.cn

structuredClone(obj)
来源：http://pu.huanxung.cn

[U93] JS：模板字符串
来源：http://rx.chemitech.net.cn

`共 ${n} 条`
来源：http://bk.panjiajie.cn

[U94] JS：箭头函数
来源：http://ft.szxytkj.cn

const double = x => x * 2;
来源：http://rd.521024.cn

[U95] JS：Promise 包装
来源：http://vz.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://nb.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://gy.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rh.bookmarksfly.cn

[U97] JS：并发请求
来源：http://so.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jh.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://er.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ix.hahajie.cn

[U99] JS：事件监听
来源：http://dg.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://bx.szxytkj.cn

[U100] JS：DOM 查询
来源：http://jl.shxzskj.cn

document.querySelector(".item")
来源：http://tc.9csxet.cn

[U101] JS：classList 操作
来源：http://us.szxytkj.cn

el.classList.toggle("active")
来源：http://yn.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://by.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kg.lnxyls.cn

[U103] JS：定时器
来源：http://oo.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gu.jctech888.com.cn

[U104] JS：防抖
来源：http://oe.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ij.yuntaijiaju.cn

[U105] JS：节流
来源：http://vz.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oq.colortex.cn

[U106] JS：日期格式化
来源：http://sr.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hy.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://ol.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xl.huanxung.cn

[U108] JS：随机整数
来源：http://wi.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kf.haigaiapp.cn

[U109] JS：数组分组
来源：http://vw.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://cf.yuexingan06.cn

[U110] JS：数组分块
来源：http://hi.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cm.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://yi.lnxyls.cn

new Map(Object.entries(obj))
来源：http://qt.chemitech.net.cn

[U112] JS：字符串补位
来源：http://yl.bjjhwx.cn

"7".padStart(3, "0")
来源：http://ts.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://mq.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://vo.9csxet.cn

[U114] JS：JSON 深比较
来源：http://kw.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yo.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://mk.chemitech.net.cn

crypto.randomUUID()
来源：http://xt.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://gm.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://gs.panjiajie.cn

[U117] JS：单元测试
来源：http://xp.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://wr.muxihuayi.cn

[U118] JS：开发服务器
来源：http://xi.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://bq.wgjwhj.cn

[U119] JS：生产构建
来源：http://ae.haigaiapp.cn

npx vite build
来源：http://bj.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://le.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://yg.521024.cn

================================================================================
来源：http://vr.muxihuayi.cn

统计汇总
来源：http://gy.yuntaijiaju.cn

================================================================================
来源：http://us.muxihuayi.cn

按语言统计（条）：
来源：http://yu.gzmigu.cn

Python ......... 252
来源：http://uy.jctech888.com.cn

PHP ............ 252
来源：http://fy.yuexingan06.cn

JavaScript ..... 252
来源：http://rq.shxzskj.cn

TypeScript ..... 212
来源：http://ab.nszjky.cn

Java ........... 212
来源：http://dq.jctech888.com.cn

Go ............. 212
来源：http://nk.jctech888.com.cn

Ruby ........... 212
来源：http://lb.asd995.cn

C# ............. 212
来源：http://ha.bjjhwx.cn

C .............. 30
来源：http://fh.jianghongdianzi.cn

C++ ............ 30
来源：http://rb.huixinmuqiang.cn

SQL ............ 90
来源：http://nm.jctech888.com.cn

Bash ........... 80
来源：http://re.szsharing.cn

Kotlin ......... 15
来源：http://kx.asd995.cn

Swift .......... 15
来源：http://yy.521024.cn

Lua ............ 10
来源：http://ht.yuexingan06.cn

Perl ........... 10
来源：http://td.asd995.cn

Scala .......... 10
来源：http://hg.szsharing.cn

------------------------------------
来源：http://ea.521024.cn

合计 ........... 2106 条
来源：http://bk.muxihuayi.cn

按章节统计：
来源：http://ap.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ms.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oq.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oz.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ys.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hf.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vg.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lh.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yi.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fq.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ja.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wk.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tb.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sh.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yq.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tt.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ox.asd995.cn

Q SQL 专题                              90
来源：http://as.shtwfgs.cn

R Bash 专题                             80
来源：http://mv.shxzskj.cn

S C / C++ 专题                          60
来源：http://qc.bjjhwx.cn

T 其他语言补充                          60
来源：http://ad.muxihuayi.cn

U 高频实用片段                         120
来源：http://iz.szxytkj.cn

------------------------------------
来源：http://yb.nicolike.cn

合计                                  2106 条
来源：http://kd.hahajie.cn

--------------------------------------------------------------------------------
来源：http://mq.nicolike.cn

使用提醒
来源：http://xe.nicolike.cn

--------------------------------------------------------------------------------
来源：http://iw.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nv.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hi.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bh.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nt.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pu.hahajie.cn

—— 文件结束 ——
来源：http://yr.lnxyls.cn

================================================================================
来源：http://dx.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://ba.nszjky.cn

Common Programming Examples Cheat Book
来源：http://km.jianghongdianzi.cn

================================================================================
来源：http://kq.huixinmuqiang.cn

【收录内容】
来源：http://ny.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mc.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tk.bjjhwx.cn

SQL · Bash · C · C++
来源：http://le.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://al.asd995.cn

【使用说明】
来源：http://pd.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bc.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yh.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lz.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fi.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ne.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yk.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bd.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cq.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://he.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rt.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nf.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mn.521024.cn

【文件统计】
来源：http://mf.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kx.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://fn.gzmigu.cn

目  录
来源：http://lk.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mx.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zr.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ne.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tz.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kd.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kg.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qa.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xp.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vx.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://st.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tn.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://da.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xc.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rn.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://km.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rj.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://np.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uq.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zh.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ne.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rz.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cx.szxytkj.cn

================================================================================
来源：http://yb.colortex.cn

A. 基础语法与类型
来源：http://hd.hahajie.cn

================================================================================
来源：http://se.wgjwhj.cn

[A01] Hello World
来源：http://vy.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ji.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://kg.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://nb.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yw.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://tp.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://od.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://il.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sh.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://qx.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uk.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ld.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tz.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oj.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://eo.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://su.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://ze.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ws.haigaiapp.cn

[A03] 常量定义
来源：http://gq.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vw.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://cu.hahajie.cn

JS:   const PI = 3.14159;
来源：http://vr.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://dc.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://rx.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://ev.asd995.cn

Ruby: PI = 3.14159
来源：http://md.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://eu.bookmarksfly.cn

[A04] 判断变量类型
来源：http://xl.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kx.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nm.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vj.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://na.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ld.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mk.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cg.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://fp.nszjky.cn

[A05] 整数除法与取模
来源：http://wc.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rl.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lk.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tp.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hv.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://tt.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://sy.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://tx.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://gg.bjjhwx.cn

[A06] 字符串转数字
来源：http://ry.colortex.cn

Py:   int("42"); float("3.14")
来源：http://ms.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ul.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yi.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yt.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rk.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nc.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bw.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vx.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://qr.wgjwhj.cn

Py:   str(42)
来源：http://mt.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://mq.hahajie.cn

JS:   String(42); (42).toString()
来源：http://gs.szsharing.cn

TS:   String(42)
来源：http://bj.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://im.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://nr.shxzskj.cn

Ruby: 42.to_s
来源：http://ak.colortex.cn

C#:   42.ToString()
来源：http://fl.9csxet.cn

[A08] 取整与四舍五入
来源：http://tp.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kn.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rf.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gr.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qt.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ox.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sc.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mq.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qn.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://on.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lj.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sz.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ix.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xx.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wl.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kf.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iz.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qc.panjiajie.cn

[A10] 生成随机数
来源：http://ji.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://su.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://ox.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cj.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eg.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://ak.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jo.521024.cn

Ruby: rand(1..100)
来源：http://pw.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://vn.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://cx.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://pb.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ds.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qf.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kr.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://cz.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://we.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hd.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://io.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://fu.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ph.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://be.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://hm.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://od.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://az.9csxet.cn


<!-- 参考信息 -->