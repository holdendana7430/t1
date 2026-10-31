代发 wailian999

[U69] PHP：PDO 预处理
来源：http://vn.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qk.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ua.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://be.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ny.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://cc.521024.cn

[U72] PHP：写错误日志
来源：http://nu.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://qp.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://sv.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://ek.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://uw.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://ur.nicolike.cn

[U75] PHP：依赖注入
来源：http://jz.huixinmuqiang.cn

composer require psr/container
来源：http://gd.hnjuh.cn

[U76] PHP：简单路由
来源：http://jt.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pr.asd995.cn

[U77] PHP：模板渲染
来源：http://um.szxytkj.cn

composer require twig/twig
来源：http://ba.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://gp.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://iq.lnxyls.cn

[U79] PHP：静态分析
来源：http://yv.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://kn.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://kj.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zt.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://ga.yuexingan06.cn

npm init -y;  npm i express
来源：http://wv.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://lo.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oh.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://dt.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dr.521024.cn

[U84] JS：CommonJS 写法
来源：http://vw.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uf.lnxyls.cn

[U85] JS：可选链
来源：http://kh.yuntaijiaju.cn

a?.b?.c
来源：http://bq.haigaiapp.cn

[U86] JS：空值合并
来源：http://ag.szxytkj.cn

a ?? b
来源：http://fx.9csxet.cn

[U87] JS：解构默认值
来源：http://tv.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://wa.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://sc.jctech888.com.cn

{ ...a, ...b }
来源：http://rm.wgjwhj.cn

[U89] JS：数组去重
来源：http://er.yuntaijiaju.cn

[...new Set(arr)]
来源：http://aw.nicolike.cn

[U90] JS：数字数组排序
来源：http://xw.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://iq.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://ot.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://co.nszjky.cn

[U92] JS：深拷贝
来源：http://vf.haigaiapp.cn

structuredClone(obj)
来源：http://fk.bjjhwx.cn

[U93] JS：模板字符串
来源：http://zr.szsharing.cn

`共 ${n} 条`
来源：http://jq.muxihuayi.cn

[U94] JS：箭头函数
来源：http://ov.wgjwhj.cn

const double = x => x * 2;
来源：http://dv.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://ig.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://go.newstarts.cn

[U96] JS：async/await 与异常
来源：http://bj.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yb.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://oc.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pn.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ej.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vo.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://qe.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://fh.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://ry.hnjuh.cn

document.querySelector(".item")
来源：http://fp.chemitech.net.cn

[U101] JS：classList 操作
来源：http://wr.asd995.cn

el.classList.toggle("active")
来源：http://ln.9csxet.cn

[U102] JS：本地存储
来源：http://nq.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yn.lnxyls.cn

[U103] JS：定时器
来源：http://em.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://da.wgjwhj.cn

[U104] JS：防抖
来源：http://po.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uv.bjjhwx.cn

[U105] JS：节流
来源：http://bl.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xd.muxihuayi.cn

[U106] JS：日期格式化
来源：http://pe.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://it.asd995.cn

[U107] JS：数字千分位
来源：http://hz.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ab.9csxet.cn

[U108] JS：随机整数
来源：http://kq.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ez.gzmigu.cn

[U109] JS：数组分组
来源：http://fl.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://bb.9csxet.cn

[U110] JS：数组分块
来源：http://zu.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bh.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://wc.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ae.nicolike.cn

[U112] JS：字符串补位
来源：http://hr.shxzukj.cn

"7".padStart(3, "0")
来源：http://ck.szxytkj.cn

[U113] JS：正则替换全部
来源：http://gt.huanxung.cn

s.replaceAll("a", "b")
来源：http://gh.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://fq.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gl.521024.cn

[U115] JS：生成 UUID
来源：http://xf.yuexingan06.cn

crypto.randomUUID()
来源：http://va.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://cm.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://bd.huixiangedu.cn

[U117] JS：单元测试
来源：http://ad.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://xv.chemitech.net.cn

[U118] JS：开发服务器
来源：http://tk.521024.cn

npm i -D vite;  npx vite
来源：http://gg.muxihuayi.cn

[U119] JS：生产构建
来源：http://el.wgjwhj.cn

npx vite build
来源：http://ir.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://dy.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://vf.gzmigu.cn

================================================================================
来源：http://bi.huixiangedu.cn

统计汇总
来源：http://py.shtwfgs.cn

================================================================================
来源：http://oi.shxzskj.cn

按语言统计（条）：
来源：http://ru.asd995.cn

Python ......... 252
来源：http://ip.nszjky.cn

PHP ............ 252
来源：http://xt.panjiajie.cn

JavaScript ..... 252
来源：http://rr.newstarts.cn

TypeScript ..... 212
来源：http://kk.hnjuh.cn

Java ........... 212
来源：http://fk.jctech888.com.cn

