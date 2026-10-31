代发 wailian999

[U79] PHP：静态分析
来源：http://be.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://bc.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://eo.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wg.szsharing.cn

[U81] JS：初始化项目
来源：http://rs.newstarts.cn

npm init -y;  npm i express
来源：http://le.521024.cn

[U82] JS：package.json 脚本
来源：http://uy.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cc.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://qm.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://av.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ca.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pl.shxzukj.cn

[U85] JS：可选链
来源：http://cg.hnjuh.cn

a?.b?.c
来源：http://yd.newstarts.cn

[U86] JS：空值合并
来源：http://lh.gzmigu.cn

a ?? b
来源：http://tb.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://ms.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://gt.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://dh.hnjuh.cn

{ ...a, ...b }
来源：http://fe.jctech888.com.cn

[U89] JS：数组去重
来源：http://rd.9csxet.cn

[...new Set(arr)]
来源：http://bk.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://vl.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ag.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://uz.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pg.gzmigu.cn

[U92] JS：深拷贝
来源：http://ex.colortex.cn

structuredClone(obj)
来源：http://ot.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://cd.haigaiapp.cn

`共 ${n} 条`
来源：http://is.panjiajie.cn

[U94] JS：箭头函数
来源：http://ze.nicolike.cn

const double = x => x * 2;
来源：http://ru.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://jv.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://du.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://yp.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://us.lnxyls.cn

[U97] JS：并发请求
来源：http://hu.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pm.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://wz.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qy.521024.cn

[U99] JS：事件监听
来源：http://mz.hahajie.cn

el.addEventListener("click", e => {})
来源：http://vd.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://gl.hahajie.cn

document.querySelector(".item")
来源：http://uv.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://te.bookmarksfly.cn

el.classList.toggle("active")
来源：http://oy.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://yo.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qm.asd995.cn

[U103] JS：定时器
来源：http://pg.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mj.szsharing.cn

[U104] JS：防抖
来源：http://wy.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ak.shxzskj.cn

[U105] JS：节流
来源：http://xk.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vh.muxihuayi.cn

[U106] JS：日期格式化
来源：http://eg.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bn.szsharing.cn

[U107] JS：数字千分位
来源：http://al.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mb.newstarts.cn

[U108] JS：随机整数
来源：http://up.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ki.nszjky.cn

[U109] JS：数组分组
来源：http://gt.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://dh.panjiajie.cn

[U110] JS：数组分块
来源：http://cp.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ef.szsharing.cn

[U111] JS：对象转 Map
来源：http://gp.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://fv.shxzukj.cn

[U112] JS：字符串补位
来源：http://sd.panjiajie.cn

"7".padStart(3, "0")
来源：http://gw.szxytkj.cn

[U113] JS：正则替换全部
来源：http://dm.nicolike.cn

s.replaceAll("a", "b")
来源：http://jt.nszjky.cn

[U114] JS：JSON 深比较
来源：http://ms.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rs.panjiajie.cn

[U115] JS：生成 UUID
来源：http://cb.shxzukj.cn

crypto.randomUUID()
来源：http://ux.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://jj.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://sh.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://qx.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://vs.chemitech.net.cn

[U118] JS：开发服务器
来源：http://uh.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://hk.521024.cn

[U119] JS：生产构建
来源：http://tn.9csxet.cn

npx vite build
来源：http://bu.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://sb.521024.cn

import.meta.env.VITE_API_URL
来源：http://kn.shxzskj.cn

================================================================================
来源：http://tr.chemitech.net.cn

统计汇总
来源：http://gq.gzmigu.cn

================================================================================
来源：http://cc.jctech888.com.cn

按语言统计（条）：
来源：http://jl.9csxet.cn

Python ......... 252
来源：http://of.panjiajie.cn

PHP ............ 252
来源：http://ps.jctech888.com.cn

JavaScript ..... 252
来源：http://hg.bookmarksfly.cn

TypeScript ..... 212
来源：http://kw.szxytkj.cn

Java ........... 212
来源：http://aw.lnxyls.cn

Go ............. 212
来源：http://bn.nszjky.cn

Ruby ........... 212
来源：http://fn.bookmarksfly.cn

C# ............. 212
来源：http://io.asd995.cn

C .............. 30
来源：http://ki.jctech888.com.cn

C++ ............ 30
来源：http://fv.nicolike.cn

SQL ............ 90
来源：http://gt.nicolike.cn

Bash ........... 80
来源：http://ns.asd995.cn

Kotlin ......... 15
来源：http://cq.jctech888.com.cn

