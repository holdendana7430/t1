代发 wailian999

[U79] PHP：静态分析
来源：http://as.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://sl.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://hs.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sr.muxihuayi.cn

[U81] JS：初始化项目
来源：http://th.huanxung.cn

npm init -y;  npm i express
来源：http://su.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://qk.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yy.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://xp.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qa.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://lv.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cz.lnxyls.cn

[U85] JS：可选链
来源：http://nn.521024.cn

a?.b?.c
来源：http://co.huanxung.cn

[U86] JS：空值合并
来源：http://zz.gzmigu.cn

a ?? b
来源：http://rj.yuexingan06.cn

[U87] JS：解构默认值
来源：http://ux.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://zt.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://cp.asd995.cn

{ ...a, ...b }
来源：http://ma.hnjuh.cn

[U89] JS：数组去重
来源：http://tu.huixinmuqiang.cn

[...new Set(arr)]
来源：http://wy.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://mn.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://rk.huanxung.cn

[U91] JS：对象键值遍历
来源：http://wb.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qi.muxihuayi.cn

[U92] JS：深拷贝
来源：http://pc.hnjuh.cn

structuredClone(obj)
来源：http://ad.szsharing.cn

[U93] JS：模板字符串
来源：http://lf.bookmarksfly.cn

`共 ${n} 条`
来源：http://hd.shxzskj.cn

[U94] JS：箭头函数
来源：http://hb.bookmarksfly.cn

const double = x => x * 2;
来源：http://eg.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://aw.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://vm.newstarts.cn

[U96] JS：async/await 与异常
来源：http://hl.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://om.shxzukj.cn

[U97] JS：并发请求
来源：http://bi.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wd.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://zq.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dd.haigaiapp.cn

[U99] JS：事件监听
来源：http://bd.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://xq.nszjky.cn

[U100] JS：DOM 查询
来源：http://lz.jianghongdianzi.cn

document.querySelector(".item")
来源：http://yj.panjiajie.cn

[U101] JS：classList 操作
来源：http://sp.szsharing.cn

el.classList.toggle("active")
来源：http://yt.chemitech.net.cn

[U102] JS：本地存储
来源：http://yt.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xk.9csxet.cn

[U103] JS：定时器
来源：http://iz.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hd.huanxung.cn

[U104] JS：防抖
来源：http://dk.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pd.hahajie.cn

[U105] JS：节流
来源：http://ty.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tq.9csxet.cn

[U106] JS：日期格式化
来源：http://ji.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hd.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://qq.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dx.panjiajie.cn

[U108] JS：随机整数
来源：http://bz.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wy.nszjky.cn

[U109] JS：数组分组
来源：http://rq.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ut.asd995.cn

[U110] JS：数组分块
来源：http://ha.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lk.hnjuh.cn

[U111] JS：对象转 Map
来源：http://ok.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://um.nicolike.cn

[U112] JS：字符串补位
来源：http://ac.wgjwhj.cn

"7".padStart(3, "0")
来源：http://xn.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://ra.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://uz.newstarts.cn

[U114] JS：JSON 深比较
来源：http://fo.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ix.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://rx.gzmigu.cn

crypto.randomUUID()
来源：http://xg.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://hx.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://vt.shtwfgs.cn

[U117] JS：单元测试
来源：http://su.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://bx.haigaiapp.cn

[U118] JS：开发服务器
来源：http://kq.lnxyls.cn

npm i -D vite;  npx vite
来源：http://jl.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://ek.521024.cn

npx vite build
来源：http://qs.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://nz.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://yb.lnxyls.cn

================================================================================
来源：http://jj.wgjwhj.cn

统计汇总
来源：http://pu.yuexingan06.cn

================================================================================
来源：http://rb.chemitech.net.cn

按语言统计（条）：
来源：http://lv.wgjwhj.cn

Python ......... 252
来源：http://no.yuexingan06.cn

PHP ............ 252
来源：http://iw.jianghongdianzi.cn

JavaScript ..... 252
来源：http://qz.9csxet.cn

TypeScript ..... 212
来源：http://te.hahajie.cn

Java ........... 212
来源：http://vu.shtwfgs.cn

Go ............. 212
来源：http://bb.huanxung.cn

Ruby ........... 212
来源：http://jm.hahajie.cn

C# ............. 212
来源：http://az.newstarts.cn

C .............. 30
来源：http://ux.huixinmuqiang.cn

C++ ............ 30
来源：http://tx.nicolike.cn

SQL ............ 90
来源：http://dw.jianghongdianzi.cn

Bash ........... 80
来源：http://fq.huixinmuqiang.cn

Kotlin ......... 15
来源：http://wo.shxzukj.cn

