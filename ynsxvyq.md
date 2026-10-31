代发 wailian999

[U59] PHP：自定义排序
来源：http://vd.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jh.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://de.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://it.521024.cn

[U61] PHP：正则
来源：http://pl.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cu.521024.cn

[U62] PHP：日期对象
来源：http://ys.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hc.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://an.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yc.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://bk.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://qr.hnjuh.cn

[U65] PHP：会话
来源：http://gh.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xe.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://eb.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://th.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://of.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xm.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://bh.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iq.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://yj.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kd.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://fo.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wj.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://yg.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://tv.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://qg.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://pw.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://so.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://uk.huanxung.cn

[U74] PHP：读取环境变量
来源：http://ms.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://qf.hnjuh.cn

[U75] PHP：依赖注入
来源：http://sz.lnxyls.cn

composer require psr/container
来源：http://ce.lnxyls.cn

[U76] PHP：简单路由
来源：http://tw.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://om.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://jr.szsharing.cn

composer require twig/twig
来源：http://em.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://xr.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://ac.chemitech.net.cn

[U79] PHP：静态分析
来源：http://pm.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://uv.colortex.cn

[U80] PHP：代码规范修复
来源：http://hh.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wh.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://ba.bookmarksfly.cn

npm init -y;  npm i express
来源：http://ux.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://sb.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qv.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://mu.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mz.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://yg.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://su.huixiangedu.cn

[U85] JS：可选链
来源：http://xx.hahajie.cn

a?.b?.c
来源：http://qs.colortex.cn

[U86] JS：空值合并
来源：http://ec.jianghongdianzi.cn

a ?? b
来源：http://fy.muxihuayi.cn

[U87] JS：解构默认值
来源：http://ei.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://aq.asd995.cn

[U88] JS：对象展开合并
来源：http://gl.haigaiapp.cn

{ ...a, ...b }
来源：http://ei.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://ni.521024.cn

[...new Set(arr)]
来源：http://fu.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://id.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://ut.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://ge.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vj.nszjky.cn

[U92] JS：深拷贝
来源：http://yd.9csxet.cn

structuredClone(obj)
来源：http://yx.wgjwhj.cn

[U93] JS：模板字符串
来源：http://el.chemitech.net.cn

`共 ${n} 条`
来源：http://ee.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://lx.shxzskj.cn

const double = x => x * 2;
来源：http://le.521024.cn

[U95] JS：Promise 包装
来源：http://qt.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://uh.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://zy.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rr.bookmarksfly.cn

[U97] JS：并发请求
来源：http://cv.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zz.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ci.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://be.asd995.cn

[U99] JS：事件监听
来源：http://mu.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://nl.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://cq.yuntaijiaju.cn

document.querySelector(".item")
来源：http://gj.newstarts.cn

[U101] JS：classList 操作
来源：http://wx.shtwfgs.cn

el.classList.toggle("active")
来源：http://lv.chemitech.net.cn

[U102] JS：本地存储
来源：http://fn.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jy.shtwfgs.cn

[U103] JS：定时器
来源：http://dy.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oa.gzmigu.cn

[U104] JS：防抖
来源：http://mq.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.haigaiapp.cn

[U105] JS：节流
来源：http://qe.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aq.gzmigu.cn

[U106] JS：日期格式化
来源：http://kp.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ly.newstarts.cn

[U107] JS：数字千分位
来源：http://pm.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ua.asd995.cn

[U108] JS：随机整数
来源：http://zy.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vy.9csxet.cn

[U109] JS：数组分组
来源：http://bb.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://mx.nicolike.cn

[U110] JS：数组分块
来源：http://be.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bh.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://gd.shxzskj.cn

new Map(Object.entries(obj))
来源：http://td.shxzskj.cn

[U112] JS：字符串补位
来源：http://ug.hnjuh.cn

"7".padStart(3, "0")
来源：http://ef.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://ui.9csxet.cn

s.replaceAll("a", "b")
来源：http://yu.9csxet.cn

[U114] JS：JSON 深比较
来源：http://is.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nj.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://ac.nszjky.cn

crypto.randomUUID()
来源：http://ls.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://hw.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://qd.newstarts.cn

[U117] JS：单元测试
来源：http://xh.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://to.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://gy.newstarts.cn

npm i -D vite;  npx vite
来源：http://fn.panjiajie.cn

[U119] JS：生产构建
来源：http://kz.lnxyls.cn

npx vite build
来源：http://pf.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://gt.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://km.521024.cn

================================================================================
来源：http://cw.hahajie.cn

统计汇总
来源：http://qq.colortex.cn

================================================================================
来源：http://ch.muxihuayi.cn

按语言统计（条）：
来源：http://ie.nicolike.cn

Python ......... 252
来源：http://xr.nicolike.cn

