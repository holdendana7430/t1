代发 wailian999

[U67] PHP：处理文件上传
来源：http://qu.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ub.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://ul.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fe.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://ib.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ru.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ks.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lk.huanxung.cn

[U71] PHP：抛出异常
来源：http://pn.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://rz.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://md.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://gy.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://su.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://de.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://an.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ij.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://mk.jctech888.com.cn

composer require psr/container
来源：http://wd.jctech888.com.cn

[U76] PHP：简单路由
来源：http://tz.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sy.shxzukj.cn

[U77] PHP：模板渲染
来源：http://jo.huanxung.cn

composer require twig/twig
来源：http://ly.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://lg.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://ps.jctech888.com.cn

[U79] PHP：静态分析
来源：http://kk.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://ii.hahajie.cn

[U80] PHP：代码规范修复
来源：http://ik.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bk.newstarts.cn

[U81] JS：初始化项目
来源：http://vc.chemitech.net.cn

npm init -y;  npm i express
来源：http://zn.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://ut.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ej.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://gb.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xn.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://lz.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://be.521024.cn

[U85] JS：可选链
来源：http://qc.asd995.cn

a?.b?.c
来源：http://nh.szxytkj.cn

[U86] JS：空值合并
来源：http://fw.hahajie.cn

a ?? b
来源：http://xh.yuexingan06.cn

[U87] JS：解构默认值
来源：http://lv.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://al.lnxyls.cn

[U88] JS：对象展开合并
来源：http://fl.haigaiapp.cn

{ ...a, ...b }
来源：http://qs.szxytkj.cn

[U89] JS：数组去重
来源：http://wf.huixiangedu.cn

[...new Set(arr)]
来源：http://ko.gzmigu.cn

[U90] JS：数字数组排序
来源：http://xx.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://pq.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://hg.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ey.colortex.cn

[U92] JS：深拷贝
来源：http://nn.chemitech.net.cn

structuredClone(obj)
来源：http://av.szsharing.cn

[U93] JS：模板字符串
来源：http://ac.nszjky.cn

`共 ${n} 条`
来源：http://cq.jctech888.com.cn

[U94] JS：箭头函数
来源：http://gj.huixiangedu.cn

const double = x => x * 2;
来源：http://kk.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://fq.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ix.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://hz.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zz.asd995.cn

[U97] JS：并发请求
来源：http://bv.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tk.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://zo.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iw.nszjky.cn

[U99] JS：事件监听
来源：http://nj.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://qe.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://ot.panjiajie.cn

document.querySelector(".item")
来源：http://of.bjjhwx.cn

[U101] JS：classList 操作
来源：http://xy.521024.cn

el.classList.toggle("active")
来源：http://oo.huixiangedu.cn

[U102] JS：本地存储
来源：http://gq.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dj.yuexingan06.cn

[U103] JS：定时器
来源：http://uu.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kr.muxihuayi.cn

[U104] JS：防抖
来源：http://vl.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dg.shtwfgs.cn

[U105] JS：节流
来源：http://nt.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vb.huanxung.cn

[U106] JS：日期格式化
来源：http://st.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wd.asd995.cn

[U107] JS：数字千分位
来源：http://rn.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mt.hahajie.cn

[U108] JS：随机整数
来源：http://dn.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://at.nicolike.cn

[U109] JS：数组分组
来源：http://lb.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://gu.szsharing.cn

[U110] JS：数组分块
来源：http://hv.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://py.hahajie.cn

[U111] JS：对象转 Map
来源：http://uz.panjiajie.cn

new Map(Object.entries(obj))
来源：http://qx.nicolike.cn

[U112] JS：字符串补位
来源：http://ov.shxzskj.cn

"7".padStart(3, "0")
来源：http://gc.nicolike.cn

[U113] JS：正则替换全部
来源：http://ur.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://jy.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://td.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sf.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://oz.szsharing.cn

crypto.randomUUID()
来源：http://tj.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ow.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://wp.huixiangedu.cn

[U117] JS：单元测试
来源：http://dl.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://vc.shtwfgs.cn

[U118] JS：开发服务器
来源：http://wq.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://rl.shxzskj.cn

[U119] JS：生产构建
来源：http://xj.haigaiapp.cn

npx vite build
来源：http://id.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://lu.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://vj.jianghongdianzi.cn

================================================================================
来源：http://rc.hahajie.cn

统计汇总
来源：http://zt.hahajie.cn

================================================================================
来源：http://ls.yuntaijiaju.cn

按语言统计（条）：
来源：http://uw.bookmarksfly.cn

Python ......... 252
来源：http://em.colortex.cn

PHP ............ 252
来源：http://pr.newstarts.cn

JavaScript ..... 252
来源：http://sz.jctech888.com.cn

TypeScript ..... 212
来源：http://jr.panjiajie.cn

Java ........... 212
来源：http://av.jianghongdianzi.cn

