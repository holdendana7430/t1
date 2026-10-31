代发 wailian999

[U69] PHP：PDO 预处理
来源：http://sy.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jj.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://ar.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xo.huanxung.cn

[U71] PHP：抛出异常
来源：http://yd.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://eb.szsharing.cn

[U72] PHP：写错误日志
来源：http://hi.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://xc.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://ne.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://gz.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://kq.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://br.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://ji.bjjhwx.cn

composer require psr/container
来源：http://hc.521024.cn

[U76] PHP：简单路由
来源：http://dg.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mv.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://mh.huixinmuqiang.cn

composer require twig/twig
来源：http://jm.hnjuh.cn

[U78] PHP：单元测试
来源：http://mp.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://jx.yuexingan06.cn

[U79] PHP：静态分析
来源：http://vv.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://og.nicolike.cn

[U80] PHP：代码规范修复
来源：http://qm.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jg.huanxung.cn

[U81] JS：初始化项目
来源：http://jl.hnjuh.cn

npm init -y;  npm i express
来源：http://qr.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://uw.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://av.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://xx.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://si.521024.cn

[U84] JS：CommonJS 写法
来源：http://ni.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wo.wgjwhj.cn

[U85] JS：可选链
来源：http://nh.huixinmuqiang.cn

a?.b?.c
来源：http://if.nicolike.cn

[U86] JS：空值合并
来源：http://rr.newstarts.cn

a ?? b
来源：http://rh.lnxyls.cn

[U87] JS：解构默认值
来源：http://eg.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://dm.nicolike.cn

[U88] JS：对象展开合并
来源：http://bq.szxytkj.cn

{ ...a, ...b }
来源：http://tc.haigaiapp.cn

[U89] JS：数组去重
来源：http://pk.huixiangedu.cn

[...new Set(arr)]
来源：http://mn.colortex.cn

[U90] JS：数字数组排序
来源：http://jx.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://xz.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://dq.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xu.newstarts.cn

[U92] JS：深拷贝
来源：http://bm.nszjky.cn

structuredClone(obj)
来源：http://vt.lnxyls.cn

[U93] JS：模板字符串
来源：http://fe.521024.cn

`共 ${n} 条`
来源：http://ig.nszjky.cn

[U94] JS：箭头函数
来源：http://cx.nszjky.cn

const double = x => x * 2;
来源：http://jg.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://wc.asd995.cn

new Promise((resolve, reject) => {})
来源：http://cm.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://is.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://do.huixiangedu.cn

[U97] JS：并发请求
来源：http://cc.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://qt.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lh.asd995.cn

[U99] JS：事件监听
来源：http://ep.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://jb.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://ah.gzmigu.cn

document.querySelector(".item")
来源：http://be.haigaiapp.cn

[U101] JS：classList 操作
来源：http://no.szxytkj.cn

el.classList.toggle("active")
来源：http://oe.lnxyls.cn

[U102] JS：本地存储
来源：http://rd.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kl.muxihuayi.cn

[U103] JS：定时器
来源：http://ue.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qa.gzmigu.cn

[U104] JS：防抖
来源：http://bm.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oc.9csxet.cn

[U105] JS：节流
来源：http://wf.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rj.shxzskj.cn

[U106] JS：日期格式化
来源：http://bs.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fs.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://yz.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://la.nicolike.cn

[U108] JS：随机整数
来源：http://bs.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iy.shtwfgs.cn

[U109] JS：数组分组
来源：http://hk.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://zd.bookmarksfly.cn

[U110] JS：数组分块
来源：http://tw.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mk.shxzukj.cn

[U111] JS：对象转 Map
来源：http://pl.lnxyls.cn

new Map(Object.entries(obj))
来源：http://xb.szxytkj.cn

[U112] JS：字符串补位
来源：http://cq.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://uq.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://mw.shxzskj.cn

s.replaceAll("a", "b")
来源：http://dz.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://cs.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mj.hahajie.cn

[U115] JS：生成 UUID
来源：http://kj.yuntaijiaju.cn

crypto.randomUUID()
来源：http://ri.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://km.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://qz.asd995.cn

[U117] JS：单元测试
来源：http://qy.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://ra.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://my.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://kf.colortex.cn

[U119] JS：生产构建
来源：http://rn.huixinmuqiang.cn

npx vite build
来源：http://pd.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://yx.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://on.bjjhwx.cn

================================================================================
来源：http://tv.wgjwhj.cn

统计汇总
来源：http://bv.jianghongdianzi.cn

================================================================================
来源：http://zp.shxzskj.cn

按语言统计（条）：
来源：http://uo.yuexingan06.cn

Python ......... 252
来源：http://ie.lnxyls.cn

PHP ............ 252
来源：http://sw.521024.cn

JavaScript ..... 252
来源：http://vo.huixiangedu.cn

TypeScript ..... 212
来源：http://xc.panjiajie.cn

Java ........... 212
来源：http://zf.haigaiapp.cn

