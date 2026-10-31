代发 wailian999

[U63] PHP：文件读写
来源：http://bb.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://na.huanxung.cn

[U64] PHP：目录遍历
来源：http://np.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ny.shxzukj.cn

[U65] PHP：会话
来源：http://ub.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gk.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://sp.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kp.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://tm.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oo.nicolike.cn

[U68] PHP：PDO 连接
来源：http://lx.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kn.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://fu.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://za.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://br.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sn.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://pb.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://vh.gzmigu.cn

[U72] PHP：写错误日志
来源：http://od.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://bt.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://xk.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://cr.huanxung.cn

[U74] PHP：读取环境变量
来源：http://gv.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://yf.huanxung.cn

[U75] PHP：依赖注入
来源：http://eg.hnjuh.cn

composer require psr/container
来源：http://ju.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ad.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ys.shxzskj.cn

[U77] PHP：模板渲染
来源：http://fh.521024.cn

composer require twig/twig
来源：http://vx.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://qu.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://ii.hnjuh.cn

[U79] PHP：静态分析
来源：http://po.colortex.cn

composer require --dev phpstan/phpstan
来源：http://rr.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://ii.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yx.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://rk.huixiangedu.cn

npm init -y;  npm i express
来源：http://hd.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://tm.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ly.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://zh.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ps.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://kz.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eh.szsharing.cn

[U85] JS：可选链
来源：http://fl.huixiangedu.cn

a?.b?.c
来源：http://kw.gzmigu.cn

[U86] JS：空值合并
来源：http://dz.hnjuh.cn

a ?? b
来源：http://gl.muxihuayi.cn

[U87] JS：解构默认值
来源：http://hf.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://op.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://yo.shxzukj.cn

{ ...a, ...b }
来源：http://lr.panjiajie.cn

[U89] JS：数组去重
来源：http://mu.muxihuayi.cn

[...new Set(arr)]
来源：http://zy.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://mc.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://mc.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://zd.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hm.huanxung.cn

[U92] JS：深拷贝
来源：http://wl.hnjuh.cn

structuredClone(obj)
来源：http://xh.hnjuh.cn

[U93] JS：模板字符串
来源：http://br.nszjky.cn

`共 ${n} 条`
来源：http://vv.panjiajie.cn

[U94] JS：箭头函数
来源：http://zq.shxzukj.cn

const double = x => x * 2;
来源：http://qv.521024.cn

[U95] JS：Promise 包装
来源：http://km.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://tj.newstarts.cn

[U96] JS：async/await 与异常
来源：http://yk.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ja.bookmarksfly.cn

[U97] JS：并发请求
来源：http://hb.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://um.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://vb.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://um.haigaiapp.cn

[U99] JS：事件监听
来源：http://qt.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://fm.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://js.yuexingan06.cn

document.querySelector(".item")
来源：http://ti.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://nf.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://rh.bjjhwx.cn

[U102] JS：本地存储
来源：http://zw.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tk.bookmarksfly.cn

[U103] JS：定时器
来源：http://to.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yf.nicolike.cn

[U104] JS：防抖
来源：http://dr.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rs.newstarts.cn

[U105] JS：节流
来源：http://nd.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://md.shtwfgs.cn

[U106] JS：日期格式化
来源：http://fn.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ed.shxzskj.cn

[U107] JS：数字千分位
来源：http://ob.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wn.chemitech.net.cn

[U108] JS：随机整数
来源：http://sc.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ha.gzmigu.cn

[U109] JS：数组分组
来源：http://li.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://li.szsharing.cn

[U110] JS：数组分块
来源：http://hj.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rp.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://qx.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://to.bjjhwx.cn

[U112] JS：字符串补位
来源：http://xy.muxihuayi.cn

"7".padStart(3, "0")
来源：http://aj.shxzukj.cn

[U113] JS：正则替换全部
来源：http://dy.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://xw.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://se.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ya.szxytkj.cn

[U115] JS：生成 UUID
来源：http://mr.muxihuayi.cn

crypto.randomUUID()
来源：http://sd.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://rt.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://or.9csxet.cn

[U117] JS：单元测试
来源：http://gw.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://uw.shxzskj.cn

[U118] JS：开发服务器
来源：http://qf.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://jy.shtwfgs.cn

[U119] JS：生产构建
来源：http://fd.shxzskj.cn

npx vite build
来源：http://jh.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://xt.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://zb.jctech888.com.cn

================================================================================
来源：http://pf.gzmigu.cn

统计汇总
来源：http://it.gzmigu.cn

================================================================================
来源：http://pu.newstarts.cn

按语言统计（条）：
来源：http://ab.huixinmuqiang.cn

