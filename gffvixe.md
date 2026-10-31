代发 wailian999

[U71] PHP：抛出异常
来源：http://mt.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://fy.hnjuh.cn

[U72] PHP：写错误日志
来源：http://nw.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://fa.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://oz.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ux.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://rr.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://wf.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://hy.wgjwhj.cn

composer require psr/container
来源：http://ul.asd995.cn

[U76] PHP：简单路由
来源：http://qb.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uc.asd995.cn

[U77] PHP：模板渲染
来源：http://cn.hnjuh.cn

composer require twig/twig
来源：http://in.shxzskj.cn

[U78] PHP：单元测试
来源：http://go.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://du.yuexingan06.cn

[U79] PHP：静态分析
来源：http://lh.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://vl.hahajie.cn

[U80] PHP：代码规范修复
来源：http://dt.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ft.shtwfgs.cn

[U81] JS：初始化项目
来源：http://as.haigaiapp.cn

npm init -y;  npm i express
来源：http://co.521024.cn

[U82] JS：package.json 脚本
来源：http://xz.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bu.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://ts.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://df.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://ol.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qc.shxzukj.cn

[U85] JS：可选链
来源：http://rm.chemitech.net.cn

a?.b?.c
来源：http://yg.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://rh.chemitech.net.cn

a ?? b
来源：http://po.gzmigu.cn

[U87] JS：解构默认值
来源：http://dr.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://sb.huanxung.cn

[U88] JS：对象展开合并
来源：http://rq.gzmigu.cn

{ ...a, ...b }
来源：http://gy.bjjhwx.cn

[U89] JS：数组去重
来源：http://vq.hnjuh.cn

[...new Set(arr)]
来源：http://wi.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://nh.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://iu.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://lg.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hq.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://nf.szsharing.cn

structuredClone(obj)
来源：http://vb.shtwfgs.cn

[U93] JS：模板字符串
来源：http://mw.asd995.cn

`共 ${n} 条`
来源：http://yq.bjjhwx.cn

[U94] JS：箭头函数
来源：http://nd.panjiajie.cn

const double = x => x * 2;
来源：http://xz.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://nr.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://jn.521024.cn

[U96] JS：async/await 与异常
来源：http://ck.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dw.nicolike.cn

[U97] JS：并发请求
来源：http://sg.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zb.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ej.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ar.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://ra.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://vm.huanxung.cn

[U100] JS：DOM 查询
来源：http://kt.yuexingan06.cn

document.querySelector(".item")
来源：http://jd.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://xo.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://zc.chemitech.net.cn

[U102] JS：本地存储
来源：http://mt.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://el.nszjky.cn

[U103] JS：定时器
来源：http://mk.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lm.asd995.cn

[U104] JS：防抖
来源：http://lx.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mi.huixiangedu.cn

[U105] JS：节流
来源：http://qe.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://te.chemitech.net.cn

[U106] JS：日期格式化
来源：http://fw.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://at.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://ox.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dk.newstarts.cn

[U108] JS：随机整数
来源：http://yn.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qn.szxytkj.cn

[U109] JS：数组分组
来源：http://ax.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://ug.bjjhwx.cn

[U110] JS：数组分块
来源：http://bo.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ao.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://dn.panjiajie.cn

new Map(Object.entries(obj))
来源：http://ao.nszjky.cn

[U112] JS：字符串补位
来源：http://zx.hahajie.cn

"7".padStart(3, "0")
来源：http://lf.hnjuh.cn

[U113] JS：正则替换全部
来源：http://zf.colortex.cn

s.replaceAll("a", "b")
来源：http://nv.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://xy.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ty.asd995.cn

[U115] JS：生成 UUID
来源：http://tt.yuexingan06.cn

crypto.randomUUID()
来源：http://lm.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://mc.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://ts.asd995.cn

[U117] JS：单元测试
来源：http://go.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://gp.wgjwhj.cn

[U118] JS：开发服务器
来源：http://gp.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://rn.hnjuh.cn

[U119] JS：生产构建
来源：http://wj.chemitech.net.cn

npx vite build
来源：http://vv.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://hz.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://ow.yuntaijiaju.cn

================================================================================
来源：http://qj.shxzskj.cn

统计汇总
来源：http://zb.szsharing.cn

================================================================================
来源：http://yj.yuexingan06.cn

按语言统计（条）：
来源：http://hq.szxytkj.cn

Python ......... 252
来源：http://ab.shxzskj.cn

PHP ............ 252
来源：http://hx.521024.cn

JavaScript ..... 252
来源：http://rb.szsharing.cn

TypeScript ..... 212
来源：http://yy.521024.cn

Java ........... 212
来源：http://lv.szxytkj.cn

Go ............. 212
来源：http://hx.muxihuayi.cn

Ruby ........... 212
来源：http://ke.huanxung.cn

C# ............. 212
来源：http://xg.colortex.cn

C .............. 30
来源：http://id.bjjhwx.cn

