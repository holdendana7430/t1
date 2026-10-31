代发 wailian999

[U67] PHP：处理文件上传
来源：http://yb.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cz.colortex.cn

[U68] PHP：PDO 连接
来源：http://gs.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pm.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://fd.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dk.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://el.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rt.asd995.cn

[U71] PHP：抛出异常
来源：http://fb.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://yh.shxzukj.cn

[U72] PHP：写错误日志
来源：http://ku.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://fm.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://yd.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://dp.colortex.cn

[U74] PHP：读取环境变量
来源：http://zo.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://sz.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://zl.gzmigu.cn

composer require psr/container
来源：http://mi.jctech888.com.cn

[U76] PHP：简单路由
来源：http://df.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ba.szsharing.cn

[U77] PHP：模板渲染
来源：http://iu.jctech888.com.cn

composer require twig/twig
来源：http://zt.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://jw.colortex.cn

composer require --dev phpunit/phpunit
来源：http://yq.haigaiapp.cn

[U79] PHP：静态分析
来源：http://lu.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://hp.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://fp.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oe.szxytkj.cn

[U81] JS：初始化项目
来源：http://vj.szsharing.cn

npm init -y;  npm i express
来源：http://wv.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://xm.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rz.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://ln.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rc.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://en.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://go.gzmigu.cn

[U85] JS：可选链
来源：http://kh.nicolike.cn

a?.b?.c
来源：http://am.asd995.cn

[U86] JS：空值合并
来源：http://rh.bjjhwx.cn

a ?? b
来源：http://np.asd995.cn

[U87] JS：解构默认值
来源：http://kw.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://jd.nszjky.cn

[U88] JS：对象展开合并
来源：http://qi.shxzskj.cn

{ ...a, ...b }
来源：http://bv.panjiajie.cn

[U89] JS：数组去重
来源：http://dt.huanxung.cn

[...new Set(arr)]
来源：http://tz.9csxet.cn

[U90] JS：数字数组排序
来源：http://mz.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://bs.huanxung.cn

[U91] JS：对象键值遍历
来源：http://zr.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jx.szsharing.cn

[U92] JS：深拷贝
来源：http://ae.521024.cn

structuredClone(obj)
来源：http://gl.nszjky.cn

[U93] JS：模板字符串
来源：http://af.szxytkj.cn

`共 ${n} 条`
来源：http://nb.nszjky.cn

[U94] JS：箭头函数
来源：http://ou.hahajie.cn

const double = x => x * 2;
来源：http://ji.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://ij.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://vb.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://gq.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dn.hnjuh.cn

[U97] JS：并发请求
来源：http://jm.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pg.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://rg.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pw.wgjwhj.cn

[U99] JS：事件监听
来源：http://gw.newstarts.cn

el.addEventListener("click", e => {})
来源：http://dr.hahajie.cn

[U100] JS：DOM 查询
来源：http://xe.wgjwhj.cn

document.querySelector(".item")
来源：http://pe.szsharing.cn

[U101] JS：classList 操作
来源：http://di.shxzukj.cn

el.classList.toggle("active")
来源：http://cz.panjiajie.cn

[U102] JS：本地存储
来源：http://ys.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pn.wgjwhj.cn

[U103] JS：定时器
来源：http://ji.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nv.shtwfgs.cn

[U104] JS：防抖
来源：http://zn.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gn.szsharing.cn

[U105] JS：节流
来源：http://ul.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zf.szxytkj.cn

[U106] JS：日期格式化
来源：http://gf.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://er.panjiajie.cn

[U107] JS：数字千分位
来源：http://tj.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://an.muxihuayi.cn

[U108] JS：随机整数
来源：http://px.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pj.szxytkj.cn

[U109] JS：数组分组
来源：http://ny.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://jx.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://px.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pd.szsharing.cn

[U111] JS：对象转 Map
来源：http://bb.521024.cn

new Map(Object.entries(obj))
来源：http://qq.jctech888.com.cn

[U112] JS：字符串补位
来源：http://go.huixiangedu.cn

"7".padStart(3, "0")
来源：http://ba.521024.cn

[U113] JS：正则替换全部
来源：http://gq.hnjuh.cn

s.replaceAll("a", "b")
来源：http://nf.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://xr.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hh.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://lj.lnxyls.cn

crypto.randomUUID()
来源：http://qf.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://zr.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://td.huixiangedu.cn

[U117] JS：单元测试
来源：http://hh.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://dv.colortex.cn

[U118] JS：开发服务器
来源：http://ip.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://fw.wgjwhj.cn

[U119] JS：生产构建
来源：http://ip.hahajie.cn

npx vite build
来源：http://il.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://gt.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://ju.szsharing.cn

================================================================================
来源：http://en.shxzukj.cn

统计汇总
来源：http://ci.9csxet.cn

================================================================================
来源：http://sa.panjiajie.cn

按语言统计（条）：
来源：http://xl.gzmigu.cn

Python ......... 252
来源：http://vc.asd995.cn

