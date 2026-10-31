代发 wailian999

[U85] JS：可选链
来源：http://nn.bjjhwx.cn

a?.b?.c
来源：http://jf.shtwfgs.cn

[U86] JS：空值合并
来源：http://am.muxihuayi.cn

a ?? b
来源：http://vu.newstarts.cn

[U87] JS：解构默认值
来源：http://np.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://lc.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://iu.hnjuh.cn

{ ...a, ...b }
来源：http://ej.huanxung.cn

[U89] JS：数组去重
来源：http://fd.colortex.cn

[...new Set(arr)]
来源：http://kl.newstarts.cn

[U90] JS：数字数组排序
来源：http://by.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://pd.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://tn.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eh.shxzukj.cn

[U92] JS：深拷贝
来源：http://id.521024.cn

structuredClone(obj)
来源：http://dx.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://eu.szxytkj.cn

`共 ${n} 条`
来源：http://vt.shxzukj.cn

[U94] JS：箭头函数
来源：http://ij.wgjwhj.cn

const double = x => x * 2;
来源：http://zy.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://zt.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://zz.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://jp.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gs.nicolike.cn

[U97] JS：并发请求
来源：http://vf.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wz.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://dd.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hb.colortex.cn

[U99] JS：事件监听
来源：http://na.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://mt.huanxung.cn

[U100] JS：DOM 查询
来源：http://ij.szsharing.cn

document.querySelector(".item")
来源：http://sh.asd995.cn

[U101] JS：classList 操作
来源：http://vo.huanxung.cn

el.classList.toggle("active")
来源：http://yz.newstarts.cn

[U102] JS：本地存储
来源：http://pi.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://do.nszjky.cn

[U103] JS：定时器
来源：http://fz.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tq.gzmigu.cn

[U104] JS：防抖
来源：http://jc.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jv.bookmarksfly.cn

[U105] JS：节流
来源：http://np.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qk.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://be.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ps.9csxet.cn

[U107] JS：数字千分位
来源：http://ha.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eq.haigaiapp.cn

[U108] JS：随机整数
来源：http://gr.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cg.huanxung.cn

[U109] JS：数组分组
来源：http://hj.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ah.jctech888.com.cn

[U110] JS：数组分块
来源：http://zl.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://au.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://zg.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://oz.521024.cn

[U112] JS：字符串补位
来源：http://zt.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://wu.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://uq.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://aj.huanxung.cn

[U114] JS：JSON 深比较
来源：http://qd.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pg.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://qi.521024.cn

crypto.randomUUID()
来源：http://ir.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://qb.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://ov.szxytkj.cn

[U117] JS：单元测试
来源：http://ff.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://pt.newstarts.cn

[U118] JS：开发服务器
来源：http://tp.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://pk.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://pc.huanxung.cn

npx vite build
来源：http://si.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ig.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://ru.bjjhwx.cn

================================================================================
来源：http://af.haigaiapp.cn

统计汇总
来源：http://qm.haigaiapp.cn

================================================================================
来源：http://us.chemitech.net.cn

按语言统计（条）：
来源：http://hn.huanxung.cn

Python ......... 252
来源：http://ab.nszjky.cn

PHP ............ 252
来源：http://gu.chemitech.net.cn

JavaScript ..... 252
来源：http://hl.chemitech.net.cn

TypeScript ..... 212
来源：http://hd.huixiangedu.cn

Java ........... 212
来源：http://ud.bookmarksfly.cn

Go ............. 212
来源：http://gn.bookmarksfly.cn

Ruby ........... 212
来源：http://ls.shxzskj.cn

C# ............. 212
来源：http://eo.hahajie.cn

C .............. 30
来源：http://dd.521024.cn

C++ ............ 30
来源：http://ra.jianghongdianzi.cn

SQL ............ 90
来源：http://kj.nszjky.cn

Bash ........... 80
来源：http://xu.nszjky.cn

Kotlin ......... 15
来源：http://by.shxzukj.cn

Swift .......... 15
来源：http://fk.asd995.cn

Lua ............ 10
来源：http://vj.haigaiapp.cn

Perl ........... 10
来源：http://sm.haigaiapp.cn

Scala .......... 10
来源：http://lb.bjjhwx.cn

------------------------------------
来源：http://cz.lnxyls.cn

合计 ........... 2106 条
来源：http://hs.jianghongdianzi.cn

按章节统计：
来源：http://xg.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dp.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yv.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nd.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xe.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lt.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vq.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dd.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://il.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xy.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xw.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oc.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oe.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qt.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tl.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rq.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gk.9csxet.cn

