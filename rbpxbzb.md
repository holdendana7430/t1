代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hl.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jx.nicolike.cn

[U70] PHP：PDO 事务
来源：http://nz.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kz.newstarts.cn

[U71] PHP：抛出异常
来源：http://by.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://pw.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://kl.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://kx.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://bb.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://eu.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://cr.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://ow.nicolike.cn

[U75] PHP：依赖注入
来源：http://ob.bookmarksfly.cn

composer require psr/container
来源：http://js.asd995.cn

[U76] PHP：简单路由
来源：http://zt.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lg.gzmigu.cn

[U77] PHP：模板渲染
来源：http://xn.bookmarksfly.cn

composer require twig/twig
来源：http://mr.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://wq.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://re.jctech888.com.cn

[U79] PHP：静态分析
来源：http://am.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://gg.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://wb.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aw.jctech888.com.cn

[U81] JS：初始化项目
来源：http://cy.haigaiapp.cn

npm init -y;  npm i express
来源：http://hl.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://ip.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lp.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://kx.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vv.521024.cn

[U84] JS：CommonJS 写法
来源：http://fr.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://id.shxzukj.cn

[U85] JS：可选链
来源：http://wt.jctech888.com.cn

a?.b?.c
来源：http://ja.muxihuayi.cn

[U86] JS：空值合并
来源：http://li.colortex.cn

a ?? b
来源：http://rh.gzmigu.cn

[U87] JS：解构默认值
来源：http://tt.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://kz.shxzukj.cn

[U88] JS：对象展开合并
来源：http://xe.9csxet.cn

{ ...a, ...b }
来源：http://ok.asd995.cn

[U89] JS：数组去重
来源：http://nv.jianghongdianzi.cn

[...new Set(arr)]
来源：http://op.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://ms.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://xv.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://jv.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ub.yuexingan06.cn

[U92] JS：深拷贝
来源：http://mk.yuexingan06.cn

structuredClone(obj)
来源：http://yp.521024.cn

[U93] JS：模板字符串
来源：http://ps.panjiajie.cn

`共 ${n} 条`
来源：http://rm.huanxung.cn

[U94] JS：箭头函数
来源：http://ip.lnxyls.cn

const double = x => x * 2;
来源：http://tp.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://kg.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://gl.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://wg.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ic.huanxung.cn

[U97] JS：并发请求
来源：http://tj.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://re.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://vi.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ml.newstarts.cn

[U99] JS：事件监听
来源：http://ad.newstarts.cn

el.addEventListener("click", e => {})
来源：http://iw.nszjky.cn

[U100] JS：DOM 查询
来源：http://yo.shxzskj.cn

document.querySelector(".item")
来源：http://zg.521024.cn

[U101] JS：classList 操作
来源：http://eq.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://al.shxzukj.cn

[U102] JS：本地存储
来源：http://oo.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fg.haigaiapp.cn

[U103] JS：定时器
来源：http://rl.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oo.gzmigu.cn

[U104] JS：防抖
来源：http://az.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ze.shtwfgs.cn

[U105] JS：节流
来源：http://xp.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ks.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://iw.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yl.colortex.cn

[U107] JS：数字千分位
来源：http://rn.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://by.wgjwhj.cn

[U108] JS：随机整数
来源：http://uy.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uh.szsharing.cn

[U109] JS：数组分组
来源：http://wi.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://mx.wgjwhj.cn

[U110] JS：数组分块
来源：http://ht.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cw.newstarts.cn

[U111] JS：对象转 Map
来源：http://zd.nicolike.cn

new Map(Object.entries(obj))
来源：http://zk.hahajie.cn

[U112] JS：字符串补位
来源：http://pc.haigaiapp.cn

"7".padStart(3, "0")
来源：http://ck.shxzukj.cn

[U113] JS：正则替换全部
来源：http://es.shxzukj.cn

s.replaceAll("a", "b")
来源：http://qi.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://zf.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://el.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://cx.9csxet.cn

crypto.randomUUID()
来源：http://bl.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://mf.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://cu.panjiajie.cn

[U117] JS：单元测试
来源：http://hs.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://en.huixiangedu.cn

[U118] JS：开发服务器
来源：http://tt.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://kg.yuexingan06.cn

[U119] JS：生产构建
来源：http://hi.jianghongdianzi.cn

npx vite build
来源：http://aw.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://do.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://eh.newstarts.cn

================================================================================
来源：http://bj.9csxet.cn

统计汇总
来源：http://lp.chemitech.net.cn

================================================================================
来源：http://jz.yuntaijiaju.cn

按语言统计（条）：
来源：http://qs.colortex.cn

Python ......... 252
来源：http://vu.muxihuayi.cn

PHP ............ 252
来源：http://dt.hnjuh.cn

JavaScript ..... 252
来源：http://sv.jianghongdianzi.cn

TypeScript ..... 212
来源：http://kj.haigaiapp.cn

Java ........... 212
来源：http://qi.colortex.cn

