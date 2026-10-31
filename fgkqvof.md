代发 wailian999

[U61] PHP：正则
来源：http://vl.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hm.asd995.cn

[U62] PHP：日期对象
来源：http://sh.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://we.huanxung.cn

[U63] PHP：文件读写
来源：http://qk.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xj.asd995.cn

[U64] PHP：目录遍历
来源：http://gv.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://ld.yuexingan06.cn

[U65] PHP：会话
来源：http://un.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jb.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://qg.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sy.colortex.cn

[U67] PHP：处理文件上传
来源：http://rv.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://if.newstarts.cn

[U68] PHP：PDO 连接
来源：http://if.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kf.colortex.cn

[U69] PHP：PDO 预处理
来源：http://ie.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uc.nicolike.cn

[U70] PHP：PDO 事务
来源：http://hu.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xu.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://yt.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://dm.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://mm.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://dx.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://wb.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://mw.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://zq.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://eg.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://jm.colortex.cn

composer require psr/container
来源：http://ue.yuexingan06.cn

[U76] PHP：简单路由
来源：http://qx.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lb.nicolike.cn

[U77] PHP：模板渲染
来源：http://db.lnxyls.cn

composer require twig/twig
来源：http://gc.panjiajie.cn

[U78] PHP：单元测试
来源：http://bu.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://gg.9csxet.cn

[U79] PHP：静态分析
来源：http://bw.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://ss.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://lf.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gn.hahajie.cn

[U81] JS：初始化项目
来源：http://pt.panjiajie.cn

npm init -y;  npm i express
来源：http://cb.nicolike.cn

[U82] JS：package.json 脚本
来源：http://qn.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://st.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://qj.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ve.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://uc.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nl.panjiajie.cn

[U85] JS：可选链
来源：http://ja.colortex.cn

a?.b?.c
来源：http://gw.lnxyls.cn

[U86] JS：空值合并
来源：http://yd.muxihuayi.cn

a ?? b
来源：http://ue.shxzukj.cn

[U87] JS：解构默认值
来源：http://pe.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://re.9csxet.cn

[U88] JS：对象展开合并
来源：http://av.lnxyls.cn

{ ...a, ...b }
来源：http://td.hnjuh.cn

[U89] JS：数组去重
来源：http://av.jctech888.com.cn

[...new Set(arr)]
来源：http://yq.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://af.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://bw.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://qe.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ey.huanxung.cn

[U92] JS：深拷贝
来源：http://yk.9csxet.cn

structuredClone(obj)
来源：http://xt.nszjky.cn

[U93] JS：模板字符串
来源：http://iz.yuntaijiaju.cn

`共 ${n} 条`
来源：http://mt.521024.cn

[U94] JS：箭头函数
来源：http://aq.newstarts.cn

const double = x => x * 2;
来源：http://ey.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://cr.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://ps.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://vd.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://de.jctech888.com.cn

[U97] JS：并发请求
来源：http://zl.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jz.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://td.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rv.szxytkj.cn

[U99] JS：事件监听
来源：http://mo.huanxung.cn

el.addEventListener("click", e => {})
来源：http://ps.gzmigu.cn

[U100] JS：DOM 查询
来源：http://ub.newstarts.cn

document.querySelector(".item")
来源：http://mn.gzmigu.cn

[U101] JS：classList 操作
来源：http://jo.szxytkj.cn

el.classList.toggle("active")
来源：http://ag.nszjky.cn

[U102] JS：本地存储
来源：http://ew.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hq.hahajie.cn

[U103] JS：定时器
来源：http://ls.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qc.huixinmuqiang.cn

[U104] JS：防抖
来源：http://ls.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vn.asd995.cn

[U105] JS：节流
来源：http://mu.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://if.panjiajie.cn

[U106] JS：日期格式化
来源：http://vk.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gr.hahajie.cn

[U107] JS：数字千分位
来源：http://bq.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fu.shtwfgs.cn

[U108] JS：随机整数
来源：http://jb.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fq.szxytkj.cn

[U109] JS：数组分组
来源：http://jj.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://gf.nszjky.cn

[U110] JS：数组分块
来源：http://ko.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://to.huanxung.cn

[U111] JS：对象转 Map
来源：http://wd.szxytkj.cn

new Map(Object.entries(obj))
来源：http://qd.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://xg.szsharing.cn

"7".padStart(3, "0")
来源：http://nf.hnjuh.cn

[U113] JS：正则替换全部
来源：http://vo.hnjuh.cn

s.replaceAll("a", "b")
来源：http://wj.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://hy.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ki.newstarts.cn

[U115] JS：生成 UUID
来源：http://ib.jctech888.com.cn

crypto.randomUUID()
来源：http://mz.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://de.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://gk.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://iy.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://qo.gzmigu.cn

[U118] JS：开发服务器
来源：http://fn.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://ep.9csxet.cn

[U119] JS：生产构建
来源：http://ig.yuntaijiaju.cn

npx vite build
来源：http://wf.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://us.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://uv.haigaiapp.cn

================================================================================
来源：http://qm.jianghongdianzi.cn

统计汇总
来源：http://kz.chemitech.net.cn

================================================================================
来源：http://va.jctech888.com.cn

