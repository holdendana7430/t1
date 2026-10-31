代发 wailian999

[U89] JS：数组去重
来源：http://ix.gzmigu.cn

[...new Set(arr)]
来源：http://je.nszjky.cn

[U90] JS：数字数组排序
来源：http://sj.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://sm.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://mi.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kh.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://ex.521024.cn

structuredClone(obj)
来源：http://eg.haigaiapp.cn

[U93] JS：模板字符串
来源：http://ad.szsharing.cn

`共 ${n} 条`
来源：http://dj.szsharing.cn

[U94] JS：箭头函数
来源：http://ha.haigaiapp.cn

const double = x => x * 2;
来源：http://xo.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ux.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://kt.newstarts.cn

[U96] JS：async/await 与异常
来源：http://te.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cp.hahajie.cn

[U97] JS：并发请求
来源：http://ki.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sm.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://jo.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ls.9csxet.cn

[U99] JS：事件监听
来源：http://dk.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://yr.9csxet.cn

[U100] JS：DOM 查询
来源：http://bm.panjiajie.cn

document.querySelector(".item")
来源：http://rp.nszjky.cn

[U101] JS：classList 操作
来源：http://ir.yuexingan06.cn

el.classList.toggle("active")
来源：http://am.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://gj.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ga.muxihuayi.cn

[U103] JS：定时器
来源：http://gw.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://he.huanxung.cn

[U104] JS：防抖
来源：http://hx.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ou.bookmarksfly.cn

[U105] JS：节流
来源：http://mn.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://la.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://yh.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cc.huixiangedu.cn

[U107] JS：数字千分位
来源：http://sq.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rr.huanxung.cn

[U108] JS：随机整数
来源：http://rc.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jt.lnxyls.cn

[U109] JS：数组分组
来源：http://qc.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://kh.asd995.cn

[U110] JS：数组分块
来源：http://dy.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pd.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://pz.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://tk.chemitech.net.cn

[U112] JS：字符串补位
来源：http://sm.bjjhwx.cn

"7".padStart(3, "0")
来源：http://mt.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://sx.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://kf.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://mt.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://es.panjiajie.cn

[U115] JS：生成 UUID
来源：http://cm.yuntaijiaju.cn

crypto.randomUUID()
来源：http://sh.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://bx.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://cr.nszjky.cn

[U117] JS：单元测试
来源：http://ym.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://wq.521024.cn

[U118] JS：开发服务器
来源：http://ny.shxzukj.cn

npm i -D vite;  npx vite
来源：http://al.colortex.cn

[U119] JS：生产构建
来源：http://ep.szsharing.cn

npx vite build
来源：http://bn.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ee.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://jx.9csxet.cn

================================================================================
来源：http://rg.shxzskj.cn

统计汇总
来源：http://gc.hahajie.cn

================================================================================
来源：http://zl.huanxung.cn

按语言统计（条）：
来源：http://bq.muxihuayi.cn

Python ......... 252
来源：http://be.shxzukj.cn

PHP ............ 252
来源：http://ww.muxihuayi.cn

JavaScript ..... 252
来源：http://vi.nicolike.cn

TypeScript ..... 212
来源：http://cw.muxihuayi.cn

Java ........... 212
来源：http://ko.szxytkj.cn

Go ............. 212
来源：http://df.shxzukj.cn

Ruby ........... 212
来源：http://rx.muxihuayi.cn

C# ............. 212
来源：http://zn.wgjwhj.cn

C .............. 30
来源：http://de.hahajie.cn

C++ ............ 30
来源：http://ym.bjjhwx.cn

SQL ............ 90
来源：http://il.szxytkj.cn

Bash ........... 80
来源：http://gn.haigaiapp.cn

Kotlin ......... 15
来源：http://dg.shtwfgs.cn

Swift .......... 15
来源：http://pv.wgjwhj.cn

Lua ............ 10
来源：http://sz.bjjhwx.cn

Perl ........... 10
来源：http://ho.haigaiapp.cn

Scala .......... 10
来源：http://mv.yuexingan06.cn

------------------------------------
来源：http://pr.muxihuayi.cn

合计 ........... 2106 条
来源：http://ht.bookmarksfly.cn

按章节统计：
来源：http://tv.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ll.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://np.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aw.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qe.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hc.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uj.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://as.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kq.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bv.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jl.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wr.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://id.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dx.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rk.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fr.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uy.shxzskj.cn

Q SQL 专题                              90
来源：http://gt.yuexingan06.cn

R Bash 专题                             80
来源：http://nh.huanxung.cn

S C / C++ 专题                          60
来源：http://wx.muxihuayi.cn

T 其他语言补充                          60
来源：http://jr.muxihuayi.cn

