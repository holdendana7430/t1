代发 wailian999

[U79] PHP：静态分析
来源：http://xj.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://kk.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://nk.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nw.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://qn.huanxung.cn

npm init -y;  npm i express
来源：http://ty.521024.cn

[U82] JS：package.json 脚本
来源：http://ny.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gx.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://fq.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://io.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://ry.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eb.panjiajie.cn

[U85] JS：可选链
来源：http://nw.szxytkj.cn

a?.b?.c
来源：http://ev.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://lf.jianghongdianzi.cn

a ?? b
来源：http://yu.huanxung.cn

[U87] JS：解构默认值
来源：http://wp.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ej.szxytkj.cn

[U88] JS：对象展开合并
来源：http://qc.bookmarksfly.cn

{ ...a, ...b }
来源：http://nt.wgjwhj.cn

[U89] JS：数组去重
来源：http://to.huanxung.cn

[...new Set(arr)]
来源：http://ot.nszjky.cn

[U90] JS：数字数组排序
来源：http://hg.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://yk.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://vq.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sr.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://ai.bookmarksfly.cn

structuredClone(obj)
来源：http://vf.nszjky.cn

[U93] JS：模板字符串
来源：http://ac.nicolike.cn

`共 ${n} 条`
来源：http://fe.lnxyls.cn

[U94] JS：箭头函数
来源：http://jz.huixinmuqiang.cn

const double = x => x * 2;
来源：http://pe.shxzukj.cn

[U95] JS：Promise 包装
来源：http://sm.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://tu.9csxet.cn

[U96] JS：async/await 与异常
来源：http://hw.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gk.gzmigu.cn

[U97] JS：并发请求
来源：http://cm.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yq.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://dh.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zs.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://sn.asd995.cn

el.addEventListener("click", e => {})
来源：http://ki.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://sk.asd995.cn

document.querySelector(".item")
来源：http://uw.panjiajie.cn

[U101] JS：classList 操作
来源：http://ly.gzmigu.cn

el.classList.toggle("active")
来源：http://bc.huanxung.cn

[U102] JS：本地存储
来源：http://sh.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://en.szsharing.cn

[U103] JS：定时器
来源：http://vg.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zv.gzmigu.cn

[U104] JS：防抖
来源：http://xw.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ye.panjiajie.cn

[U105] JS：节流
来源：http://lz.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eq.hnjuh.cn

[U106] JS：日期格式化
来源：http://kt.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xv.muxihuayi.cn

[U107] JS：数字千分位
来源：http://zs.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ha.szxytkj.cn

[U108] JS：随机整数
来源：http://qe.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://en.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://km.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://jd.wgjwhj.cn

[U110] JS：数组分块
来源：http://sz.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xt.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://by.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://wq.jctech888.com.cn

[U112] JS：字符串补位
来源：http://az.lnxyls.cn

"7".padStart(3, "0")
来源：http://aw.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://er.colortex.cn

s.replaceAll("a", "b")
来源：http://kg.nicolike.cn

[U114] JS：JSON 深比较
来源：http://hy.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cc.nszjky.cn

[U115] JS：生成 UUID
来源：http://rs.521024.cn

crypto.randomUUID()
来源：http://hy.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://el.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://oz.szxytkj.cn

[U117] JS：单元测试
来源：http://mx.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://ye.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://oj.newstarts.cn

npm i -D vite;  npx vite
来源：http://gi.bookmarksfly.cn

[U119] JS：生产构建
来源：http://op.hahajie.cn

npx vite build
来源：http://pj.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://sp.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://pd.jctech888.com.cn

================================================================================
来源：http://wp.jianghongdianzi.cn

统计汇总
来源：http://rq.newstarts.cn

================================================================================
来源：http://cs.gzmigu.cn

按语言统计（条）：
来源：http://qn.hahajie.cn

Python ......... 252
来源：http://cd.yuexingan06.cn

PHP ............ 252
来源：http://lu.haigaiapp.cn

JavaScript ..... 252
来源：http://yy.huixiangedu.cn

TypeScript ..... 212
来源：http://sr.szsharing.cn

Java ........... 212
来源：http://mu.521024.cn

Go ............. 212
来源：http://hq.panjiajie.cn

Ruby ........... 212
来源：http://et.521024.cn

C# ............. 212
来源：http://xw.asd995.cn

C .............. 30
来源：http://hz.yuexingan06.cn

C++ ............ 30
来源：http://hb.521024.cn

SQL ............ 90
来源：http://xm.panjiajie.cn

Bash ........... 80
来源：http://wv.chemitech.net.cn

Kotlin ......... 15
来源：http://wv.gzmigu.cn

Swift .......... 15
来源：http://nh.szsharing.cn

