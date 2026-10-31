代发 wailian999

[U79] PHP：静态分析
来源：http://pb.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://yd.hahajie.cn

[U80] PHP：代码规范修复
来源：http://il.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mg.huanxung.cn

[U81] JS：初始化项目
来源：http://gw.gzmigu.cn

npm init -y;  npm i express
来源：http://ga.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://ih.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ht.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://yc.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ni.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://ix.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gx.colortex.cn

[U85] JS：可选链
来源：http://lh.huixiangedu.cn

a?.b?.c
来源：http://rj.hnjuh.cn

[U86] JS：空值合并
来源：http://xd.newstarts.cn

a ?? b
来源：http://zj.hnjuh.cn

[U87] JS：解构默认值
来源：http://iz.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://yw.hnjuh.cn

[U88] JS：对象展开合并
来源：http://uz.521024.cn

{ ...a, ...b }
来源：http://xq.9csxet.cn

[U89] JS：数组去重
来源：http://nv.9csxet.cn

[...new Set(arr)]
来源：http://jc.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://kp.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://kk.asd995.cn

[U91] JS：对象键值遍历
来源：http://xs.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pn.9csxet.cn

[U92] JS：深拷贝
来源：http://gv.hahajie.cn

structuredClone(obj)
来源：http://fz.huixiangedu.cn

[U93] JS：模板字符串
来源：http://ka.nszjky.cn

`共 ${n} 条`
来源：http://iy.yuexingan06.cn

[U94] JS：箭头函数
来源：http://ns.asd995.cn

const double = x => x * 2;
来源：http://ak.hnjuh.cn

[U95] JS：Promise 包装
来源：http://sk.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://ym.newstarts.cn

[U96] JS：async/await 与异常
来源：http://no.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tm.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://ly.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rc.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://lr.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bk.lnxyls.cn

[U99] JS：事件监听
来源：http://ov.9csxet.cn

el.addEventListener("click", e => {})
来源：http://rg.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://hx.nszjky.cn

document.querySelector(".item")
来源：http://bs.bjjhwx.cn

[U101] JS：classList 操作
来源：http://nj.panjiajie.cn

el.classList.toggle("active")
来源：http://pt.shxzskj.cn

[U102] JS：本地存储
来源：http://ek.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yp.jianghongdianzi.cn

[U103] JS：定时器
来源：http://kp.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uk.9csxet.cn

[U104] JS：防抖
来源：http://om.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ce.hnjuh.cn

[U105] JS：节流
来源：http://kf.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://of.nszjky.cn

[U106] JS：日期格式化
来源：http://gd.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://la.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://qk.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fj.szxytkj.cn

[U108] JS：随机整数
来源：http://jl.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pi.lnxyls.cn

[U109] JS：数组分组
来源：http://xr.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://yd.521024.cn

[U110] JS：数组分块
来源：http://gs.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://el.9csxet.cn

[U111] JS：对象转 Map
来源：http://lr.shxzukj.cn

new Map(Object.entries(obj))
来源：http://wi.szxytkj.cn

[U112] JS：字符串补位
来源：http://zz.panjiajie.cn

"7".padStart(3, "0")
来源：http://ui.shxzskj.cn

[U113] JS：正则替换全部
来源：http://nx.nicolike.cn

s.replaceAll("a", "b")
来源：http://dh.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://tp.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tc.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://dp.panjiajie.cn

crypto.randomUUID()
来源：http://bf.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://jt.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://yb.hnjuh.cn

[U117] JS：单元测试
来源：http://iq.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://lh.wgjwhj.cn

[U118] JS：开发服务器
来源：http://vw.hnjuh.cn

npm i -D vite;  npx vite
来源：http://ry.muxihuayi.cn

[U119] JS：生产构建
来源：http://vz.huixiangedu.cn

npx vite build
来源：http://sk.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://td.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://gv.muxihuayi.cn

================================================================================
来源：http://lr.hnjuh.cn

统计汇总
来源：http://ki.chemitech.net.cn

================================================================================
来源：http://gr.huixinmuqiang.cn

按语言统计（条）：
来源：http://tm.huixinmuqiang.cn

Python ......... 252
来源：http://wf.colortex.cn

PHP ............ 252
来源：http://ff.muxihuayi.cn

JavaScript ..... 252
来源：http://ba.szxytkj.cn

TypeScript ..... 212
来源：http://dq.huixiangedu.cn

Java ........... 212
来源：http://de.yuexingan06.cn

Go ............. 212
来源：http://lo.asd995.cn

Ruby ........... 212
来源：http://ci.asd995.cn

C# ............. 212
来源：http://is.9csxet.cn

C .............. 30
来源：http://qp.huixinmuqiang.cn

C++ ............ 30
来源：http://om.szsharing.cn