U 高频实用片段                         120
来源：http://ge.wgjwhj.cn

------------------------------------
来源：http://lx.yuexingan06.cn

合计                                  2106 条
来源：http://rj.521024.cn

--------------------------------------------------------------------------------
来源：http://nf.jianghongdianzi.cn

使用提醒
来源：http://fi.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://kc.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xd.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ib.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sg.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nh.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jh.nicolike.cn

—— 文件结束 ——
来源：http://oo.muxihuayi.cn

================================================================================
来源：http://if.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://ur.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://hr.huanxung.cn

================================================================================
来源：http://cp.asd995.cn

【收录内容】
来源：http://od.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uf.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bl.shtwfgs.cn

SQL · Bash · C · C++
来源：http://ov.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nj.9csxet.cn

【使用说明】
来源：http://ox.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nv.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sf.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tk.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sa.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zm.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xf.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nd.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nb.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vy.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zy.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yc.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wd.9csxet.cn

【文件统计】
来源：http://wg.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xq.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ba.jianghongdianzi.cn

目  录
来源：http://xy.nszjky.cn

--------------------------------------------------------------------------------
来源：http://lh.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yx.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zv.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rh.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ya.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rg.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://as.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tj.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ng.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tk.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xu.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://et.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uv.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cd.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xz.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://os.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vk.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://na.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ik.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uq.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://il.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ix.huanxung.cn

================================================================================
来源：http://yv.jianghongdianzi.cn

A. 基础语法与类型
来源：http://ds.newstarts.cn

================================================================================
来源：http://jw.9csxet.cn

[A01] Hello World
来源：http://ro.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://kf.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://cc.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://hq.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ho.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://wt.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://lt.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://ey.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://go.newstarts.cn

[A02] 变量声明与赋值
来源：http://go.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rf.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aa.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kw.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ig.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://ar.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://ss.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://yq.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jy.huixiangedu.cn

[A03] 常量定义
来源：http://bp.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xd.521024.cn

PHP:  const PI = 3.14159;
来源：http://lb.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://da.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://bq.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://ku.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://fo.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://rw.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://xh.muxihuayi.cn

[A04] 判断变量类型
来源：http://fg.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yx.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iv.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ye.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://ck.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ns.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yg.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zk.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://nr.panjiajie.cn

[A05] 整数除法与取模
来源：http://iy.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ku.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://am.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yi.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bb.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://iu.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://ex.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://jq.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://rc.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://gt.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://oy.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hs.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://od.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mk.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qe.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tt.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ab.yuexingan06.cn

[A07] 数字转字符串
来源：http://mj.jianghongdianzi.cn

Py:   str(42)
来源：http://ee.521024.cn

PHP:  (string) 42; strval(42)
来源：http://va.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://tj.szxytkj.cn

TS:   String(42)
来源：http://cy.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gm.colortex.cn

Go:   strconv.Itoa(42)
来源：http://ix.bjjhwx.cn

Ruby: 42.to_s
来源：http://bv.shtwfgs.cn

C#:   42.ToString()
来源：http://wo.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://jy.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ry.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dl.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://am.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xw.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yf.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dc.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lu.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zw.colortex.cn

[A09] 绝对值与最大最小值
来源：http://ww.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zs.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pb.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bm.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kw.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://js.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aw.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ts.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ui.hnjuh.cn

[A10] 生成随机数
来源：http://fc.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://oq.huanxung.cn

PHP:  random_int(1, 100);
来源：http://fi.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jg.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rd.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://na.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fo.huixiangedu.cn

Ruby: rand(1..100)
来源：http://uz.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://kq.hahajie.cn

[A11] 条件表达式（三元）
来源：http://bd.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://gw.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sb.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kg.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qv.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://uf.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://md.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gp.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xd.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://le.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qo.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hg.colortex.cn

JS:   `Hello, ${name}!`
来源：http://rv.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://lz.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://fa.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xb.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://jm.521024.cn

C#:   $"Hello, {name}!"
来源：http://ua.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rs.colortex.cn

Py:   "第一行\n第二行"
来源：http://yb.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://fq.nicolike.cn

JS:   "第一行\n第二行"
来源：http://hc.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://la.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://qy.nicolike.cn

Go:   "第一行\n第二行"
来源：http://fp.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://jf.newstarts.cn

C#:   "第一行\n第二行"
来源：http://ic.lnxyls.cn

[A14] 注释写法
来源：http://zc.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dm.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ho.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://at.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://wf.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ue.521024.cn

Go:   // 单行；/* 多行 */
来源：http://am.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bf.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://wj.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://mm.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://ww.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://en.jianghongdianzi.cn


<!-- 参考信息 -->