Swift .......... 15
来源：http://xv.hnjuh.cn

Lua ............ 10
来源：http://oo.newstarts.cn

Perl ........... 10
来源：http://as.yuexingan06.cn

Scala .......... 10
来源：http://tj.shtwfgs.cn

------------------------------------
来源：http://du.9csxet.cn

合计 ........... 2106 条
来源：http://wp.jianghongdianzi.cn

按章节统计：
来源：http://mj.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qa.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qk.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ns.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ro.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fk.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xo.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nm.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://co.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pp.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jp.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pg.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qf.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wn.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ut.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dy.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qv.huanxung.cn

Q SQL 专题                              90
来源：http://jv.nicolike.cn

R Bash 专题                             80
来源：http://tw.shtwfgs.cn

S C / C++ 专题                          60
来源：http://so.panjiajie.cn

T 其他语言补充                          60
来源：http://sg.jctech888.com.cn

U 高频实用片段                         120
来源：http://zi.shtwfgs.cn

------------------------------------
来源：http://go.shxzukj.cn

合计                                  2106 条
来源：http://bn.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://go.gzmigu.cn

使用提醒
来源：http://wk.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ls.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ln.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wx.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bi.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pz.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ed.szxytkj.cn

—— 文件结束 ——
来源：http://ds.jianghongdianzi.cn

================================================================================
来源：http://vr.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://ab.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://hw.szsharing.cn

================================================================================
来源：http://ec.bookmarksfly.cn

【收录内容】
来源：http://xr.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jn.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dn.colortex.cn

SQL · Bash · C · C++
来源：http://yt.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mf.9csxet.cn

【使用说明】
来源：http://ph.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hv.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jm.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ol.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ar.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ne.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ho.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bj.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yo.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zp.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qz.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://su.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qg.lnxyls.cn

【文件统计】
来源：http://hi.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://po.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ep.521024.cn

目  录
来源：http://rt.colortex.cn

--------------------------------------------------------------------------------
来源：http://bc.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ae.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zq.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sz.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://io.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://co.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nk.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://an.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vv.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bo.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vc.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aq.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://je.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ow.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xl.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://um.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://to.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xq.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iu.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uj.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ju.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ee.panjiajie.cn

================================================================================
来源：http://nh.huixinmuqiang.cn

A. 基础语法与类型
来源：http://yg.shxzukj.cn

================================================================================
来源：http://ud.colortex.cn

[A01] Hello World
来源：http://wu.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://af.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://rl.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://ha.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ef.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://fs.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://rg.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://kr.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://od.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://nj.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qb.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bb.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iy.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pr.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://xw.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://bu.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://gp.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dt.521024.cn

[A03] 常量定义
来源：http://dt.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://am.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://rt.hahajie.cn

JS:   const PI = 3.14159;
来源：http://ei.521024.cn

TS:   const PI: number = 3.14159;
来源：http://cq.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://by.nszjky.cn

Go:   const PI = 3.14159
来源：http://lv.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://qx.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://kw.hnjuh.cn

[A04] 判断变量类型
来源：http://qw.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://do.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lm.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tg.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://bf.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fz.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hm.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yu.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://xy.asd995.cn

[A05] 整数除法与取模
来源：http://sm.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bc.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zi.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ma.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yp.521024.cn

Java: 7 / 2; 7 % 2
来源：http://yf.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://bg.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://sa.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://tm.hahajie.cn

[A06] 字符串转数字
来源：http://pb.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://xh.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hv.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kk.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ah.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pc.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ml.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dg.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ex.newstarts.cn

[A07] 数字转字符串
来源：http://tn.shtwfgs.cn

Py:   str(42)
来源：http://sz.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://wz.hahajie.cn

JS:   String(42); (42).toString()
来源：http://fg.szxytkj.cn

TS:   String(42)
来源：http://mr.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bg.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://as.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://bx.gzmigu.cn

C#:   42.ToString()
来源：http://tz.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://bo.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aw.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lc.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fc.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qt.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tq.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cb.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yk.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gp.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://fl.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://he.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://je.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sy.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dl.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zv.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bl.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oq.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gi.shxzskj.cn

[A10] 生成随机数
来源：http://iq.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://uw.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://mg.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kd.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wa.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://pn.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ev.wgjwhj.cn

Ruby: rand(1..100)
来源：http://zz.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://al.newstarts.cn

[A11] 条件表达式（三元）
来源：http://eg.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://xj.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cz.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://we.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ry.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://qf.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jh.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ox.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ly.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://wd.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zx.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sr.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://rp.521024.cn

TS:   `Hello, ${name}!`
来源：http://cz.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://sh.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nh.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://wd.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://je.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dm.wgjwhj.cn


<!-- 参考信息 -->