Go ............. 212
来源：http://no.shxzukj.cn

Ruby ........... 212
来源：http://uu.hahajie.cn

C# ............. 212
来源：http://gt.wgjwhj.cn

C .............. 30
来源：http://pu.haigaiapp.cn

C++ ............ 30
来源：http://uy.9csxet.cn

SQL ............ 90
来源：http://yz.nicolike.cn

Bash ........... 80
来源：http://ez.huixiangedu.cn

Kotlin ......... 15
来源：http://nj.shtwfgs.cn

Swift .......... 15
来源：http://rf.huanxung.cn

Lua ............ 10
来源：http://bp.szxytkj.cn

Perl ........... 10
来源：http://kl.asd995.cn

Scala .......... 10
来源：http://ao.521024.cn

------------------------------------
来源：http://lr.lnxyls.cn

合计 ........... 2106 条
来源：http://fy.yuexingan06.cn

按章节统计：
来源：http://gm.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bk.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xk.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sw.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oq.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vy.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fj.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sh.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cy.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gu.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gb.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pk.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://un.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fb.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gj.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yx.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qj.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://xh.9csxet.cn

R Bash 专题                             80
来源：http://vz.9csxet.cn

S C / C++ 专题                          60
来源：http://gf.haigaiapp.cn

T 其他语言补充                          60
来源：http://pm.hahajie.cn

U 高频实用片段                         120
来源：http://wn.wgjwhj.cn

------------------------------------
来源：http://uh.shxzukj.cn

合计                                  2106 条
来源：http://az.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://yg.chemitech.net.cn

使用提醒
来源：http://tj.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://xv.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lg.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://es.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kg.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lm.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qx.bookmarksfly.cn

—— 文件结束 ——
来源：http://wr.nszjky.cn

================================================================================
来源：http://cw.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://kg.521024.cn

Common Programming Examples Cheat Book
来源：http://he.jianghongdianzi.cn

================================================================================
来源：http://vr.9csxet.cn

【收录内容】
来源：http://wy.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gt.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hc.muxihuayi.cn

SQL · Bash · C · C++
来源：http://pk.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mg.gzmigu.cn

【使用说明】
来源：http://cg.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ki.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mj.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hb.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rg.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://en.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hq.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jm.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zy.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ld.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://li.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ya.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tp.szxytkj.cn

【文件统计】
来源：http://nn.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zt.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://lc.colortex.cn

目  录
来源：http://wp.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://na.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kd.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eg.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jv.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://di.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vk.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bk.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vl.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jc.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jo.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vq.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kr.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xq.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dc.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nj.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lo.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oq.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://an.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nz.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jm.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qw.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oi.yuntaijiaju.cn

================================================================================
来源：http://vm.jctech888.com.cn

A. 基础语法与类型
来源：http://yn.9csxet.cn

================================================================================
来源：http://nn.newstarts.cn

[A01] Hello World
来源：http://zl.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://ff.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://qt.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://vp.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gu.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://ln.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://cs.colortex.cn

Ruby: puts "Hello, World!"
来源：http://gz.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iy.shxzukj.cn

[A02] 变量声明与赋值
来源：http://df.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ua.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ev.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jl.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ji.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://gi.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://no.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://cv.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gm.szxytkj.cn

[A03] 常量定义
来源：http://iw.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gu.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://ac.9csxet.cn

JS:   const PI = 3.14159;
来源：http://dw.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://gq.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://qu.huanxung.cn

Go:   const PI = 3.14159
来源：http://ci.9csxet.cn

Ruby: PI = 3.14159
来源：http://iq.521024.cn

C#:   const double PI = 3.14159;
来源：http://zy.huanxung.cn

[A04] 判断变量类型
来源：http://bg.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oe.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://on.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://va.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://jr.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zb.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vh.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ho.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://em.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://io.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://na.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nn.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vc.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dx.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://ay.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://ld.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ta.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://zc.lnxyls.cn

[A06] 字符串转数字
来源：http://gn.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://us.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ml.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qf.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ij.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://al.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lz.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nq.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gc.nicolike.cn

[A07] 数字转字符串
来源：http://xm.szsharing.cn

Py:   str(42)
来源：http://hw.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://oq.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://oa.asd995.cn

TS:   String(42)
来源：http://og.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nr.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://bo.bookmarksfly.cn

Ruby: 42.to_s
来源：http://qg.shtwfgs.cn

C#:   42.ToString()
来源：http://kf.asd995.cn

[A08] 取整与四舍五入
来源：http://zw.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wj.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ys.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mu.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mm.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sp.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ye.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gu.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://li.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://ar.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eb.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://go.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://me.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hy.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ro.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rm.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bo.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lf.bjjhwx.cn

[A10] 生成随机数
来源：http://no.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://hx.colortex.cn

PHP:  random_int(1, 100);
来源：http://ux.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pw.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fw.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://cv.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jf.asd995.cn

Ruby: rand(1..100)
来源：http://tk.jianghongdianzi.cn


<!-- 参考信息 -->