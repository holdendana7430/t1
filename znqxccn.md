代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://uk.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nf.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ev.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nk.yuntaijiaju.cn

[U85] JS：可选链
来源：http://jw.521024.cn

a?.b?.c
来源：http://cs.shtwfgs.cn

[U86] JS：空值合并
来源：http://ea.yuexingan06.cn

a ?? b
来源：http://qg.gzmigu.cn

[U87] JS：解构默认值
来源：http://em.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://yz.huanxung.cn

[U88] JS：对象展开合并
来源：http://ye.bookmarksfly.cn

{ ...a, ...b }
来源：http://th.gzmigu.cn

[U89] JS：数组去重
来源：http://sv.colortex.cn

[...new Set(arr)]
来源：http://tl.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://dr.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://av.nicolike.cn

[U91] JS：对象键值遍历
来源：http://hy.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sp.shxzskj.cn

[U92] JS：深拷贝
来源：http://yc.nicolike.cn

structuredClone(obj)
来源：http://yh.9csxet.cn

[U93] JS：模板字符串
来源：http://sa.hnjuh.cn

`共 ${n} 条`
来源：http://ew.hahajie.cn

[U94] JS：箭头函数
来源：http://ik.panjiajie.cn

const double = x => x * 2;
来源：http://hm.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://ju.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://on.521024.cn

[U96] JS：async/await 与异常
来源：http://hb.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rx.nszjky.cn

[U97] JS：并发请求
来源：http://md.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ky.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://xs.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wf.521024.cn

[U99] JS：事件监听
来源：http://cx.asd995.cn

el.addEventListener("click", e => {})
来源：http://kv.shxzskj.cn

[U100] JS：DOM 查询
来源：http://uo.lnxyls.cn

document.querySelector(".item")
来源：http://yu.panjiajie.cn

[U101] JS：classList 操作
来源：http://ku.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://ir.nszjky.cn

[U102] JS：本地存储
来源：http://if.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xx.muxihuayi.cn

[U103] JS：定时器
来源：http://hm.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cm.haigaiapp.cn

[U104] JS：防抖
来源：http://ps.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mq.yuexingan06.cn

[U105] JS：节流
来源：http://mk.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rq.huixiangedu.cn

[U106] JS：日期格式化
来源：http://ll.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kh.huixiangedu.cn

[U107] JS：数字千分位
来源：http://gz.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yj.nszjky.cn

[U108] JS：随机整数
来源：http://lu.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ur.hnjuh.cn

[U109] JS：数组分组
来源：http://po.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://pa.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://jt.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uv.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://tm.shxzukj.cn

new Map(Object.entries(obj))
来源：http://up.nicolike.cn

[U112] JS：字符串补位
来源：http://fq.szsharing.cn

"7".padStart(3, "0")
来源：http://zy.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://oj.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://ow.hahajie.cn

[U114] JS：JSON 深比较
来源：http://bm.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iy.panjiajie.cn

[U115] JS：生成 UUID
来源：http://yj.szsharing.cn

crypto.randomUUID()
来源：http://ug.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://ol.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ub.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://oz.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://xw.gzmigu.cn

[U118] JS：开发服务器
来源：http://am.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://yt.huanxung.cn

[U119] JS：生产构建
来源：http://ou.bjjhwx.cn

npx vite build
来源：http://ls.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://bv.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://jy.szsharing.cn

================================================================================
来源：http://yn.wgjwhj.cn

统计汇总
来源：http://ai.hahajie.cn

================================================================================
来源：http://og.bookmarksfly.cn

按语言统计（条）：
来源：http://wz.bookmarksfly.cn

Python ......... 252
来源：http://ef.shtwfgs.cn

PHP ............ 252
来源：http://jc.szsharing.cn

JavaScript ..... 252
来源：http://nc.colortex.cn

TypeScript ..... 212
来源：http://om.huanxung.cn

Java ........... 212
来源：http://xz.huixiangedu.cn

Go ............. 212
来源：http://tr.szxytkj.cn

Ruby ........... 212
来源：http://yj.521024.cn

C# ............. 212
来源：http://kc.yuexingan06.cn

C .............. 30
来源：http://zb.szxytkj.cn

C++ ............ 30
来源：http://pr.huanxung.cn

SQL ............ 90
来源：http://nh.yuexingan06.cn

Bash ........... 80
来源：http://xr.yuexingan06.cn

Kotlin ......... 15
来源：http://au.chemitech.net.cn

Swift .......... 15
来源：http://zz.colortex.cn

Lua ............ 10
来源：http://za.asd995.cn

Perl ........... 10
来源：http://mw.haigaiapp.cn

Scala .......... 10
来源：http://wo.newstarts.cn

------------------------------------
来源：http://mk.gzmigu.cn

