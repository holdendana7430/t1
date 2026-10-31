代发 wailian999

[U67] PHP：处理文件上传
来源：http://yu.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://if.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://xe.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nt.asd995.cn

[U69] PHP：PDO 预处理
来源：http://fj.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ib.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://iy.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uv.huanxung.cn

[U71] PHP：抛出异常
来源：http://xu.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://qe.hnjuh.cn

[U72] PHP：写错误日志
来源：http://vk.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://ss.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://ey.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://pi.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://sy.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://tn.shxzskj.cn

[U75] PHP：依赖注入
来源：http://id.chemitech.net.cn

composer require psr/container
来源：http://fw.bjjhwx.cn

[U76] PHP：简单路由
来源：http://ew.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mf.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://qe.gzmigu.cn

composer require twig/twig
来源：http://na.szsharing.cn

[U78] PHP：单元测试
来源：http://lr.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://ua.shxzskj.cn

[U79] PHP：静态分析
来源：http://wm.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://ze.hahajie.cn

[U80] PHP：代码规范修复
来源：http://jn.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xh.shtwfgs.cn

[U81] JS：初始化项目
来源：http://eq.9csxet.cn

npm init -y;  npm i express
来源：http://mc.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://ii.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xl.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://bn.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ex.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://zi.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jd.gzmigu.cn

[U85] JS：可选链
来源：http://pu.nicolike.cn

a?.b?.c
来源：http://tc.nicolike.cn

[U86] JS：空值合并
来源：http://pl.bjjhwx.cn

a ?? b
来源：http://wv.nicolike.cn

[U87] JS：解构默认值
来源：http://se.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://gk.szxytkj.cn

[U88] JS：对象展开合并
来源：http://hi.521024.cn

{ ...a, ...b }
来源：http://wj.jctech888.com.cn

[U89] JS：数组去重
来源：http://md.asd995.cn

[...new Set(arr)]
来源：http://oh.szsharing.cn

[U90] JS：数字数组排序
来源：http://in.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://cg.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://kl.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kf.521024.cn

[U92] JS：深拷贝
来源：http://fi.asd995.cn

structuredClone(obj)
来源：http://gz.bjjhwx.cn

[U93] JS：模板字符串
来源：http://gi.shxzskj.cn

`共 ${n} 条`
来源：http://cb.nicolike.cn

[U94] JS：箭头函数
来源：http://nd.szsharing.cn

const double = x => x * 2;
来源：http://kn.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ie.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://to.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://ms.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kf.newstarts.cn

[U97] JS：并发请求
来源：http://dj.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://ha.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qx.panjiajie.cn

[U99] JS：事件监听
来源：http://ch.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://iq.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://rl.huixinmuqiang.cn

document.querySelector(".item")
来源：http://su.521024.cn

[U101] JS：classList 操作
来源：http://xa.szxytkj.cn

el.classList.toggle("active")
来源：http://ez.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://aw.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rm.yuntaijiaju.cn

[U103] JS：定时器
来源：http://in.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ez.szxytkj.cn

[U104] JS：防抖
来源：http://eg.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yv.bookmarksfly.cn

[U105] JS：节流
来源：http://hi.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pp.nicolike.cn

[U106] JS：日期格式化
来源：http://wp.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fm.shxzukj.cn

[U107] JS：数字千分位
来源：http://dl.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lz.hahajie.cn

[U108] JS：随机整数
来源：http://st.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://de.shtwfgs.cn

[U109] JS：数组分组
来源：http://jz.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ja.chemitech.net.cn

[U110] JS：数组分块
来源：http://yd.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rd.shxzskj.cn

[U111] JS：对象转 Map
来源：http://yg.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://vm.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://fp.nicolike.cn

"7".padStart(3, "0")
来源：http://vp.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ri.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://gp.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://xh.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uh.szxytkj.cn

[U115] JS：生成 UUID
来源：http://ke.huixiangedu.cn

crypto.randomUUID()
来源：http://li.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://ka.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://jz.huanxung.cn

[U117] JS：单元测试
来源：http://fi.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://ft.haigaiapp.cn

[U118] JS：开发服务器
来源：http://ms.gzmigu.cn

npm i -D vite;  npx vite
来源：http://hm.lnxyls.cn

[U119] JS：生产构建
来源：http://td.asd995.cn

npx vite build
来源：http://wd.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://kv.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://bi.nicolike.cn

================================================================================
来源：http://ok.bjjhwx.cn

统计汇总
来源：http://zw.shxzskj.cn

================================================================================
来源：http://av.muxihuayi.cn

按语言统计（条）：
来源：http://fw.9csxet.cn

Python ......... 252
来源：http://qr.521024.cn

PHP ............ 252
来源：http://ws.jctech888.com.cn

JavaScript ..... 252
来源：http://io.asd995.cn