Q SQL 专题                              90
来源：http://ln.gzmigu.cn

R Bash 专题                             80
来源：http://ad.panjiajie.cn

S C / C++ 专题                          60
来源：http://vx.hnjuh.cn

T 其他语言补充                          60
来源：http://xb.bjjhwx.cn

U 高频实用片段                         120
来源：http://qb.yuntaijiaju.cn

------------------------------------
来源：http://vd.haigaiapp.cn

合计                                  2106 条
来源：http://wy.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://md.gzmigu.cn

使用提醒
来源：http://bj.huanxung.cn

--------------------------------------------------------------------------------
来源：http://kl.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ey.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vz.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wf.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eg.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://io.yuexingan06.cn

—— 文件结束 ——
来源：http://dm.9csxet.cn

================================================================================
来源：http://kb.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://kt.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://di.9csxet.cn

================================================================================
来源：http://lv.asd995.cn

【收录内容】
来源：http://px.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jx.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nj.asd995.cn

SQL · Bash · C · C++
来源：http://tu.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xy.asd995.cn

【使用说明】
来源：http://nf.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wf.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://un.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oj.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lc.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sg.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://na.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mc.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lq.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sy.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qm.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sb.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dc.panjiajie.cn

【文件统计】
来源：http://ua.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pz.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://om.szsharing.cn

目  录
来源：http://ge.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://nk.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ol.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eq.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hj.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kj.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gw.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lv.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pe.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bp.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ju.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tp.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rc.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kx.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gy.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dx.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lv.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bb.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ln.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lr.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iv.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://av.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cn.newstarts.cn

================================================================================
来源：http://ke.shtwfgs.cn

A. 基础语法与类型
来源：http://lo.bjjhwx.cn

================================================================================
来源：http://bd.shxzskj.cn

[A01] Hello World
来源：http://do.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://vj.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://he.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://uc.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ca.521024.cn

Java: System.out.println("Hello, World!");
来源：http://po.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://dn.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://op.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wo.szxytkj.cn

[A02] 变量声明与赋值
来源：http://ov.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yi.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ef.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vk.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ts.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://gr.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://bh.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://ag.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ln.lnxyls.cn

[A03] 常量定义
来源：http://ec.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xy.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://nw.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://jx.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://mi.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://du.nszjky.cn

Go:   const PI = 3.14159
来源：http://fu.hnjuh.cn

Ruby: PI = 3.14159
来源：http://dr.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://ro.shtwfgs.cn

[A04] 判断变量类型
来源：http://fg.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cd.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wq.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dr.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://cv.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cv.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iz.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uw.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://eo.bjjhwx.cn

[A05] 整数除法与取模
来源：http://zp.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yw.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vy.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wo.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ii.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://pi.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://kt.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://ez.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://fy.jctech888.com.cn

[A06] 字符串转数字
来源：http://sd.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://uw.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ut.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fs.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wn.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qe.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jv.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bx.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tc.haigaiapp.cn

[A07] 数字转字符串
来源：http://wz.bookmarksfly.cn

Py:   str(42)
来源：http://jh.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://lf.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://ru.huixinmuqiang.cn

TS:   String(42)
来源：http://dz.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://we.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://fe.nszjky.cn

Ruby: 42.to_s
来源：http://ak.521024.cn

C#:   42.ToString()
来源：http://ot.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://ed.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vl.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oo.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bk.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zl.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://if.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uy.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://it.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gf.colortex.cn

[A09] 绝对值与最大最小值
来源：http://sr.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yc.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mt.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://et.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ln.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ei.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qj.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://db.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://am.panjiajie.cn

[A10] 生成随机数
来源：http://yz.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://ig.asd995.cn

PHP:  random_int(1, 100);
来源：http://rb.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ai.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jv.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://pe.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nj.521024.cn

Ruby: rand(1..100)
来源：http://ac.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://zx.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://gq.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://fi.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jk.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bo.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wv.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://nv.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://du.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iw.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ew.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://pa.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://be.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://st.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://ge.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://ms.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://vl.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zp.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://hv.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://xo.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mg.asd995.cn

Py:   "第一行\n第二行"
来源：http://ri.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://gb.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://kq.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://bs.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://hr.szsharing.cn

Go:   "第一行\n第二行"
来源：http://zh.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://ek.colortex.cn

C#:   "第一行\n第二行"
来源：http://mr.bookmarksfly.cn

[A14] 注释写法
来源：http://yy.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vc.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wg.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://wr.hnjuh.cn


<!-- 参考信息 -->