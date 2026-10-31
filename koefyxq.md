代发 wailian999

[U67] PHP：处理文件上传
来源：http://xc.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eh.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://el.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dt.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://uz.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qt.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://be.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xi.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://nm.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://ui.hahajie.cn

[U72] PHP：写错误日志
来源：http://gv.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://hj.521024.cn

[U73] PHP：读取 ini 配置
来源：http://cq.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://yp.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://ny.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://zk.szsharing.cn

[U75] PHP：依赖注入
来源：http://hl.nicolike.cn

composer require psr/container
来源：http://dq.nicolike.cn

[U76] PHP：简单路由
来源：http://df.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sk.newstarts.cn

[U77] PHP：模板渲染
来源：http://ps.hnjuh.cn

composer require twig/twig
来源：http://gd.hnjuh.cn

[U78] PHP：单元测试
来源：http://cg.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://wt.colortex.cn

[U79] PHP：静态分析
来源：http://qv.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://rv.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://gl.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kp.shxzukj.cn

[U81] JS：初始化项目
来源：http://mh.bookmarksfly.cn

npm init -y;  npm i express
来源：http://dn.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://xj.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sk.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://gv.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yl.colortex.cn

[U84] JS：CommonJS 写法
来源：http://mt.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pc.yuntaijiaju.cn

[U85] JS：可选链
来源：http://mg.gzmigu.cn

a?.b?.c
来源：http://wh.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://rb.panjiajie.cn

a ?? b
来源：http://cx.nicolike.cn

[U87] JS：解构默认值
来源：http://qq.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://bd.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://cw.9csxet.cn

{ ...a, ...b }
来源：http://if.nszjky.cn

[U89] JS：数组去重
来源：http://vo.521024.cn

[...new Set(arr)]
来源：http://iu.shxzukj.cn

[U90] JS：数字数组排序
来源：http://df.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://rp.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ix.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jv.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://xo.panjiajie.cn

structuredClone(obj)
来源：http://df.colortex.cn

[U93] JS：模板字符串
来源：http://jg.newstarts.cn

`共 ${n} 条`
来源：http://zg.yuexingan06.cn

[U94] JS：箭头函数
来源：http://vj.asd995.cn

const double = x => x * 2;
来源：http://lh.newstarts.cn

[U95] JS：Promise 包装
来源：http://je.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://el.szsharing.cn

[U96] JS：async/await 与异常
来源：http://pr.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ib.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://pt.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://yk.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://by.hnjuh.cn

[U99] JS：事件监听
来源：http://bn.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://xw.lnxyls.cn

[U100] JS：DOM 查询
来源：http://mw.asd995.cn

document.querySelector(".item")
来源：http://yt.hahajie.cn

[U101] JS：classList 操作
来源：http://ex.chemitech.net.cn

el.classList.toggle("active")
来源：http://cp.huanxung.cn

[U102] JS：本地存储
来源：http://ks.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ru.hahajie.cn

[U103] JS：定时器
来源：http://lm.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://la.chemitech.net.cn

[U104] JS：防抖
来源：http://xk.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gz.huanxung.cn

[U105] JS：节流
来源：http://xv.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://va.newstarts.cn

[U106] JS：日期格式化
来源：http://ux.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dr.colortex.cn

[U107] JS：数字千分位
来源：http://rr.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fw.szxytkj.cn

[U108] JS：随机整数
来源：http://sj.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mq.szxytkj.cn

[U109] JS：数组分组
来源：http://he.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://iq.bjjhwx.cn

[U110] JS：数组分块
来源：http://bz.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ox.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://sp.gzmigu.cn

new Map(Object.entries(obj))
来源：http://vm.hahajie.cn

[U112] JS：字符串补位
来源：http://ma.muxihuayi.cn

"7".padStart(3, "0")
来源：http://hj.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ld.shxzukj.cn

s.replaceAll("a", "b")
来源：http://nc.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://ej.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oq.newstarts.cn

[U115] JS：生成 UUID
来源：http://nd.huixiangedu.cn

crypto.randomUUID()
来源：http://cs.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://xl.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://wu.gzmigu.cn

[U117] JS：单元测试
来源：http://iz.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://tl.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://gx.colortex.cn

npm i -D vite;  npx vite
来源：http://tp.shxzskj.cn

[U119] JS：生产构建
来源：http://mp.bookmarksfly.cn

npx vite build
来源：http://br.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://jd.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://me.wgjwhj.cn

================================================================================
来源：http://or.panjiajie.cn

统计汇总
来源：http://th.jianghongdianzi.cn

================================================================================
来源：http://mw.nszjky.cn

按语言统计（条）：
来源：http://pf.yuntaijiaju.cn

Python ......... 252
来源：http://vd.newstarts.cn

PHP ............ 252
来源：http://ka.nicolike.cn

JavaScript ..... 252
来源：http://uf.szsharing.cn

TypeScript ..... 212
来源：http://cf.szsharing.cn

