代发 wailian999

[U69] PHP：PDO 预处理
来源：http://gc.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uc.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://zd.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rm.huanxung.cn

[U71] PHP：抛出异常
来源：http://hh.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://kp.hahajie.cn

[U72] PHP：写错误日志
来源：http://vi.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://rv.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://pj.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://kd.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://la.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://tx.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ta.hahajie.cn

composer require psr/container
来源：http://hp.asd995.cn

[U76] PHP：简单路由
来源：http://jw.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oa.nszjky.cn

[U77] PHP：模板渲染
来源：http://cf.asd995.cn

composer require twig/twig
来源：http://rc.panjiajie.cn

[U78] PHP：单元测试
来源：http://su.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://xb.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://nw.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://jn.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://sa.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nv.bjjhwx.cn

[U81] JS：初始化项目
来源：http://uw.9csxet.cn

npm init -y;  npm i express
来源：http://rl.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://ii.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bk.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://dc.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mc.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://vb.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vq.jianghongdianzi.cn

[U85] JS：可选链
来源：http://gs.yuntaijiaju.cn

a?.b?.c
来源：http://dz.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://vb.huanxung.cn

a ?? b
来源：http://sz.colortex.cn

[U87] JS：解构默认值
来源：http://nd.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://wv.lnxyls.cn

[U88] JS：对象展开合并
来源：http://ns.huixinmuqiang.cn

{ ...a, ...b }
来源：http://jl.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://sf.huanxung.cn

[...new Set(arr)]
来源：http://nx.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://ck.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://fm.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://lv.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cc.szsharing.cn

[U92] JS：深拷贝
来源：http://ft.shxzukj.cn

structuredClone(obj)
来源：http://li.shtwfgs.cn

[U93] JS：模板字符串
来源：http://th.newstarts.cn

`共 ${n} 条`
来源：http://qg.szsharing.cn

[U94] JS：箭头函数
来源：http://zs.bookmarksfly.cn

const double = x => x * 2;
来源：http://ae.gzmigu.cn

[U95] JS：Promise 包装
来源：http://xi.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://os.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://vn.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ql.szxytkj.cn

[U97] JS：并发请求
来源：http://nh.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://se.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://mn.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kw.szxytkj.cn

[U99] JS：事件监听
来源：http://au.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://sl.521024.cn

[U100] JS：DOM 查询
来源：http://lg.nicolike.cn

document.querySelector(".item")
来源：http://sp.nszjky.cn

[U101] JS：classList 操作
来源：http://xx.muxihuayi.cn

el.classList.toggle("active")
来源：http://tx.gzmigu.cn

[U102] JS：本地存储
来源：http://qw.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ei.szsharing.cn

[U103] JS：定时器
来源：http://yx.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rz.nicolike.cn

[U104] JS：防抖
来源：http://py.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pc.shxzukj.cn

[U105] JS：节流
来源：http://jj.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sq.huixiangedu.cn

[U106] JS：日期格式化
来源：http://mf.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yr.huanxung.cn

[U107] JS：数字千分位
来源：http://qh.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nb.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://kw.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qw.bookmarksfly.cn

[U109] JS：数组分组
来源：http://su.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://bj.shxzukj.cn

[U110] JS：数组分块
来源：http://mo.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jl.nicolike.cn

[U111] JS：对象转 Map
来源：http://dy.lnxyls.cn

new Map(Object.entries(obj))
来源：http://jc.shxzskj.cn

[U112] JS：字符串补位
来源：http://pl.nszjky.cn

"7".padStart(3, "0")
来源：http://dw.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://zd.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://ys.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://ei.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tr.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ev.huanxung.cn

crypto.randomUUID()
来源：http://uk.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://vw.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://wh.colortex.cn

[U117] JS：单元测试
来源：http://dp.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://ke.nszjky.cn

[U118] JS：开发服务器
来源：http://ig.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://ns.wgjwhj.cn

[U119] JS：生产构建
来源：http://mb.9csxet.cn

npx vite build
来源：http://ts.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://xu.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://fm.bookmarksfly.cn

================================================================================
来源：http://ti.muxihuayi.cn

统计汇总
来源：http://sp.haigaiapp.cn

================================================================================
来源：http://hq.haigaiapp.cn

按语言统计（条）：
来源：http://xa.shtwfgs.cn

Python ......... 252
来源：http://gw.hnjuh.cn

PHP ............ 252
来源：http://jy.szxytkj.cn

JavaScript ..... 252
来源：http://wn.panjiajie.cn

TypeScript ..... 212
来源：http://uu.colortex.cn

Java ........... 212
来源：http://bx.newstarts.cn

Go ............. 212
来源：http://pi.bookmarksfly.cn

Ruby ........... 212
来源：http://wl.shxzskj.cn

C# ............. 212
来源：http://pt.newstarts.cn