按语言统计（条）：
来源：http://gn.nszjky.cn

Python ......... 252
来源：http://rh.9csxet.cn

PHP ............ 252
来源：http://gi.shxzukj.cn

JavaScript ..... 252
来源：http://vm.hahajie.cn

TypeScript ..... 212
来源：http://ml.yuntaijiaju.cn

Java ........... 212
来源：http://rg.shxzukj.cn

Go ............. 212
来源：http://mo.newstarts.cn

Ruby ........... 212
来源：http://og.huanxung.cn

C# ............. 212
来源：http://ro.szxytkj.cn

C .............. 30
来源：http://xl.panjiajie.cn

C++ ............ 30
来源：http://gi.huanxung.cn

SQL ............ 90
来源：http://yy.huixinmuqiang.cn

Bash ........... 80
来源：http://jq.szsharing.cn

Kotlin ......... 15
来源：http://ce.szxytkj.cn

Swift .......... 15
来源：http://py.gzmigu.cn

Lua ............ 10
来源：http://vi.yuexingan06.cn

Perl ........... 10
来源：http://ta.wgjwhj.cn

Scala .......... 10
来源：http://mr.huixinmuqiang.cn

------------------------------------
来源：http://qu.nicolike.cn

合计 ........... 2106 条
来源：http://fx.huixiangedu.cn

按章节统计：
来源：http://ne.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cy.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bo.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cu.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://am.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ib.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gs.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bi.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ri.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zm.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mx.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ry.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cx.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gg.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sf.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ac.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wt.szsharing.cn

Q SQL 专题                              90
来源：http://ki.hahajie.cn

R Bash 专题                             80
来源：http://mn.9csxet.cn

S C / C++ 专题                          60
来源：http://on.521024.cn

T 其他语言补充                          60
来源：http://ka.haigaiapp.cn

U 高频实用片段                         120
来源：http://iw.jianghongdianzi.cn

------------------------------------
来源：http://bv.yuexingan06.cn

合计                                  2106 条
来源：http://hm.newstarts.cn

--------------------------------------------------------------------------------
来源：http://qg.yuntaijiaju.cn

使用提醒
来源：http://ws.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://az.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hj.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fe.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://os.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hl.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yy.jctech888.com.cn

—— 文件结束 ——
来源：http://hi.bookmarksfly.cn

================================================================================
来源：http://io.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://ze.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://pb.haigaiapp.cn

================================================================================
来源：http://ez.huixiangedu.cn

【收录内容】
来源：http://lp.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hy.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nc.szxytkj.cn

SQL · Bash · C · C++
来源：http://xm.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wz.gzmigu.cn

【使用说明】
来源：http://tq.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uq.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mn.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://au.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mi.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sj.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ww.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ll.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lv.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jg.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ue.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hy.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ee.yuexingan06.cn

【文件统计】
来源：http://dp.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oe.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://rw.gzmigu.cn

目  录
来源：http://ux.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://gc.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nq.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dp.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ho.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ih.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jl.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lh.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gx.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sl.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bw.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cx.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qz.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ev.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rb.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ij.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ay.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fu.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://td.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ie.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ms.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eq.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rr.haigaiapp.cn

================================================================================
来源：http://uc.szsharing.cn

A. 基础语法与类型
来源：http://kd.bookmarksfly.cn

================================================================================
来源：http://it.bjjhwx.cn

[A01] Hello World
来源：http://ds.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://cx.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://vg.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://cm.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nh.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://lp.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://mn.colortex.cn

Ruby: puts "Hello, World!"
来源：http://ix.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mo.nszjky.cn

[A02] 变量声明与赋值
来源：http://kw.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://al.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bd.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tq.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oi.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://jz.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://an.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://oh.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ed.gzmigu.cn

[A03] 常量定义
来源：http://au.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://af.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://wa.newstarts.cn

JS:   const PI = 3.14159;
来源：http://uh.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://wi.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://hl.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://ep.lnxyls.cn

Ruby: PI = 3.14159
来源：http://ld.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://gn.jctech888.com.cn

[A04] 判断变量类型
来源：http://zo.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dj.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://po.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ug.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://ov.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ws.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wx.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pf.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://uo.wgjwhj.cn

[A05] 整数除法与取模
来源：http://np.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ci.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://em.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ao.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cy.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://yg.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://pc.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://hv.521024.cn

C#:   7 / 2; 7 % 2
来源：http://yo.chemitech.net.cn

[A06] 字符串转数字
来源：http://rm.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://yw.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vg.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iv.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uz.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fi.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rs.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cj.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pp.jctech888.com.cn

[A07] 数字转字符串
来源：http://tc.chemitech.net.cn

Py:   str(42)
来源：http://vd.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://yh.521024.cn

JS:   String(42); (42).toString()
来源：http://xl.huixiangedu.cn

TS:   String(42)
来源：http://qr.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wu.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://ix.szsharing.cn

Ruby: 42.to_s
来源：http://qg.bookmarksfly.cn

C#:   42.ToString()
来源：http://ey.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://tv.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oz.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vg.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ur.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sr.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dh.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dz.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mj.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mg.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://sd.nicolike.cn


<!-- 参考信息 -->