合计 ........... 2106 条
来源：http://nt.hnjuh.cn

按章节统计：
来源：http://fa.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lm.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lh.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ym.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fm.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gl.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ym.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pa.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vv.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qg.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gg.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://og.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lz.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://er.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oh.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://er.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ec.shxzukj.cn

Q SQL 专题                              90
来源：http://hj.yuexingan06.cn

R Bash 专题                             80
来源：http://lz.jctech888.com.cn

S C / C++ 专题                          60
来源：http://so.jctech888.com.cn

T 其他语言补充                          60
来源：http://cr.chemitech.net.cn

U 高频实用片段                         120
来源：http://ws.muxihuayi.cn

------------------------------------
来源：http://rj.muxihuayi.cn

合计                                  2106 条
来源：http://gb.asd995.cn

--------------------------------------------------------------------------------
来源：http://of.lnxyls.cn

使用提醒
来源：http://vj.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ea.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xq.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yt.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ui.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ia.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jw.521024.cn

—— 文件结束 ——
来源：http://hl.szsharing.cn

================================================================================
来源：http://qy.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://nt.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://jn.szsharing.cn

================================================================================
来源：http://os.bjjhwx.cn

【收录内容】
来源：http://yt.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ye.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zm.gzmigu.cn

SQL · Bash · C · C++
来源：http://xz.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nm.huixiangedu.cn

【使用说明】
来源：http://bl.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oh.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xs.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iq.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rr.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vc.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uq.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vk.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kp.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://be.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ya.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ta.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nn.nszjky.cn

【文件统计】
来源：http://my.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://up.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://rm.hahajie.cn

目  录
来源：http://yz.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ue.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ms.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fs.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://za.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ls.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rs.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lx.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eh.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qx.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gv.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://re.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vy.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jt.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ak.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aw.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ay.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://le.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iu.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bx.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://or.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lq.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kr.huixiangedu.cn

================================================================================
来源：http://to.yuexingan06.cn

A. 基础语法与类型
来源：http://kl.asd995.cn

================================================================================
来源：http://ah.colortex.cn

[A01] Hello World
来源：http://oj.newstarts.cn

Py:   print("Hello, World!")
来源：http://rq.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://wy.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://cv.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vz.521024.cn

Java: System.out.println("Hello, World!");
来源：http://sh.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://wa.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://rp.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://op.szsharing.cn

[A02] 变量声明与赋值
来源：http://af.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cc.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bw.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jq.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hh.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://cg.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://rh.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://fo.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sc.yuexingan06.cn

[A03] 常量定义
来源：http://cj.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kx.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://is.9csxet.cn

JS:   const PI = 3.14159;
来源：http://em.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://vy.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://px.hnjuh.cn

Go:   const PI = 3.14159
来源：http://mk.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://aq.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://oh.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://bc.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ip.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vf.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qo.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://nk.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ec.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wy.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dt.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://ks.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://gb.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://su.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mq.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yz.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ds.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://ac.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://ni.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://st.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://zf.9csxet.cn

[A06] 字符串转数字
来源：http://fe.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://je.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gm.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://di.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ki.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uu.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://na.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vy.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://za.asd995.cn

[A07] 数字转字符串
来源：http://vj.panjiajie.cn

Py:   str(42)
来源：http://ym.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://er.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://mr.nicolike.cn

TS:   String(42)
来源：http://cd.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bp.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://bs.chemitech.net.cn

Ruby: 42.to_s
来源：http://kp.huixiangedu.cn

C#:   42.ToString()
来源：http://et.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://ko.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wz.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zv.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uy.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pt.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://de.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wi.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pw.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qj.colortex.cn

[A09] 绝对值与最大最小值
来源：http://vi.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sk.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://af.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fe.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://le.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ce.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hi.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vt.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://je.yuexingan06.cn

[A10] 生成随机数
来源：http://vk.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://wb.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://hb.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pb.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yd.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://qr.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yb.nicolike.cn

Ruby: rand(1..100)
来源：http://bj.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://wu.nszjky.cn

[A11] 条件表达式（三元）
来源：http://ci.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://cu.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xd.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iq.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bj.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://zf.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wb.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bm.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ft.521024.cn

[A12] 字符串插值 / 格式化
来源：http://pv.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ml.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pv.asd995.cn

JS:   `Hello, ${name}!`
来源：http://fh.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://jg.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ga.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yb.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://kh.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://gs.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ym.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://fn.521024.cn

PHP:  "第一行\n第二行"
来源：http://lr.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://jv.521024.cn

TS:   "第一行\n第二行"
来源：http://pz.521024.cn

Java: "第一行\n第二行"
来源：http://fu.hahajie.cn

Go:   "第一行\n第二行"
来源：http://iw.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://ct.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://va.shtwfgs.cn


<!-- 参考信息 -->