Swift .......... 15
来源：http://ue.gzmigu.cn

Lua ............ 10
来源：http://hr.szsharing.cn

Perl ........... 10
来源：http://kr.9csxet.cn

Scala .......... 10
来源：http://ub.shxzukj.cn

------------------------------------
来源：http://au.muxihuayi.cn

合计 ........... 2106 条
来源：http://bb.shxzukj.cn

按章节统计：
来源：http://jj.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pd.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ue.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zq.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rl.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yx.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hn.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ye.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pe.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pu.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qu.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yh.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lx.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ol.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jk.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zw.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dx.bjjhwx.cn

Q SQL 专题                              90
来源：http://jz.haigaiapp.cn

R Bash 专题                             80
来源：http://ji.jctech888.com.cn

S C / C++ 专题                          60
来源：http://kc.muxihuayi.cn

T 其他语言补充                          60
来源：http://sc.huanxung.cn

U 高频实用片段                         120
来源：http://hv.shxzskj.cn

------------------------------------
来源：http://rg.9csxet.cn

合计                                  2106 条
来源：http://lp.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://wk.huanxung.cn

使用提醒
来源：http://iy.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://tx.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bi.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wk.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mw.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://of.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gd.shtwfgs.cn

—— 文件结束 ——
来源：http://tq.haigaiapp.cn

================================================================================
来源：http://so.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://bh.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://sy.asd995.cn

================================================================================
来源：http://nj.bookmarksfly.cn

【收录内容】
来源：http://tb.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dm.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bj.shtwfgs.cn

SQL · Bash · C · C++
来源：http://xm.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://je.shxzskj.cn

【使用说明】
来源：http://re.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ee.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lt.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yu.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nw.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lt.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rc.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kn.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iv.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dh.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://og.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://si.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dm.hahajie.cn

【文件统计】
来源：http://sq.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sg.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://sq.gzmigu.cn

目  录
来源：http://we.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://px.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iu.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cc.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zq.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jr.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://om.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tb.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wx.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gi.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dy.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oo.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tg.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ts.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jd.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hm.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uw.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oz.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://us.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gm.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sv.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hv.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ar.haigaiapp.cn

================================================================================
来源：http://zz.szsharing.cn

A. 基础语法与类型
来源：http://id.muxihuayi.cn

================================================================================
来源：http://xs.muxihuayi.cn

[A01] Hello World
来源：http://os.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://yo.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://yy.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://fi.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mb.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://rv.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ry.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://mb.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fy.szxytkj.cn

[A02] 变量声明与赋值
来源：http://il.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xc.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yr.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zu.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ey.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://gw.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://bg.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://xt.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ez.shtwfgs.cn

[A03] 常量定义
来源：http://kb.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ny.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://bd.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://xu.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://bl.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://xa.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://cy.521024.cn

Ruby: PI = 3.14159
来源：http://sg.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://pt.szxytkj.cn

[A04] 判断变量类型
来源：http://mq.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ws.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zx.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vp.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://un.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ru.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lc.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yd.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://tn.szxytkj.cn

[A05] 整数除法与取模
来源：http://ib.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ui.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ko.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://el.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eh.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://bv.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://ug.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://gp.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://uy.lnxyls.cn

[A06] 字符串转数字
来源：http://qp.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://xu.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ta.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sf.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kx.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kl.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qx.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hn.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xm.shxzukj.cn

[A07] 数字转字符串
来源：http://sk.9csxet.cn

Py:   str(42)
来源：http://da.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://rj.colortex.cn

JS:   String(42); (42).toString()
来源：http://en.bookmarksfly.cn

TS:   String(42)
来源：http://zn.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ff.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://xq.colortex.cn

Ruby: 42.to_s
来源：http://jp.panjiajie.cn

C#:   42.ToString()
来源：http://jc.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://dx.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gi.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yj.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iw.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yp.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://re.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ja.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mk.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ta.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://jj.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ro.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oe.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gf.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kl.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rp.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://al.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fl.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nl.shxzskj.cn

[A10] 生成随机数
来源：http://ro.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://ch.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://xd.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eq.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mq.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ho.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cq.shxzskj.cn

Ruby: rand(1..100)
来源：http://xo.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://cw.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://aw.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ee.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://as.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dq.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ze.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://mt.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://io.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mv.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ma.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://cv.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hn.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vh.asd995.cn

JS:   `Hello, ${name}!`
来源：http://iw.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://wm.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://nf.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ko.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ly.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://zw.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://og.shxzskj.cn


<!-- 参考信息 -->