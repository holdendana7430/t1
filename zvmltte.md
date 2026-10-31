代发 wailian999

[U69] PHP：PDO 预处理
来源：http://fb.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cc.hahajie.cn

[U70] PHP：PDO 事务
来源：http://un.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zt.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ni.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://vg.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://kz.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://bd.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://rs.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://mw.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://yz.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ps.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://fb.gzmigu.cn

composer require psr/container
来源：http://zn.huanxung.cn

[U76] PHP：简单路由
来源：http://ia.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xn.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://wv.hnjuh.cn

composer require twig/twig
来源：http://xw.shtwfgs.cn

[U78] PHP：单元测试
来源：http://yd.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://ne.yuexingan06.cn

[U79] PHP：静态分析
来源：http://dd.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://so.nicolike.cn

[U80] PHP：代码规范修复
来源：http://tt.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sq.huixiangedu.cn

[U81] JS：初始化项目
来源：http://rc.hnjuh.cn

npm init -y;  npm i express
来源：http://rr.asd995.cn

[U82] JS：package.json 脚本
来源：http://uq.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xi.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://rj.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lq.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://nq.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yp.haigaiapp.cn

[U85] JS：可选链
来源：http://mv.panjiajie.cn

a?.b?.c
来源：http://oz.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://fp.bjjhwx.cn

a ?? b
来源：http://pu.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://yp.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://fu.szsharing.cn

[U88] JS：对象展开合并
来源：http://xv.huixiangedu.cn

{ ...a, ...b }
来源：http://lj.nicolike.cn

[U89] JS：数组去重
来源：http://si.szsharing.cn

[...new Set(arr)]
来源：http://hl.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://xp.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://xz.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://ul.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eu.newstarts.cn

[U92] JS：深拷贝
来源：http://bo.jctech888.com.cn

structuredClone(obj)
来源：http://bx.shtwfgs.cn

[U93] JS：模板字符串
来源：http://wn.shxzukj.cn

`共 ${n} 条`
来源：http://ej.gzmigu.cn

[U94] JS：箭头函数
来源：http://vx.muxihuayi.cn

const double = x => x * 2;
来源：http://fz.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://bp.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://un.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://qi.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://th.bjjhwx.cn

[U97] JS：并发请求
来源：http://wc.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://we.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://do.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kn.shtwfgs.cn

[U99] JS：事件监听
来源：http://yj.hahajie.cn

el.addEventListener("click", e => {})
来源：http://co.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://gg.newstarts.cn

document.querySelector(".item")
来源：http://km.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://ah.shxzukj.cn

el.classList.toggle("active")
来源：http://ti.haigaiapp.cn

[U102] JS：本地存储
来源：http://vf.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qd.huixinmuqiang.cn

[U103] JS：定时器
来源：http://xb.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gt.szxytkj.cn

[U104] JS：防抖
来源：http://os.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tt.bookmarksfly.cn

[U105] JS：节流
来源：http://ty.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fu.szxytkj.cn

[U106] JS：日期格式化
来源：http://um.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gz.9csxet.cn

[U107] JS：数字千分位
来源：http://fv.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lf.szsharing.cn

[U108] JS：随机整数
来源：http://mr.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ua.jctech888.com.cn

[U109] JS：数组分组
来源：http://cd.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://cz.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://lj.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wu.shxzukj.cn

[U111] JS：对象转 Map
来源：http://hh.hnjuh.cn

new Map(Object.entries(obj))
来源：http://uw.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://mr.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://ek.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://qu.gzmigu.cn

s.replaceAll("a", "b")
来源：http://mv.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://fr.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://me.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://jv.jianghongdianzi.cn

crypto.randomUUID()
来源：http://zx.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tv.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://fc.shxzskj.cn

[U117] JS：单元测试
来源：http://tn.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ho.szsharing.cn

[U118] JS：开发服务器
来源：http://qc.hahajie.cn

npm i -D vite;  npx vite
来源：http://ap.nicolike.cn

[U119] JS：生产构建
来源：http://dq.szsharing.cn

npx vite build
来源：http://rx.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://kr.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://pz.jianghongdianzi.cn

================================================================================
来源：http://cc.chemitech.net.cn

统计汇总
来源：http://wi.szxytkj.cn

================================================================================
来源：http://fb.huixiangedu.cn

按语言统计（条）：
来源：http://zt.colortex.cn

Python ......... 252
来源：http://if.newstarts.cn

PHP ............ 252
来源：http://iu.shxzskj.cn

JavaScript ..... 252
来源：http://hy.panjiajie.cn

TypeScript ..... 212
来源：http://in.panjiajie.cn

Java ........... 212
来源：http://es.chemitech.net.cn