C .............. 30
来源：http://zd.wgjwhj.cn

C++ ............ 30
来源：http://pr.haigaiapp.cn

SQL ............ 90
来源：http://kh.hahajie.cn

Bash ........... 80
来源：http://sh.panjiajie.cn

Kotlin ......... 15
来源：http://qj.huixinmuqiang.cn

Swift .......... 15
来源：http://ad.bjjhwx.cn

Lua ............ 10
来源：http://td.panjiajie.cn

Perl ........... 10
来源：http://qx.panjiajie.cn

Scala .......... 10
来源：http://td.hnjuh.cn

------------------------------------
来源：http://pt.lnxyls.cn

合计 ........... 2106 条
来源：http://jv.521024.cn

按章节统计：
来源：http://ti.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zi.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ol.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gt.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zl.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nq.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cq.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fh.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ot.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://du.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sc.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://si.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cf.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lr.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jr.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hj.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://to.szsharing.cn

Q SQL 专题                              90
来源：http://zn.bookmarksfly.cn

R Bash 专题                             80
来源：http://fu.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://az.jctech888.com.cn

T 其他语言补充                          60
来源：http://fw.jctech888.com.cn

U 高频实用片段                         120
来源：http://oz.hahajie.cn

------------------------------------
来源：http://do.jctech888.com.cn

合计                                  2106 条
来源：http://qv.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://cg.jianghongdianzi.cn

使用提醒
来源：http://re.hahajie.cn

--------------------------------------------------------------------------------
来源：http://qf.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vo.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qp.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fn.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ji.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zr.jctech888.com.cn

—— 文件结束 ——
来源：http://pe.muxihuayi.cn

================================================================================
来源：http://rl.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://hw.szsharing.cn

Common Programming Examples Cheat Book
来源：http://lf.bookmarksfly.cn

================================================================================
来源：http://ql.lnxyls.cn

【收录内容】
来源：http://ia.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://aa.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ti.lnxyls.cn

SQL · Bash · C · C++
来源：http://ex.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://am.shtwfgs.cn

【使用说明】
来源：http://jh.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wp.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ja.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xx.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oy.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rv.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pq.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iz.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nq.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qw.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tt.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bl.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oe.hnjuh.cn

【文件统计】
来源：http://lm.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ps.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ct.521024.cn

目  录
来源：http://zr.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://rk.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ya.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nt.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yy.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ed.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://os.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cw.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wz.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://te.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tr.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ah.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jg.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oa.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pj.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gn.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jv.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://to.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bh.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gp.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xq.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://om.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bw.huixinmuqiang.cn

================================================================================
来源：http://hg.huixinmuqiang.cn

A. 基础语法与类型
来源：http://mh.9csxet.cn

================================================================================
来源：http://dc.muxihuayi.cn

[A01] Hello World
来源：http://iu.colortex.cn

Py:   print("Hello, World!")
来源：http://rl.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://rj.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://ek.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ws.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://ra.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://mc.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://fz.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rn.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://ek.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uv.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rk.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ly.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ot.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://zy.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://ho.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://jk.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qf.hahajie.cn

[A03] 常量定义
来源：http://ti.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vv.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://ol.nicolike.cn

JS:   const PI = 3.14159;
来源：http://ch.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://ib.colortex.cn

Java: static final double PI = 3.14159;
来源：http://lh.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://pp.shxzukj.cn

Ruby: PI = 3.14159
来源：http://ki.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://ws.szxytkj.cn

[A04] 判断变量类型
来源：http://ty.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rf.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zi.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qo.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://as.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zg.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fm.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dk.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://lg.szxytkj.cn

[A05] 整数除法与取模
来源：http://vg.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sc.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qu.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://np.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rp.521024.cn

Java: 7 / 2; 7 % 2
来源：http://ba.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://hf.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://mg.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://qg.colortex.cn

[A06] 字符串转数字
来源：http://cb.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://ob.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uk.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jp.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lq.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ts.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yv.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eg.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lo.wgjwhj.cn

[A07] 数字转字符串
来源：http://pa.lnxyls.cn

Py:   str(42)
来源：http://ii.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://xa.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://kz.yuntaijiaju.cn

TS:   String(42)
来源：http://vd.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zh.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://wn.521024.cn

Ruby: 42.to_s
来源：http://oy.newstarts.cn

C#:   42.ToString()
来源：http://yg.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://ud.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://li.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ki.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ek.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://io.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kh.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hk.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ig.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ol.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://hj.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qo.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dl.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mr.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pf.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lx.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tc.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yx.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tc.haigaiapp.cn

[A10] 生成随机数
来源：http://mk.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ll.nicolike.cn

PHP:  random_int(1, 100);
来源：http://vx.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pu.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pq.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ri.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fz.shxzskj.cn

Ruby: rand(1..100)
来源：http://gn.chemitech.net.cn


<!-- 参考信息 -->