PHP ............ 252
来源：http://qe.jctech888.com.cn

JavaScript ..... 252
来源：http://bz.521024.cn

TypeScript ..... 212
来源：http://ml.haigaiapp.cn

Java ........... 212
来源：http://le.bookmarksfly.cn

Go ............. 212
来源：http://tw.lnxyls.cn

Ruby ........... 212
来源：http://ff.nszjky.cn

C# ............. 212
来源：http://oi.yuntaijiaju.cn

C .............. 30
来源：http://ft.jctech888.com.cn

C++ ............ 30
来源：http://is.jctech888.com.cn

SQL ............ 90
来源：http://ae.jianghongdianzi.cn

Bash ........... 80
来源：http://yr.shxzskj.cn

Kotlin ......... 15
来源：http://fc.nicolike.cn

Swift .......... 15
来源：http://dc.newstarts.cn

Lua ............ 10
来源：http://vz.hnjuh.cn

Perl ........... 10
来源：http://li.newstarts.cn

Scala .......... 10
来源：http://du.panjiajie.cn

------------------------------------
来源：http://wx.asd995.cn

合计 ........... 2106 条
来源：http://js.nicolike.cn

按章节统计：
来源：http://te.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fi.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zu.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zc.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rc.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://no.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://da.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fw.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ge.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mn.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tr.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ht.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yd.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://id.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kb.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ue.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mz.521024.cn

Q SQL 专题                              90
来源：http://vi.wgjwhj.cn

R Bash 专题                             80
来源：http://ku.shxzukj.cn

S C / C++ 专题                          60
来源：http://dg.chemitech.net.cn

T 其他语言补充                          60
来源：http://xz.shtwfgs.cn

U 高频实用片段                         120
来源：http://sr.nszjky.cn

------------------------------------
来源：http://ad.szsharing.cn

合计                                  2106 条
来源：http://rx.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bp.szxytkj.cn

使用提醒
来源：http://xi.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://tl.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vy.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fd.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dn.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tc.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://su.wgjwhj.cn

—— 文件结束 ——
来源：http://qw.hahajie.cn

================================================================================
来源：http://qh.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://rp.newstarts.cn

Common Programming Examples Cheat Book
来源：http://ef.huanxung.cn

================================================================================
来源：http://ij.huixiangedu.cn

【收录内容】
来源：http://bp.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pp.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uy.shxzskj.cn

SQL · Bash · C · C++
来源：http://xi.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lp.gzmigu.cn

【使用说明】
来源：http://ld.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bj.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mm.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://az.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ye.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ek.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kb.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://un.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ys.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://js.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yg.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cy.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ig.shxzskj.cn

【文件统计】
来源：http://wx.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yh.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ba.jctech888.com.cn

目  录
来源：http://ac.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://fb.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ll.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://im.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ry.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xg.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ph.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://av.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dx.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://us.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ri.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ip.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://um.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bi.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pi.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://um.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://im.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rt.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://as.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jd.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bc.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pp.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qb.bookmarksfly.cn

================================================================================
来源：http://yv.szsharing.cn

A. 基础语法与类型
来源：http://ow.shxzskj.cn

================================================================================
来源：http://ja.chemitech.net.cn

[A01] Hello World
来源：http://sm.hahajie.cn

Py:   print("Hello, World!")
来源：http://zd.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://yl.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://fm.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nt.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://cl.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://zx.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://sy.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wi.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://jo.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://we.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gy.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cb.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vo.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://so.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://nw.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://ir.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pk.bookmarksfly.cn

[A03] 常量定义
来源：http://pc.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nt.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://om.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://tp.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://hw.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://pl.hahajie.cn

Go:   const PI = 3.14159
来源：http://eb.huanxung.cn

Ruby: PI = 3.14159
来源：http://vx.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://dx.wgjwhj.cn

[A04] 判断变量类型
来源：http://mn.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qc.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zh.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uk.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://ha.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pe.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kr.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ei.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://lq.lnxyls.cn

[A05] 整数除法与取模
来源：http://oa.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://to.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xb.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cq.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rg.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://wu.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://vm.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://ne.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://kt.shxzskj.cn

[A06] 字符串转数字
来源：http://oz.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://mq.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bn.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jy.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://an.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zs.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jg.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zl.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gz.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://qw.hnjuh.cn

Py:   str(42)
来源：http://gm.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://fl.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://ge.szsharing.cn

TS:   String(42)
来源：http://lz.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ul.asd995.cn

Go:   strconv.Itoa(42)
来源：http://yg.gzmigu.cn

Ruby: 42.to_s
来源：http://ln.huanxung.cn

C#:   42.ToString()
来源：http://wr.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://uz.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://po.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zh.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ai.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tv.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rk.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mj.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ms.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gt.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://eb.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ad.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hm.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ig.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pw.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rs.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mp.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cj.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xi.huixiangedu.cn

[A10] 生成随机数
来源：http://sk.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://om.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://eb.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hv.shxzukj.cn


<!-- 参考信息 -->