Go ............. 212
来源：http://qw.hahajie.cn

Ruby ........... 212
来源：http://cj.yuntaijiaju.cn

C# ............. 212
来源：http://dv.jctech888.com.cn

C .............. 30
来源：http://fq.haigaiapp.cn

C++ ............ 30
来源：http://fy.bjjhwx.cn

SQL ............ 90
来源：http://em.shtwfgs.cn

Bash ........... 80
来源：http://yx.yuexingan06.cn

Kotlin ......... 15
来源：http://ho.bookmarksfly.cn

Swift .......... 15
来源：http://tt.chemitech.net.cn

Lua ............ 10
来源：http://cu.shtwfgs.cn

Perl ........... 10
来源：http://gg.bjjhwx.cn

Scala .......... 10
来源：http://iu.yuexingan06.cn

------------------------------------
来源：http://rg.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://uf.haigaiapp.cn

按章节统计：
来源：http://iq.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zg.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nz.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lc.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kq.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fx.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iv.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://th.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pq.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bp.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mp.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bm.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fk.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nv.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ko.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yn.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://au.lnxyls.cn

Q SQL 专题                              90
来源：http://pw.asd995.cn

R Bash 专题                             80
来源：http://fk.shxzukj.cn

S C / C++ 专题                          60
来源：http://ie.jctech888.com.cn

T 其他语言补充                          60
来源：http://ic.huixiangedu.cn

U 高频实用片段                         120
来源：http://zo.bjjhwx.cn

------------------------------------
来源：http://cw.yuexingan06.cn

合计                                  2106 条
来源：http://fc.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://el.panjiajie.cn

使用提醒
来源：http://re.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://id.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vh.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fv.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lz.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bc.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ny.yuexingan06.cn

—— 文件结束 ——
来源：http://on.huixiangedu.cn

================================================================================
来源：http://yo.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://bh.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://tz.hnjuh.cn

================================================================================
来源：http://ob.jctech888.com.cn

【收录内容】
来源：http://zv.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://up.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://le.szsharing.cn

SQL · Bash · C · C++
来源：http://ed.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://li.jianghongdianzi.cn

【使用说明】
来源：http://yg.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fa.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lm.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qv.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cu.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qj.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bb.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zp.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lv.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ei.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cc.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pz.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gh.yuexingan06.cn

【文件统计】
来源：http://jf.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://re.huanxung.cn

--------------------------------------------------------------------------------
来源：http://wm.panjiajie.cn

目  录
来源：http://up.asd995.cn

--------------------------------------------------------------------------------
来源：http://or.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zz.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hg.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zy.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ad.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://in.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lw.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ux.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://li.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sf.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ve.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xt.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nt.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yl.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gh.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qm.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sa.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://go.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eu.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xi.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ur.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lv.521024.cn

================================================================================
来源：http://vd.panjiajie.cn

A. 基础语法与类型
来源：http://la.hnjuh.cn

================================================================================
来源：http://xe.shxzukj.cn

[A01] Hello World
来源：http://or.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://qv.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://li.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://vj.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xw.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://kj.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://dp.colortex.cn

Ruby: puts "Hello, World!"
来源：http://jb.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mo.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://ug.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oa.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ad.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hz.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hy.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://gj.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://km.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://wq.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://no.shxzukj.cn

[A03] 常量定义
来源：http://zs.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://co.colortex.cn

PHP:  const PI = 3.14159;
来源：http://mf.newstarts.cn

JS:   const PI = 3.14159;
来源：http://qn.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://ax.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://kz.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://jc.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://df.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://bo.asd995.cn

[A04] 判断变量类型
来源：http://bo.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://be.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ad.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rj.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://vu.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://my.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yk.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fl.521024.cn

C#:   x.GetType().Name; x is int
来源：http://jc.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://rl.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sc.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xp.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yq.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yh.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://mh.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://jz.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://tb.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://vt.bjjhwx.cn

[A06] 字符串转数字
来源：http://yz.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://vp.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cv.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ag.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ff.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bu.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xw.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ru.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gh.colortex.cn

[A07] 数字转字符串
来源：http://ss.haigaiapp.cn

Py:   str(42)
来源：http://lv.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://pk.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://qn.szsharing.cn

TS:   String(42)
来源：http://de.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://em.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://sz.wgjwhj.cn

Ruby: 42.to_s
来源：http://zj.gzmigu.cn

C#:   42.ToString()
来源：http://ma.szxytkj.cn

[A08] 取整与四舍五入
来源：http://ls.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tv.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zt.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://la.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dl.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vq.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sa.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://do.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ps.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://ps.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gq.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://px.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lk.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hi.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rk.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iv.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uw.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qk.asd995.cn

[A10] 生成随机数
来源：http://sj.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://en.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://cx.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yt.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://os.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://fj.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ct.521024.cn

Ruby: rand(1..100)
来源：http://qd.asd995.cn


<!-- 参考信息 -->