TypeScript ..... 212
来源：http://bu.lnxyls.cn

Java ........... 212
来源：http://gs.asd995.cn

Go ............. 212
来源：http://xg.nszjky.cn

Ruby ........... 212
来源：http://dr.bookmarksfly.cn

C# ............. 212
来源：http://qq.jctech888.com.cn

C .............. 30
来源：http://tz.muxihuayi.cn

C++ ............ 30
来源：http://ox.panjiajie.cn

SQL ............ 90
来源：http://yx.nszjky.cn

Bash ........... 80
来源：http://gu.bookmarksfly.cn

Kotlin ......... 15
来源：http://ty.huixiangedu.cn

Swift .......... 15
来源：http://hn.asd995.cn

Lua ............ 10
来源：http://hy.nszjky.cn

Perl ........... 10
来源：http://rs.bookmarksfly.cn

Scala .......... 10
来源：http://wq.shxzukj.cn

------------------------------------
来源：http://im.hahajie.cn

合计 ........... 2106 条
来源：http://xs.shtwfgs.cn

按章节统计：
来源：http://kl.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bp.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rb.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uo.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oo.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dj.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pe.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lh.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ss.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qv.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cz.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yz.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rh.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wi.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gi.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aj.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dg.shtwfgs.cn

Q SQL 专题                              90
来源：http://bo.hnjuh.cn

R Bash 专题                             80
来源：http://vq.colortex.cn

S C / C++ 专题                          60
来源：http://vw.hnjuh.cn

T 其他语言补充                          60
来源：http://jn.jctech888.com.cn

U 高频实用片段                         120
来源：http://bb.panjiajie.cn

------------------------------------
来源：http://ky.hahajie.cn

合计                                  2106 条
来源：http://bm.colortex.cn

--------------------------------------------------------------------------------
来源：http://qe.yuntaijiaju.cn

使用提醒
来源：http://hm.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://tv.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zm.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tu.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://to.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oa.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eh.szsharing.cn

—— 文件结束 ——
来源：http://we.newstarts.cn

================================================================================
来源：http://bm.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://qc.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://fm.jianghongdianzi.cn

================================================================================
来源：http://sy.muxihuayi.cn

【收录内容】
来源：http://od.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fs.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xc.lnxyls.cn

SQL · Bash · C · C++
来源：http://ea.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vl.panjiajie.cn

【使用说明】
来源：http://tt.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://va.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ds.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xr.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ne.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cl.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eh.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://im.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ri.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qn.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://po.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jk.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fk.nicolike.cn

【文件统计】
来源：http://bz.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vt.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ln.panjiajie.cn

目  录
来源：http://my.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://qb.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ul.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fn.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xe.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yt.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rm.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vp.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nk.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nl.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://co.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kh.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ai.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qf.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vl.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lm.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yf.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gq.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qw.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ez.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pt.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dn.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://su.newstarts.cn

================================================================================
来源：http://my.shtwfgs.cn

A. 基础语法与类型
来源：http://as.shtwfgs.cn

================================================================================
来源：http://qp.jctech888.com.cn

[A01] Hello World
来源：http://gn.colortex.cn

Py:   print("Hello, World!")
来源：http://ty.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://pp.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://qt.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nb.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://cz.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://pi.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://pz.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lg.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://fy.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hj.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ab.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oc.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cd.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://vj.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://oc.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://oz.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zl.nicolike.cn

[A03] 常量定义
来源：http://rk.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mn.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://np.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://rc.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://gy.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://ba.521024.cn

Go:   const PI = 3.14159
来源：http://ze.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://om.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://nq.muxihuayi.cn

[A04] 判断变量类型
来源：http://bl.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dw.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wf.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://he.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ge.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://za.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vc.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://re.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://yx.shxzskj.cn

[A05] 整数除法与取模
来源：http://pv.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wt.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zm.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vt.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zp.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://ey.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://cb.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://bx.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://ju.9csxet.cn

[A06] 字符串转数字
来源：http://bo.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://fo.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://au.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://de.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sm.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dx.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yz.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nn.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cy.shtwfgs.cn

[A07] 数字转字符串
来源：http://ke.yuntaijiaju.cn

Py:   str(42)
来源：http://ny.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://jx.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://tj.nszjky.cn

TS:   String(42)
来源：http://io.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oh.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://rw.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://in.hnjuh.cn

C#:   42.ToString()
来源：http://jt.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://ub.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nb.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rt.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eq.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nd.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hi.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wf.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vy.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://is.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://sk.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sa.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bp.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yg.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://it.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ut.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wu.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jg.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yr.huixinmuqiang.cn

[A10] 生成随机数
来源：http://af.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://zq.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://mv.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://se.bookmarksfly.cn


<!-- 参考信息 -->