Go ............. 212
来源：http://zj.shxzskj.cn

Ruby ........... 212
来源：http://bw.colortex.cn

C# ............. 212
来源：http://my.jianghongdianzi.cn

C .............. 30
来源：http://io.hahajie.cn

C++ ............ 30
来源：http://gu.szsharing.cn

SQL ............ 90
来源：http://wm.hnjuh.cn

Bash ........... 80
来源：http://ab.haigaiapp.cn

Kotlin ......... 15
来源：http://ev.colortex.cn

Swift .......... 15
来源：http://jx.shxzukj.cn

Lua ............ 10
来源：http://jo.9csxet.cn

Perl ........... 10
来源：http://fl.colortex.cn

Scala .......... 10
来源：http://xc.huanxung.cn

------------------------------------
来源：http://mg.hnjuh.cn

合计 ........... 2106 条
来源：http://fp.shxzskj.cn

按章节统计：
来源：http://ge.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kr.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zf.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qk.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gl.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vh.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gb.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pw.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ca.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dc.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xi.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mb.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zn.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://la.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kg.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ff.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hb.colortex.cn

Q SQL 专题                              90
来源：http://wk.huanxung.cn

R Bash 专题                             80
来源：http://ta.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://dx.lnxyls.cn

T 其他语言补充                          60
来源：http://hh.bookmarksfly.cn

U 高频实用片段                         120
来源：http://jx.shxzukj.cn

------------------------------------
来源：http://xs.szxytkj.cn

合计                                  2106 条
来源：http://ix.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://av.nszjky.cn

使用提醒
来源：http://ua.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ei.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lh.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ov.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xj.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bp.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ru.wgjwhj.cn

—— 文件结束 ——
来源：http://vp.haigaiapp.cn

================================================================================
来源：http://jb.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ce.521024.cn

Common Programming Examples Cheat Book
来源：http://bt.521024.cn

================================================================================
来源：http://qd.huixinmuqiang.cn

【收录内容】
来源：http://cm.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gb.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vt.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://rt.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ok.jctech888.com.cn

【使用说明】
来源：http://yj.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xv.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jx.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aa.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gp.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ou.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vq.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://an.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ye.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dl.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ua.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://is.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bn.shxzskj.cn

【文件统计】
来源：http://du.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ts.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://my.bjjhwx.cn

目  录
来源：http://mu.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://lp.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hf.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xv.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yr.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ut.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vv.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dv.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ut.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sn.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nn.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ub.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qz.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dp.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ph.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mn.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hr.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gj.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sw.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fp.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ed.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bu.bjjhwx.cn

================================================================================
来源：http://tg.szxytkj.cn

A. 基础语法与类型
来源：http://vy.panjiajie.cn

================================================================================
来源：http://vu.colortex.cn

[A01] Hello World
来源：http://wa.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ne.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://jg.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://dt.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xu.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://mg.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://zj.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://ws.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ce.9csxet.cn

[A02] 变量声明与赋值
来源：http://jt.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ni.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aw.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xk.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://th.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ry.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://df.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://tp.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jh.hnjuh.cn

[A03] 常量定义
来源：http://tm.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ee.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://ja.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ne.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://hx.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://wo.szsharing.cn

Go:   const PI = 3.14159
来源：http://zi.521024.cn

Ruby: PI = 3.14159
来源：http://jm.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://pp.yuexingan06.cn

[A04] 判断变量类型
来源：http://zt.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dt.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sz.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qj.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://dx.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jw.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yq.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rp.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://hg.newstarts.cn

[A05] 整数除法与取模
来源：http://tk.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pv.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qv.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eu.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gn.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://pt.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://oy.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://qi.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://vn.huixiangedu.cn

[A06] 字符串转数字
来源：http://qg.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://we.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vi.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cl.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fg.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hf.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kf.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gu.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tg.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://sr.bookmarksfly.cn

Py:   str(42)
来源：http://cr.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ni.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://ka.nszjky.cn

TS:   String(42)
来源：http://bd.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qk.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://jx.muxihuayi.cn

Ruby: 42.to_s
来源：http://nj.521024.cn

C#:   42.ToString()
来源：http://vq.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://dd.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://st.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lx.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eg.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ku.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://od.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eo.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hr.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sg.asd995.cn

[A09] 绝对值与最大最小值
来源：http://yv.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pc.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wl.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://de.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uc.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://et.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vw.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pg.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pc.bjjhwx.cn

[A10] 生成随机数
来源：http://th.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://ct.huanxung.cn

PHP:  random_int(1, 100);
来源：http://qx.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://su.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ml.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://xz.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nd.bjjhwx.cn

Ruby: rand(1..100)
来源：http://nd.shxzskj.cn


<!-- 参考信息 -->