Lua ............ 10
来源：http://jn.chemitech.net.cn

Perl ........... 10
来源：http://lv.bjjhwx.cn

Scala .......... 10
来源：http://bk.bjjhwx.cn

------------------------------------
来源：http://cs.hnjuh.cn

合计 ........... 2106 条
来源：http://ex.panjiajie.cn

按章节统计：
来源：http://ia.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://un.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qu.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hf.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sd.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://za.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zw.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vh.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bg.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://so.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jw.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nj.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vo.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xf.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hr.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cd.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://so.shxzskj.cn

Q SQL 专题                              90
来源：http://kf.gzmigu.cn

R Bash 专题                             80
来源：http://cy.szsharing.cn

S C / C++ 专题                          60
来源：http://gi.colortex.cn

T 其他语言补充                          60
来源：http://ia.shxzskj.cn

U 高频实用片段                         120
来源：http://ma.yuntaijiaju.cn

------------------------------------
来源：http://hg.szsharing.cn

合计                                  2106 条
来源：http://ol.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://pg.hnjuh.cn

使用提醒
来源：http://vj.nicolike.cn

--------------------------------------------------------------------------------
来源：http://tj.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hw.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://if.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ac.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ru.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bo.bookmarksfly.cn

—— 文件结束 ——
来源：http://sx.lnxyls.cn

================================================================================
来源：http://hv.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://li.szsharing.cn

Common Programming Examples Cheat Book
来源：http://uc.hnjuh.cn

================================================================================
来源：http://mr.lnxyls.cn

【收录内容】
来源：http://vw.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://re.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hb.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://hz.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oq.nszjky.cn

【使用说明】
来源：http://wd.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gc.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iy.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xz.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fe.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zs.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bp.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pj.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bg.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ru.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yw.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ps.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://id.haigaiapp.cn

【文件统计】
来源：http://nq.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ry.nicolike.cn

--------------------------------------------------------------------------------
来源：http://kx.lnxyls.cn

目  录
来源：http://wm.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://de.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tq.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ty.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cx.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bv.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yx.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ck.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://au.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kq.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rr.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gl.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bc.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nu.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rg.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gx.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://es.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fb.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bg.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nc.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mu.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://iw.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jn.nicolike.cn

================================================================================
来源：http://zl.huanxung.cn

A. 基础语法与类型
来源：http://ey.jianghongdianzi.cn

================================================================================
来源：http://ix.yuexingan06.cn

[A01] Hello World
来源：http://vf.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://pp.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://ke.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://yz.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vs.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://dg.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://wq.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://no.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zx.hnjuh.cn

[A02] 变量声明与赋值
来源：http://hm.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fg.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ol.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cv.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pu.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://le.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://cn.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://pf.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tf.chemitech.net.cn

[A03] 常量定义
来源：http://fz.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yp.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://vb.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ld.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://fz.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://vy.nicolike.cn

Go:   const PI = 3.14159
来源：http://du.nszjky.cn

Ruby: PI = 3.14159
来源：http://pq.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://gm.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://uy.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hw.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gg.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xp.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://xb.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gb.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ms.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sl.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://pw.asd995.cn

[A05] 整数除法与取模
来源：http://dn.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xc.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xo.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://al.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://os.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://mb.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://bf.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://yx.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://nr.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://mg.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://rk.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cq.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dh.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tm.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hx.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fd.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qv.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lk.jctech888.com.cn

[A07] 数字转字符串
来源：http://cy.bookmarksfly.cn

Py:   str(42)
来源：http://ax.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://aa.huanxung.cn

JS:   String(42); (42).toString()
来源：http://gf.chemitech.net.cn

TS:   String(42)
来源：http://zk.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ny.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://em.nicolike.cn

Ruby: 42.to_s
来源：http://rj.lnxyls.cn

C#:   42.ToString()
来源：http://he.hnjuh.cn

[A08] 取整与四舍五入
来源：http://ym.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kh.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wy.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vn.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kk.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jp.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bd.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pt.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vs.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://tt.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://na.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sm.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cf.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wf.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qm.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ko.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wh.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vj.shxzukj.cn

[A10] 生成随机数
来源：http://tf.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://xq.nszjky.cn

PHP:  random_int(1, 100);
来源：http://lj.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mn.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dr.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://rk.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cz.szxytkj.cn

Ruby: rand(1..100)
来源：http://xl.521024.cn

C#:   new Random().Next(1, 101)
来源：http://kw.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://ul.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://gb.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jy.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vg.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kl.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://zu.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vq.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hp.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yo.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://sp.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zq.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wz.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://jv.521024.cn

TS:   `Hello, ${name}!`
来源：http://qf.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://yr.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tg.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://dw.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://ih.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yd.shtwfgs.cn


<!-- 参考信息 -->