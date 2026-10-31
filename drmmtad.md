代发 wailian999

[U89] JS：数组去重
来源：http://eg.szsharing.cn

[...new Set(arr)]
来源：http://sv.panjiajie.cn

[U90] JS：数字数组排序
来源：http://mc.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://cz.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://lk.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://er.huanxung.cn

[U92] JS：深拷贝
来源：http://oz.gzmigu.cn

structuredClone(obj)
来源：http://vp.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://lz.hahajie.cn

`共 ${n} 条`
来源：http://pj.lnxyls.cn

[U94] JS：箭头函数
来源：http://su.9csxet.cn

const double = x => x * 2;
来源：http://ja.lnxyls.cn

[U95] JS：Promise 包装
来源：http://nv.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://jw.hahajie.cn

[U96] JS：async/await 与异常
来源：http://ri.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dq.shxzukj.cn

[U97] JS：并发请求
来源：http://vo.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tq.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://ie.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://in.jctech888.com.cn

[U99] JS：事件监听
来源：http://qq.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://mm.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://wz.521024.cn

document.querySelector(".item")
来源：http://wv.muxihuayi.cn

[U101] JS：classList 操作
来源：http://hy.hahajie.cn

el.classList.toggle("active")
来源：http://of.yuexingan06.cn

[U102] JS：本地存储
来源：http://vj.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dz.colortex.cn

[U103] JS：定时器
来源：http://cc.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qq.wgjwhj.cn

[U104] JS：防抖
来源：http://zx.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.shxzukj.cn

[U105] JS：节流
来源：http://wo.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jt.hnjuh.cn

[U106] JS：日期格式化
来源：http://mu.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ix.szxytkj.cn

[U107] JS：数字千分位
来源：http://io.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nl.wgjwhj.cn

[U108] JS：随机整数
来源：http://di.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sf.9csxet.cn

[U109] JS：数组分组
来源：http://sr.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://xr.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://jx.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iw.colortex.cn

[U111] JS：对象转 Map
来源：http://ye.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://rr.newstarts.cn

[U112] JS：字符串补位
来源：http://wv.jctech888.com.cn

"7".padStart(3, "0")
来源：http://cl.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://dm.asd995.cn

s.replaceAll("a", "b")
来源：http://iq.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://bg.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oy.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://of.huanxung.cn

crypto.randomUUID()
来源：http://ua.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://fo.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://ag.haigaiapp.cn

[U117] JS：单元测试
来源：http://fs.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://zi.asd995.cn

[U118] JS：开发服务器
来源：http://gl.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://zv.szsharing.cn

[U119] JS：生产构建
来源：http://yl.haigaiapp.cn

npx vite build
来源：http://xf.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://la.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://xt.huixiangedu.cn

================================================================================
来源：http://rl.muxihuayi.cn

统计汇总
来源：http://ng.yuntaijiaju.cn

================================================================================
来源：http://cc.wgjwhj.cn

按语言统计（条）：
来源：http://vt.521024.cn

Python ......... 252
来源：http://ni.nszjky.cn

PHP ............ 252
来源：http://xh.yuntaijiaju.cn

JavaScript ..... 252
来源：http://ff.chemitech.net.cn

TypeScript ..... 212
来源：http://xw.521024.cn

Java ........... 212
来源：http://ir.shtwfgs.cn

Go ............. 212
来源：http://zh.gzmigu.cn

Ruby ........... 212
来源：http://hx.hnjuh.cn

C# ............. 212
来源：http://jz.hnjuh.cn

C .............. 30
来源：http://xo.hnjuh.cn

C++ ............ 30
来源：http://ab.9csxet.cn

SQL ............ 90
来源：http://bz.huixinmuqiang.cn

Bash ........... 80
来源：http://dq.wgjwhj.cn

Kotlin ......... 15
来源：http://zp.yuntaijiaju.cn

Swift .......... 15
来源：http://xv.panjiajie.cn

Lua ............ 10
来源：http://aj.shxzskj.cn

Perl ........... 10
来源：http://fb.muxihuayi.cn

Scala .......... 10
来源：http://vw.szxytkj.cn

------------------------------------
来源：http://np.bjjhwx.cn

合计 ........... 2106 条
来源：http://yj.colortex.cn

按章节统计：
来源：http://dp.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fv.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fg.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ny.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://az.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jq.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ze.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://of.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ik.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fq.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fg.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wq.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qg.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hn.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ta.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hl.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hw.lnxyls.cn

Q SQL 专题                              90
来源：http://lc.gzmigu.cn

R Bash 专题                             80
来源：http://jl.shxzukj.cn