Python ......... 252
来源：http://nd.jctech888.com.cn

PHP ............ 252
来源：http://kd.shxzskj.cn

JavaScript ..... 252
来源：http://dc.huanxung.cn

TypeScript ..... 212
来源：http://ab.yuntaijiaju.cn

Java ........... 212
来源：http://th.lnxyls.cn

Go ............. 212
来源：http://rx.shxzukj.cn

Ruby ........... 212
来源：http://xw.9csxet.cn

C# ............. 212
来源：http://fh.huixiangedu.cn

C .............. 30
来源：http://gn.bjjhwx.cn

C++ ............ 30
来源：http://mg.521024.cn

SQL ............ 90
来源：http://yy.shxzskj.cn

Bash ........... 80
来源：http://sb.yuexingan06.cn

Kotlin ......... 15
来源：http://lj.jianghongdianzi.cn

Swift .......... 15
来源：http://jo.wgjwhj.cn

Lua ............ 10
来源：http://we.muxihuayi.cn

Perl ........... 10
来源：http://sr.9csxet.cn

Scala .......... 10
来源：http://dn.jianghongdianzi.cn

------------------------------------
来源：http://kt.newstarts.cn

合计 ........... 2106 条
来源：http://tm.yuntaijiaju.cn

按章节统计：
来源：http://oc.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xu.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qg.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tw.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fj.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xz.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wn.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ph.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://za.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rr.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uo.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mb.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ki.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ut.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qk.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hy.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://js.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://cg.yuntaijiaju.cn

R Bash 专题                             80
来源：http://hm.wgjwhj.cn

S C / C++ 专题                          60
来源：http://zk.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://pb.shxzukj.cn

U 高频实用片段                         120
来源：http://vm.hnjuh.cn

------------------------------------
来源：http://ky.hnjuh.cn

合计                                  2106 条
来源：http://og.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://do.panjiajie.cn

使用提醒
来源：http://tz.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ai.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ju.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ol.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://py.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gh.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wu.521024.cn

—— 文件结束 ——
来源：http://jb.hahajie.cn

================================================================================
来源：http://kf.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://rb.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://qx.newstarts.cn

================================================================================
来源：http://so.wgjwhj.cn

【收录内容】
来源：http://cw.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jp.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eq.9csxet.cn

SQL · Bash · C · C++
来源：http://gp.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dj.asd995.cn

【使用说明】
来源：http://eg.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eg.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iv.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tm.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://us.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lj.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xi.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zn.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://la.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://he.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cq.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vs.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kz.asd995.cn

【文件统计】
来源：http://oi.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rd.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://fc.muxihuayi.cn

目  录
来源：http://en.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://xg.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oy.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zc.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yc.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jg.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ep.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mf.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ai.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sr.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rj.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ni.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wf.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nr.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://as.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jc.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wo.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rt.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zk.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ac.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iy.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qc.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lo.muxihuayi.cn

================================================================================
来源：http://gi.hahajie.cn

A. 基础语法与类型
来源：http://nf.panjiajie.cn

================================================================================
来源：http://lw.asd995.cn

[A01] Hello World
来源：http://ob.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://sc.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://hz.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://pe.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wn.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://un.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://zs.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://ov.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xx.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://zx.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dd.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://to.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zm.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yh.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://br.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://ly.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://lt.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nx.jianghongdianzi.cn

[A03] 常量定义
来源：http://zo.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wm.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://ut.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://zt.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://ou.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://dp.gzmigu.cn

Go:   const PI = 3.14159
来源：http://mb.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://xv.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://wp.chemitech.net.cn

[A04] 判断变量类型
来源：http://dh.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gz.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nz.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kk.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://lq.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ac.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uc.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kg.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://hl.wgjwhj.cn

[A05] 整数除法与取模
来源：http://qf.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hj.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qf.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pj.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pi.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://pv.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://xb.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://pb.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://oc.wgjwhj.cn

[A06] 字符串转数字
来源：http://ac.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://th.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lb.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://no.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jd.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cz.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yb.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zs.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eb.huixiangedu.cn

[A07] 数字转字符串
来源：http://sr.yuntaijiaju.cn

Py:   str(42)
来源：http://lb.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://zf.nicolike.cn

JS:   String(42); (42).toString()
来源：http://kz.muxihuayi.cn

TS:   String(42)
来源：http://kr.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ln.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://gl.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://fy.hahajie.cn

C#:   42.ToString()
来源：http://st.huanxung.cn

[A08] 取整与四舍五入
来源：http://rm.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cu.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://su.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://za.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xh.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cq.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mf.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ym.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pi.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://ez.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://is.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cz.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://we.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nx.shtwfgs.cn


<!-- 参考信息 -->