Go ............. 212
来源：http://ld.gzmigu.cn

Ruby ........... 212
来源：http://te.nszjky.cn

C# ............. 212
来源：http://kr.muxihuayi.cn

C .............. 30
来源：http://fd.szsharing.cn

C++ ............ 30
来源：http://gx.hahajie.cn

SQL ............ 90
来源：http://ok.wgjwhj.cn

Bash ........... 80
来源：http://go.muxihuayi.cn

Kotlin ......... 15
来源：http://tk.shxzskj.cn

Swift .......... 15
来源：http://kh.9csxet.cn

Lua ............ 10
来源：http://gk.nszjky.cn

Perl ........... 10
来源：http://ln.szsharing.cn

Scala .......... 10
来源：http://lw.jianghongdianzi.cn

------------------------------------
来源：http://wg.hahajie.cn

合计 ........... 2106 条
来源：http://zl.haigaiapp.cn

按章节统计：
来源：http://hu.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ig.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wa.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yw.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bu.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ns.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kc.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qr.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iv.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uw.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lc.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ei.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qx.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ot.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wa.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cs.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ya.bookmarksfly.cn

Q SQL 专题                              90
来源：http://pd.bookmarksfly.cn

R Bash 专题                             80
来源：http://fo.szsharing.cn

S C / C++ 专题                          60
来源：http://wa.521024.cn

T 其他语言补充                          60
来源：http://at.nicolike.cn

U 高频实用片段                         120
来源：http://if.jianghongdianzi.cn

------------------------------------
来源：http://zw.asd995.cn

合计                                  2106 条
来源：http://st.colortex.cn

--------------------------------------------------------------------------------
来源：http://kf.yuexingan06.cn

使用提醒
来源：http://gu.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://il.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vd.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bc.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jq.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ux.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yp.muxihuayi.cn

—— 文件结束 ——
来源：http://pm.shxzskj.cn

================================================================================
来源：http://ss.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://ce.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://ux.hahajie.cn

================================================================================
来源：http://dy.huixinmuqiang.cn

【收录内容】
来源：http://ag.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bp.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ls.gzmigu.cn

SQL · Bash · C · C++
来源：http://en.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aw.jianghongdianzi.cn

【使用说明】
来源：http://pc.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ey.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ug.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iq.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://je.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lu.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ox.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nt.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://up.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ea.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kq.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yo.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://im.hnjuh.cn

【文件统计】
来源：http://hj.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ge.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://us.asd995.cn

目  录
来源：http://oo.colortex.cn

--------------------------------------------------------------------------------
来源：http://ew.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aj.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gr.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ob.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gd.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xb.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vh.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xa.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qr.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wo.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mj.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mu.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ea.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cm.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hs.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kk.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yg.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vx.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://of.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zk.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jj.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rq.9csxet.cn

================================================================================
来源：http://zo.gzmigu.cn

A. 基础语法与类型
来源：http://fc.chemitech.net.cn

================================================================================
来源：http://rn.asd995.cn

[A01] Hello World
来源：http://qo.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ql.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://qm.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://ta.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jv.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://ls.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://nv.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://xa.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fm.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://tr.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yy.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fw.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rv.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qm.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://kz.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://gw.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://io.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xw.huixinmuqiang.cn

[A03] 常量定义
来源：http://zd.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fg.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://cy.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://tu.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ms.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://qs.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://em.nszjky.cn

Ruby: PI = 3.14159
来源：http://hr.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://zb.colortex.cn

[A04] 判断变量类型
来源：http://kw.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://em.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ke.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://be.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://mw.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ym.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qa.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oy.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://tc.shxzskj.cn

[A05] 整数除法与取模
来源：http://wr.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xc.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nc.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ga.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vb.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://la.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://bd.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ah.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://yf.nicolike.cn

[A06] 字符串转数字
来源：http://rh.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://yw.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gw.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nd.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vq.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fr.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://em.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xx.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://me.chemitech.net.cn

[A07] 数字转字符串
来源：http://br.chemitech.net.cn

Py:   str(42)
来源：http://xd.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://cd.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://zh.shxzskj.cn

TS:   String(42)
来源：http://dk.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hb.521024.cn

Go:   strconv.Itoa(42)
来源：http://yy.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://xg.huixinmuqiang.cn

C#:   42.ToString()
来源：http://mr.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://kn.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://of.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jq.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://if.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://if.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://me.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ca.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gw.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yx.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://vy.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rh.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ok.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ax.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fn.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zf.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://it.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lb.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://de.haigaiapp.cn

[A10] 生成随机数
来源：http://kl.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://qa.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://zl.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dc.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ay.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://bu.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qe.gzmigu.cn

Ruby: rand(1..100)
来源：http://qu.521024.cn


<!-- 参考信息 -->