Java ........... 212
来源：http://ge.asd995.cn

Go ............. 212
来源：http://rn.shxzukj.cn

Ruby ........... 212
来源：http://iw.asd995.cn

C# ............. 212
来源：http://an.521024.cn

C .............. 30
来源：http://zf.9csxet.cn

C++ ............ 30
来源：http://ds.wgjwhj.cn

SQL ............ 90
来源：http://pg.521024.cn

Bash ........... 80
来源：http://my.colortex.cn

Kotlin ......... 15
来源：http://dn.bjjhwx.cn

Swift .......... 15
来源：http://yi.nicolike.cn

Lua ............ 10
来源：http://nq.hnjuh.cn

Perl ........... 10
来源：http://zh.hnjuh.cn

Scala .......... 10
来源：http://kw.szxytkj.cn

------------------------------------
来源：http://hg.yuexingan06.cn

合计 ........... 2106 条
来源：http://ar.yuexingan06.cn

按章节统计：
来源：http://bp.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vh.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ov.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aj.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://le.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://im.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mg.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tm.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rs.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ym.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://el.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sm.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jy.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gu.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lk.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ji.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gx.jctech888.com.cn

Q SQL 专题                              90
来源：http://ld.jianghongdianzi.cn

R Bash 专题                             80
来源：http://mb.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://ls.shxzukj.cn

T 其他语言补充                          60
来源：http://bb.szxytkj.cn

U 高频实用片段                         120
来源：http://qy.hnjuh.cn

------------------------------------
来源：http://ar.shxzskj.cn

合计                                  2106 条
来源：http://qt.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://bm.gzmigu.cn

使用提醒
来源：http://dr.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://io.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ru.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mg.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fh.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iv.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://by.yuntaijiaju.cn

—— 文件结束 ——
来源：http://el.hahajie.cn

================================================================================
来源：http://ba.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://sm.huanxung.cn

Common Programming Examples Cheat Book
来源：http://lg.yuntaijiaju.cn

================================================================================
来源：http://vv.chemitech.net.cn

【收录内容】
来源：http://ju.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://te.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ew.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://ex.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tz.jctech888.com.cn

【使用说明】
来源：http://pc.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ot.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ka.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eu.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://we.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lc.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://za.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vx.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jb.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cg.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lz.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xo.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fh.yuntaijiaju.cn

【文件统计】
来源：http://he.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mm.colortex.cn

--------------------------------------------------------------------------------
来源：http://hy.muxihuayi.cn

目  录
来源：http://kc.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://gx.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ui.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ar.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fm.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kx.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ud.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fp.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://an.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ty.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nf.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://co.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ip.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oz.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://og.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ou.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zg.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iu.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ow.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sj.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://db.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jp.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cf.521024.cn

================================================================================
来源：http://dl.bookmarksfly.cn

A. 基础语法与类型
来源：http://kf.bjjhwx.cn

================================================================================
来源：http://xs.huixinmuqiang.cn

[A01] Hello World
来源：http://vr.hnjuh.cn

Py:   print("Hello, World!")
来源：http://io.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://oi.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://jf.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://je.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://fa.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://bt.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://hp.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://we.newstarts.cn

[A02] 变量声明与赋值
来源：http://qk.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sx.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eu.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yy.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yq.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://sx.521024.cn

Go:   name := "Alex"; age := 20
来源：http://yx.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://um.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jm.huixiangedu.cn

[A03] 常量定义
来源：http://cu.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ej.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://hw.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://rz.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://ua.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://vj.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://wt.lnxyls.cn

Ruby: PI = 3.14159
来源：http://ds.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://uo.9csxet.cn

[A04] 判断变量类型
来源：http://lc.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ga.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ma.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rb.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://ef.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cd.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gk.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qz.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://pm.szsharing.cn

[A05] 整数除法与取模
来源：http://vw.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bv.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wo.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zs.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pc.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://on.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://kw.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://oy.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://ku.colortex.cn

[A06] 字符串转数字
来源：http://kg.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://nf.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hn.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ac.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vy.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ma.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vy.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fm.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://te.jctech888.com.cn

[A07] 数字转字符串
来源：http://lp.shtwfgs.cn

Py:   str(42)
来源：http://jm.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://vw.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://px.bjjhwx.cn

TS:   String(42)
来源：http://pd.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://je.521024.cn

Go:   strconv.Itoa(42)
来源：http://rc.hnjuh.cn

Ruby: 42.to_s
来源：http://ek.lnxyls.cn

C#:   42.ToString()
来源：http://hv.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://he.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zz.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://op.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mr.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bz.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qn.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wl.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ay.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ro.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://wf.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gv.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pg.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://es.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bd.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xi.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oq.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fp.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vb.huanxung.cn

[A10] 生成随机数
来源：http://rc.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://rn.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://jt.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wv.yuntaijiaju.cn


<!-- 参考信息 -->