Go ............. 212
来源：http://rn.huixinmuqiang.cn

Ruby ........... 212
来源：http://ga.bookmarksfly.cn

C# ............. 212
来源：http://wp.shtwfgs.cn

C .............. 30
来源：http://ud.nicolike.cn

C++ ............ 30
来源：http://nv.hnjuh.cn

SQL ............ 90
来源：http://vr.haigaiapp.cn

Bash ........... 80
来源：http://uv.shtwfgs.cn

Kotlin ......... 15
来源：http://qz.szxytkj.cn

Swift .......... 15
来源：http://ss.colortex.cn

Lua ............ 10
来源：http://dw.asd995.cn

Perl ........... 10
来源：http://xy.wgjwhj.cn

Scala .......... 10
来源：http://gh.huixinmuqiang.cn

------------------------------------
来源：http://fz.gzmigu.cn

合计 ........... 2106 条
来源：http://zi.yuntaijiaju.cn

按章节统计：
来源：http://ak.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ct.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hy.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pk.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nc.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ky.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bb.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tt.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nc.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kw.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jh.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xa.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cn.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rg.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wp.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hm.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://un.yuexingan06.cn

Q SQL 专题                              90
来源：http://sd.colortex.cn

R Bash 专题                             80
来源：http://qf.yuexingan06.cn

S C / C++ 专题                          60
来源：http://js.szxytkj.cn

T 其他语言补充                          60
来源：http://hh.shtwfgs.cn

U 高频实用片段                         120
来源：http://gn.hahajie.cn

------------------------------------
来源：http://za.asd995.cn

合计                                  2106 条
来源：http://xj.521024.cn

--------------------------------------------------------------------------------
来源：http://py.hahajie.cn

使用提醒
来源：http://af.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ix.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ca.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://en.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vk.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zr.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qs.nicolike.cn

—— 文件结束 ——
来源：http://vh.shtwfgs.cn

================================================================================
来源：http://rl.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://sn.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://sk.haigaiapp.cn

================================================================================
来源：http://or.nicolike.cn

【收录内容】
来源：http://he.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fp.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://so.shxzskj.cn

SQL · Bash · C · C++
来源：http://yy.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ad.haigaiapp.cn

【使用说明】
来源：http://iq.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lu.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sr.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uv.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qq.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cg.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dv.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pr.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ub.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kq.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pt.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://we.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ai.shtwfgs.cn

【文件统计】
来源：http://gj.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tc.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ho.521024.cn

目  录
来源：http://ht.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mu.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rx.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ju.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bj.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eg.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xz.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yp.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iy.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qi.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wy.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://id.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dv.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ot.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iy.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://si.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vt.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://az.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dt.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ht.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qt.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://is.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uc.hahajie.cn

================================================================================
来源：http://iy.hnjuh.cn

A. 基础语法与类型
来源：http://rt.shxzukj.cn

================================================================================
来源：http://tf.shxzukj.cn

[A01] Hello World
来源：http://yu.asd995.cn

Py:   print("Hello, World!")
来源：http://dj.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://bk.colortex.cn

JS:   console.log("Hello, World!");
来源：http://oo.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://im.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://ia.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://hz.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://ap.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://um.shxzskj.cn

[A02] 变量声明与赋值
来源：http://eb.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nn.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nr.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tp.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://db.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://aa.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://to.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://se.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sp.bjjhwx.cn

[A03] 常量定义
来源：http://ny.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rs.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://xr.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://ap.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://tq.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://xr.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ck.nszjky.cn

Ruby: PI = 3.14159
来源：http://bi.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://uv.yuexingan06.cn

[A04] 判断变量类型
来源：http://nm.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sy.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ra.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ft.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://eu.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dw.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dm.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://er.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://vx.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://tl.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wh.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wi.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://em.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vy.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://oa.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://dx.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://pm.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://jp.szsharing.cn

[A06] 字符串转数字
来源：http://vl.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://re.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dk.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ot.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rl.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mj.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ed.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://om.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kf.hnjuh.cn

[A07] 数字转字符串
来源：http://qe.jctech888.com.cn

Py:   str(42)
来源：http://sk.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://rb.nszjky.cn

JS:   String(42); (42).toString()
来源：http://wn.yuexingan06.cn

TS:   String(42)
来源：http://uk.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sn.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://bj.nszjky.cn

Ruby: 42.to_s
来源：http://ym.bjjhwx.cn

C#:   42.ToString()
来源：http://uw.szsharing.cn

[A08] 取整与四舍五入
来源：http://so.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://de.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zx.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jv.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nm.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zy.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mg.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cy.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fn.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://ix.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lk.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hx.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ea.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ee.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iw.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dv.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wr.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hb.asd995.cn

[A10] 生成随机数
来源：http://nj.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://tg.newstarts.cn

PHP:  random_int(1, 100);
来源：http://lt.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kx.9csxet.cn


<!-- 参考信息 -->