SQL ............ 90
来源：http://xg.nszjky.cn

Bash ........... 80
来源：http://ci.hahajie.cn

Kotlin ......... 15
来源：http://dw.nszjky.cn

Swift .......... 15
来源：http://nx.szsharing.cn

Lua ............ 10
来源：http://cd.wgjwhj.cn

Perl ........... 10
来源：http://st.shtwfgs.cn

Scala .......... 10
来源：http://rl.hahajie.cn

------------------------------------
来源：http://yp.shxzskj.cn

合计 ........... 2106 条
来源：http://rp.nicolike.cn

按章节统计：
来源：http://jz.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kp.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wx.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sc.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dx.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lx.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tw.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cm.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sl.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ex.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ri.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eo.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ox.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fc.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lo.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xj.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jz.muxihuayi.cn

Q SQL 专题                              90
来源：http://ds.huixiangedu.cn

R Bash 专题                             80
来源：http://dx.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://zu.huanxung.cn

T 其他语言补充                          60
来源：http://jb.nicolike.cn

U 高频实用片段                         120
来源：http://yw.bookmarksfly.cn

------------------------------------
来源：http://rq.szsharing.cn

合计                                  2106 条
来源：http://sp.521024.cn

--------------------------------------------------------------------------------
来源：http://hb.asd995.cn

使用提醒
来源：http://kk.9csxet.cn

--------------------------------------------------------------------------------
来源：http://tc.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ef.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ym.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://um.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bb.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://le.asd995.cn

—— 文件结束 ——
来源：http://cb.jianghongdianzi.cn

================================================================================
来源：http://og.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://ls.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://az.jianghongdianzi.cn

================================================================================
来源：http://yt.gzmigu.cn

【收录内容】
来源：http://lk.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zk.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pl.shxzukj.cn

SQL · Bash · C · C++
来源：http://jh.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eb.colortex.cn

【使用说明】
来源：http://hk.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yi.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ge.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jo.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gf.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dx.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nj.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xu.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ya.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gs.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kf.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eq.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oj.9csxet.cn

【文件统计】
来源：http://wi.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gx.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ff.huixinmuqiang.cn

目  录
来源：http://yx.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://it.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lq.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eu.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bx.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tm.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pz.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://az.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rq.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://di.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zi.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://or.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dp.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fc.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xk.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nl.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vq.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fv.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bl.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wd.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://el.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oy.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ns.huixinmuqiang.cn

================================================================================
来源：http://dg.panjiajie.cn

A. 基础语法与类型
来源：http://hy.hnjuh.cn

================================================================================
来源：http://fg.yuexingan06.cn

[A01] Hello World
来源：http://xl.9csxet.cn

Py:   print("Hello, World!")
来源：http://gc.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://iq.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://jd.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yk.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://yq.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://bt.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://bq.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ri.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://cd.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dl.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xg.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nu.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vp.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://ll.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://ut.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://jo.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ml.colortex.cn

[A03] 常量定义
来源：http://gv.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tc.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://oj.szsharing.cn

JS:   const PI = 3.14159;
来源：http://rv.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://nz.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://wg.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://ap.colortex.cn

Ruby: PI = 3.14159
来源：http://am.colortex.cn

C#:   const double PI = 3.14159;
来源：http://uq.hnjuh.cn

[A04] 判断变量类型
来源：http://ak.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nk.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zl.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://od.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://iw.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rz.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eb.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ap.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://gn.jctech888.com.cn

[A05] 整数除法与取模
来源：http://xr.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pr.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yj.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ac.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mf.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://ge.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://aw.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://ba.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://xl.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://cj.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://jp.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hj.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rj.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nr.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zr.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yh.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wl.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rf.szxytkj.cn

[A07] 数字转字符串
来源：http://tm.szsharing.cn

Py:   str(42)
来源：http://ip.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://jl.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://dz.yuexingan06.cn

TS:   String(42)
来源：http://xe.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fs.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://rq.9csxet.cn

Ruby: 42.to_s
来源：http://qs.nszjky.cn

C#:   42.ToString()
来源：http://fv.521024.cn

[A08] 取整与四舍五入
来源：http://rt.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ro.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ii.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ci.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kp.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zw.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rt.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tq.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zh.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://ai.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mh.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xc.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ks.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bk.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bh.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bl.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gh.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://to.hahajie.cn

[A10] 生成随机数
来源：http://mx.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ht.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://ad.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lx.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lm.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://cr.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xe.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://xp.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://hd.szsharing.cn

[A11] 条件表达式（三元）
来源：http://ew.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://dp.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wx.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gt.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pu.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://zb.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mh.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jb.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pz.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://nh.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ee.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zv.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://yd.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ec.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://bx.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sb.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://lt.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://uk.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ga.shxzskj.cn


<!-- 参考信息 -->