S C / C++ 专题                          60
来源：http://qo.gzmigu.cn

T 其他语言补充                          60
来源：http://ga.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://sq.9csxet.cn

------------------------------------
来源：http://mv.gzmigu.cn

合计                                  2106 条
来源：http://tg.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://mv.jianghongdianzi.cn

使用提醒
来源：http://kk.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://xa.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kl.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fo.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pa.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://me.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dy.shxzukj.cn

—— 文件结束 ——
来源：http://az.huanxung.cn

================================================================================
来源：http://ga.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://bg.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://cw.wgjwhj.cn

================================================================================
来源：http://tf.shxzukj.cn

【收录内容】
来源：http://hg.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qg.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wj.nicolike.cn

SQL · Bash · C · C++
来源：http://kv.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ns.huixiangedu.cn

【使用说明】
来源：http://qt.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ts.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wu.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ii.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nv.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eq.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jo.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gz.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ws.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://os.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uv.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rf.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pp.huanxung.cn

【文件统计】
来源：http://bo.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tt.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://cu.colortex.cn

目  录
来源：http://bi.nszjky.cn

--------------------------------------------------------------------------------
来源：http://le.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lc.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://or.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://da.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ts.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tr.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://at.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qp.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nb.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fj.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qm.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sm.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ne.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gq.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wb.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gl.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yo.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tk.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nn.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yj.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wh.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mf.gzmigu.cn

================================================================================
来源：http://ro.colortex.cn

A. 基础语法与类型
来源：http://de.wgjwhj.cn

================================================================================
来源：http://px.hahajie.cn

[A01] Hello World
来源：http://mi.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://ne.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://tj.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://bg.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sh.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://xy.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://rp.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://ki.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yv.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://ef.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kk.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bi.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wv.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uw.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://dq.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://hc.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://ux.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ug.shxzukj.cn

[A03] 常量定义
来源：http://if.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oj.521024.cn

PHP:  const PI = 3.14159;
来源：http://je.newstarts.cn

JS:   const PI = 3.14159;
来源：http://al.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://co.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://eb.hnjuh.cn

Go:   const PI = 3.14159
来源：http://kp.521024.cn

Ruby: PI = 3.14159
来源：http://js.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://lw.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://gb.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lk.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bz.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nl.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://ir.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hq.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mj.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://js.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://lz.szsharing.cn

[A05] 整数除法与取模
来源：http://to.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://id.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ux.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://io.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nt.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://oc.521024.cn

Go:   7 / 2; 7 % 2
来源：http://zp.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://vg.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://sn.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://kp.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://jd.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hj.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://va.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xa.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dl.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wr.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qb.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://md.newstarts.cn

[A07] 数字转字符串
来源：http://kd.jianghongdianzi.cn

Py:   str(42)
来源：http://is.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://ae.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://bg.shtwfgs.cn

TS:   String(42)
来源：http://zf.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sa.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://if.asd995.cn

Ruby: 42.to_s
来源：http://ol.chemitech.net.cn

C#:   42.ToString()
来源：http://hn.lnxyls.cn

[A08] 取整与四舍五入
来源：http://yx.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://th.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ko.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pj.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yk.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jl.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qh.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xd.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lq.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://uz.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lc.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ms.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kb.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vg.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zw.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mf.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fq.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tt.gzmigu.cn

[A10] 生成随机数
来源：http://jf.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://km.521024.cn

PHP:  random_int(1, 100);
来源：http://ac.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ot.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ax.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://am.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ml.huixiangedu.cn

Ruby: rand(1..100)
来源：http://rd.521024.cn

C#:   new Random().Next(1, 101)
来源：http://rw.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://cc.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://xr.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ot.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bm.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ye.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://uz.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tx.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tk.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ov.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://hd.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pb.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lt.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://ul.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://sf.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://dq.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bh.521024.cn

Ruby: "Hello, #{name}!"
来源：http://eh.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://wd.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mq.szsharing.cn

Py:   "第一行\n第二行"
来源：http://pj.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://gx.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://ts.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://oa.hnjuh.cn

Java: "第一行\n第二行"
来源：http://gr.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://zz.521024.cn

Ruby: "第一行\n第二行"
来源：http://lt.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://nx.panjiajie.cn

[A14] 注释写法
来源：http://uy.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yv.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tv.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://mp.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://ok.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rs.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://se.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ls.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://gm.lnxyls.cn

[A15] 空值判断与默认值
来源：http://hx.asd995.cn

Py:   value = data or "默认值"
来源：http://oa.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://yu.huixiangedu.cn


<!-- 参考信息 -->