PHP ............ 252
来源：http://zu.shtwfgs.cn

JavaScript ..... 252
来源：http://uc.bjjhwx.cn

TypeScript ..... 212
来源：http://wr.521024.cn

Java ........... 212
来源：http://kf.szsharing.cn

Go ............. 212
来源：http://th.hnjuh.cn

Ruby ........... 212
来源：http://ul.panjiajie.cn

C# ............. 212
来源：http://tg.jctech888.com.cn

C .............. 30
来源：http://qk.panjiajie.cn

C++ ............ 30
来源：http://pi.9csxet.cn

SQL ............ 90
来源：http://ky.colortex.cn

Bash ........... 80
来源：http://dy.9csxet.cn

Kotlin ......... 15
来源：http://gi.shtwfgs.cn

Swift .......... 15
来源：http://bq.huixinmuqiang.cn

Lua ............ 10
来源：http://si.haigaiapp.cn

Perl ........... 10
来源：http://uq.nszjky.cn

Scala .......... 10
来源：http://pi.colortex.cn

------------------------------------
来源：http://ws.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://fv.szsharing.cn

按章节统计：
来源：http://ey.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cb.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gi.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ey.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hq.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pz.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://la.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://st.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bz.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ga.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wj.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://al.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kd.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gr.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ph.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cg.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yq.haigaiapp.cn

Q SQL 专题                              90
来源：http://it.nszjky.cn

R Bash 专题                             80
来源：http://sc.yuexingan06.cn

S C / C++ 专题                          60
来源：http://do.lnxyls.cn

T 其他语言补充                          60
来源：http://us.panjiajie.cn

U 高频实用片段                         120
来源：http://hf.huixiangedu.cn

------------------------------------
来源：http://ke.lnxyls.cn

合计                                  2106 条
来源：http://sz.newstarts.cn

--------------------------------------------------------------------------------
来源：http://sd.bookmarksfly.cn

使用提醒
来源：http://bs.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ij.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nu.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hd.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uw.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bp.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ja.szxytkj.cn

—— 文件结束 ——
来源：http://im.newstarts.cn

================================================================================
来源：http://gx.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://gg.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://gb.szsharing.cn

================================================================================
来源：http://gs.colortex.cn

【收录内容】
来源：http://bv.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qn.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ok.wgjwhj.cn

SQL · Bash · C · C++
来源：http://ww.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vz.521024.cn

【使用说明】
来源：http://ge.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fl.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xm.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cw.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rn.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xx.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ej.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mk.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ez.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ns.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ws.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kq.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wa.bjjhwx.cn

【文件统计】
来源：http://le.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gl.colortex.cn

--------------------------------------------------------------------------------
来源：http://ev.nicolike.cn

目  录
来源：http://xz.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://xi.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ku.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vc.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bp.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ga.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ft.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://my.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fo.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fp.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iz.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hm.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ya.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jv.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sx.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bg.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wh.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sb.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sb.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://om.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gk.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bc.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mo.wgjwhj.cn

================================================================================
来源：http://gr.hnjuh.cn

A. 基础语法与类型
来源：http://qn.521024.cn

================================================================================
来源：http://xi.9csxet.cn

[A01] Hello World
来源：http://iq.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://kq.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://kl.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://of.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oc.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://tf.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://mj.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://gt.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nm.shxzukj.cn

[A02] 变量声明与赋值
来源：http://wo.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pg.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kb.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://al.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://db.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://xe.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://zf.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://io.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sw.nszjky.cn

[A03] 常量定义
来源：http://yl.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ng.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://kj.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://af.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://rs.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://mb.colortex.cn

Go:   const PI = 3.14159
来源：http://ne.szsharing.cn

Ruby: PI = 3.14159
来源：http://jb.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://oy.jctech888.com.cn

[A04] 判断变量类型
来源：http://rr.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mu.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kd.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xe.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://ly.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ri.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kv.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rb.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://zw.gzmigu.cn

[A05] 整数除法与取模
来源：http://fr.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kw.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://su.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://px.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ey.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://hs.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://jc.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://ir.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://kw.chemitech.net.cn

[A06] 字符串转数字
来源：http://nh.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://xq.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mj.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bz.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hk.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ub.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lw.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://to.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sj.shxzukj.cn

[A07] 数字转字符串
来源：http://rh.huixiangedu.cn

Py:   str(42)
来源：http://qk.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://dw.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://uq.nicolike.cn

TS:   String(42)
来源：http://gr.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nx.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://gj.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://ni.huixinmuqiang.cn

C#:   42.ToString()
来源：http://zl.szsharing.cn

[A08] 取整与四舍五入
来源：http://cp.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://az.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ek.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eu.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nv.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ce.nicolike.cn


<!-- 参考信息 -->