C++ ............ 30
来源：http://eu.colortex.cn

SQL ............ 90
来源：http://uc.nszjky.cn

Bash ........... 80
来源：http://ko.szsharing.cn

Kotlin ......... 15
来源：http://xr.shxzukj.cn

Swift .......... 15
来源：http://ng.chemitech.net.cn

Lua ............ 10
来源：http://vq.gzmigu.cn

Perl ........... 10
来源：http://wd.muxihuayi.cn

Scala .......... 10
来源：http://ze.hnjuh.cn

------------------------------------
来源：http://yt.lnxyls.cn

合计 ........... 2106 条
来源：http://ut.shxzukj.cn

按章节统计：
来源：http://wk.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ap.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bp.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kt.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ws.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vw.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bh.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gb.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ty.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dr.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://te.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zi.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yu.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pw.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yo.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cd.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dy.wgjwhj.cn

Q SQL 专题                              90
来源：http://xi.yuntaijiaju.cn

R Bash 专题                             80
来源：http://wb.chemitech.net.cn

S C / C++ 专题                          60
来源：http://rj.szxytkj.cn

T 其他语言补充                          60
来源：http://tn.szxytkj.cn

U 高频实用片段                         120
来源：http://jg.colortex.cn

------------------------------------
来源：http://ui.yuntaijiaju.cn

合计                                  2106 条
来源：http://zw.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://vw.haigaiapp.cn

使用提醒
来源：http://sb.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://di.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://up.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sv.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gd.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://le.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mw.hnjuh.cn

—— 文件结束 ——
来源：http://zw.shtwfgs.cn

================================================================================
来源：http://fm.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://uh.szsharing.cn

Common Programming Examples Cheat Book
来源：http://co.shxzskj.cn

================================================================================
来源：http://qi.jctech888.com.cn

【收录内容】
来源：http://xj.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ti.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qw.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://ys.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sr.bookmarksfly.cn

【使用说明】
来源：http://hf.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tn.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hk.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tq.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wh.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nd.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ph.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hd.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yz.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ej.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ar.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vo.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xk.bookmarksfly.cn

【文件统计】
来源：http://gv.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://md.szsharing.cn

--------------------------------------------------------------------------------
来源：http://bu.haigaiapp.cn

目  录
来源：http://pn.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ji.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qo.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mf.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ju.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ou.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mx.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://he.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nm.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://of.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ms.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://np.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fm.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://om.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://op.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fw.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://id.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zu.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sx.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qn.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qo.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pm.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zn.yuexingan06.cn

================================================================================
来源：http://yg.muxihuayi.cn

A. 基础语法与类型
来源：http://ub.asd995.cn

================================================================================
来源：http://ep.shtwfgs.cn

[A01] Hello World
来源：http://cp.panjiajie.cn

Py:   print("Hello, World!")
来源：http://ou.521024.cn

PHP:  echo "Hello, World!";
来源：http://de.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://by.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ao.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://ii.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://eh.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://xx.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jj.521024.cn

[A02] 变量声明与赋值
来源：http://pi.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nm.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vo.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ow.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wn.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://gc.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://hh.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://uc.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ly.chemitech.net.cn

[A03] 常量定义
来源：http://bp.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jn.asd995.cn

PHP:  const PI = 3.14159;
来源：http://dy.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://lm.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://kx.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://eg.szsharing.cn

Go:   const PI = 3.14159
来源：http://uh.shxzukj.cn

Ruby: PI = 3.14159
来源：http://ep.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://pu.haigaiapp.cn

[A04] 判断变量类型
来源：http://zn.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ly.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dx.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fn.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://bb.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gy.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ge.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ts.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://ef.hnjuh.cn

[A05] 整数除法与取模
来源：http://pa.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bz.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ek.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://io.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xh.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://ik.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://iv.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://br.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://wx.nszjky.cn

[A06] 字符串转数字
来源：http://do.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://pf.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yh.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uh.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wq.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lv.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ua.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://un.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hl.nszjky.cn

[A07] 数字转字符串
来源：http://dz.jctech888.com.cn

Py:   str(42)
来源：http://fb.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://pr.521024.cn

JS:   String(42); (42).toString()
来源：http://yf.yuexingan06.cn

TS:   String(42)
来源：http://rc.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ho.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://yc.shxzukj.cn

Ruby: 42.to_s
来源：http://kw.muxihuayi.cn

C#:   42.ToString()
来源：http://er.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://ay.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yz.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kj.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lr.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jv.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fc.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qr.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xd.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ti.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://dr.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zi.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cb.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eo.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://an.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pb.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://to.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fl.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ob.yuexingan06.cn

[A10] 生成随机数
来源：http://va.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ui.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://xo.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xn.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yb.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://ie.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ki.shxzskj.cn

Ruby: rand(1..100)
来源：http://vy.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://hk.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://oh.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://jk.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rp.wgjwhj.cn


<!-- 参考信息 -->