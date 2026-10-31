代发 wailian999

[U59] PHP：自定义排序
来源：http://ax.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://va.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://bw.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wr.gzmigu.cn

[U61] PHP：正则
来源：http://zl.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vr.panjiajie.cn

[U62] PHP：日期对象
来源：http://fv.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wg.521024.cn

[U63] PHP：文件读写
来源：http://gv.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ee.shxzskj.cn

[U64] PHP：目录遍历
来源：http://uy.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://ng.asd995.cn

[U65] PHP：会话
来源：http://uf.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yl.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://zb.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://we.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://xs.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://km.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://ac.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ev.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://rr.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pi.9csxet.cn

[U70] PHP：PDO 事务
来源：http://xl.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mg.huanxung.cn

[U71] PHP：抛出异常
来源：http://zs.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://hj.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://ce.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://tl.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://mg.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://tr.nicolike.cn

[U74] PHP：读取环境变量
来源：http://ai.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://xs.nicolike.cn

[U75] PHP：依赖注入
来源：http://qe.asd995.cn

composer require psr/container
来源：http://nr.szxytkj.cn

[U76] PHP：简单路由
来源：http://ic.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://br.lnxyls.cn

[U77] PHP：模板渲染
来源：http://ij.jctech888.com.cn

composer require twig/twig
来源：http://ze.newstarts.cn

[U78] PHP：单元测试
来源：http://wg.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://vm.shxzukj.cn

[U79] PHP：静态分析
来源：http://am.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://wl.colortex.cn

[U80] PHP：代码规范修复
来源：http://hg.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eh.wgjwhj.cn

[U81] JS：初始化项目
来源：http://tx.huixiangedu.cn

npm init -y;  npm i express
来源：http://cj.9csxet.cn

[U82] JS：package.json 脚本
来源：http://wc.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mt.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://wa.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nj.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://pv.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xu.shxzukj.cn

[U85] JS：可选链
来源：http://ti.szxytkj.cn

a?.b?.c
来源：http://bj.chemitech.net.cn

[U86] JS：空值合并
来源：http://uq.9csxet.cn

a ?? b
来源：http://in.gzmigu.cn

[U87] JS：解构默认值
来源：http://kf.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ni.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://kr.lnxyls.cn

{ ...a, ...b }
来源：http://px.colortex.cn

[U89] JS：数组去重
来源：http://im.huanxung.cn

[...new Set(arr)]
来源：http://mx.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://fw.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://iu.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://js.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gq.shxzskj.cn

[U92] JS：深拷贝
来源：http://nv.szsharing.cn

structuredClone(obj)
来源：http://ma.haigaiapp.cn

[U93] JS：模板字符串
来源：http://vy.huixinmuqiang.cn

`共 ${n} 条`
来源：http://vp.yuexingan06.cn

[U94] JS：箭头函数
来源：http://lo.521024.cn

const double = x => x * 2;
来源：http://gz.huanxung.cn

[U95] JS：Promise 包装
来源：http://xa.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://cn.newstarts.cn

[U96] JS：async/await 与异常
来源：http://uu.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bp.shxzukj.cn

[U97] JS：并发请求
来源：http://ls.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rp.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://fb.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gd.lnxyls.cn

[U99] JS：事件监听
来源：http://df.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://iq.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://ve.jctech888.com.cn

document.querySelector(".item")
来源：http://ss.bjjhwx.cn

[U101] JS：classList 操作
来源：http://xz.521024.cn

el.classList.toggle("active")
来源：http://sk.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://vf.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pt.yuntaijiaju.cn

[U103] JS：定时器
来源：http://ur.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yl.wgjwhj.cn

[U104] JS：防抖
来源：http://jy.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kj.jianghongdianzi.cn

[U105] JS：节流
来源：http://gw.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://za.hnjuh.cn

[U106] JS：日期格式化
来源：http://bv.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ih.huanxung.cn

[U107] JS：数字千分位
来源：http://ku.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nh.asd995.cn

[U108] JS：随机整数
来源：http://cx.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qt.haigaiapp.cn

[U109] JS：数组分组
来源：http://km.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://jg.huanxung.cn

[U110] JS：数组分块
来源：http://fa.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://me.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ri.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://yc.szsharing.cn

[U112] JS：字符串补位
来源：http://ui.panjiajie.cn

"7".padStart(3, "0")
来源：http://du.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://mn.nszjky.cn

s.replaceAll("a", "b")
来源：http://za.hahajie.cn

[U114] JS：JSON 深比较
来源：http://mo.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ih.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ad.shxzukj.cn

crypto.randomUUID()
来源：http://hn.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://qn.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://co.huanxung.cn

[U117] JS：单元测试
来源：http://ir.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://vu.9csxet.cn

[U118] JS：开发服务器
来源：http://xn.lnxyls.cn

npm i -D vite;  npx vite
来源：http://nu.nicolike.cn

[U119] JS：生产构建
来源：http://yr.shxzskj.cn

npx vite build
来源：http://bo.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ho.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://pb.huixinmuqiang.cn

================================================================================
来源：http://dx.521024.cn

统计汇总
来源：http://fl.bookmarksfly.cn

================================================================================
来源：http://qo.shxzskj.cn

按语言统计（条）：
来源：http://mt.asd995.cn

Python ......... 252
来源：http://fp.521024.cn

PHP ............ 252
来源：http://si.szxytkj.cn

JavaScript ..... 252
来源：http://hb.yuntaijiaju.cn

TypeScript ..... 212
来源：http://oq.muxihuayi.cn

Java ........... 212
来源：http://pf.panjiajie.cn

Go ............. 212
来源：http://df.bookmarksfly.cn

Ruby ........... 212
来源：http://ho.panjiajie.cn

C# ............. 212
来源：http://ud.huixinmuqiang.cn

C .............. 30
来源：http://ys.hahajie.cn

C++ ............ 30
来源：http://zs.newstarts.cn

SQL ............ 90
来源：http://kz.nszjky.cn

Bash ........... 80
来源：http://ud.yuexingan06.cn

Kotlin ......... 15
来源：http://po.chemitech.net.cn

Swift .......... 15
来源：http://mb.shtwfgs.cn

Lua ............ 10
来源：http://ns.chemitech.net.cn

Perl ........... 10
来源：http://aa.lnxyls.cn

Scala .......... 10
来源：http://zr.9csxet.cn

------------------------------------
来源：http://mb.nicolike.cn

合计 ........... 2106 条
来源：http://rh.asd995.cn

按章节统计：
来源：http://uu.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mq.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kw.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gi.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ud.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ld.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uj.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wd.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://co.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ap.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sw.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ei.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qf.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wo.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nu.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nk.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qe.huixiangedu.cn

Q SQL 专题                              90
来源：http://bt.szsharing.cn

R Bash 专题                             80
来源：http://gk.haigaiapp.cn

S C / C++ 专题                          60
来源：http://iv.asd995.cn

T 其他语言补充                          60
来源：http://ra.lnxyls.cn

U 高频实用片段                         120
来源：http://ym.hnjuh.cn

------------------------------------
来源：http://xz.asd995.cn

合计                                  2106 条
来源：http://zz.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ds.chemitech.net.cn

使用提醒
来源：http://ce.nszjky.cn

--------------------------------------------------------------------------------
来源：http://cn.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ts.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oy.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tx.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yt.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ms.haigaiapp.cn

—— 文件结束 ——
来源：http://ut.jianghongdianzi.cn

================================================================================
来源：http://sc.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://hi.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://fu.huixinmuqiang.cn

================================================================================
来源：http://tj.asd995.cn

【收录内容】
来源：http://ce.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wz.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bz.521024.cn

SQL · Bash · C · C++
来源：http://as.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ud.jctech888.com.cn

【使用说明】
来源：http://dj.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lx.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qe.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iq.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bx.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zs.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ry.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ry.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ot.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cg.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zi.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://td.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iv.yuntaijiaju.cn

【文件统计】
来源：http://iz.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hd.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://zq.yuntaijiaju.cn

目  录
来源：http://ng.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://zj.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kn.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gy.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tl.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ll.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ig.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uk.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ed.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pj.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ee.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lt.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wr.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ct.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nc.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tx.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kg.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zy.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mq.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ny.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://os.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oe.bookmarksfly.cn

================================================================================
来源：http://pz.muxihuayi.cn

A. 基础语法与类型
来源：http://ls.huixiangedu.cn

================================================================================
来源：http://fb.szxytkj.cn

[A01] Hello World
来源：http://bp.nicolike.cn

Py:   print("Hello, World!")
来源：http://zr.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://qy.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://yu.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hj.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://hs.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://id.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://gm.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kp.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://bq.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uw.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ki.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qw.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ko.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://cx.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://gs.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://fm.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hb.panjiajie.cn

[A03] 常量定义
来源：http://mq.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xe.asd995.cn

PHP:  const PI = 3.14159;
来源：http://jq.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://fl.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://gb.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://kf.shxzskj.cn

Go:   const PI = 3.14159
来源：http://sk.newstarts.cn

Ruby: PI = 3.14159
来源：http://yg.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://sa.shtwfgs.cn

[A04] 判断变量类型
来源：http://uz.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mh.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qy.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fq.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://wp.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nv.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gr.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zq.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://bf.haigaiapp.cn

[A05] 整数除法与取模
来源：http://va.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ot.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tn.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rs.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hw.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://lc.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://sc.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://uq.521024.cn

C#:   7 / 2; 7 % 2
来源：http://ha.521024.cn

[A06] 字符串转数字
来源：http://hs.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://go.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tl.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lx.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hv.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ea.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wx.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wc.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://at.chemitech.net.cn

[A07] 数字转字符串
来源：http://uk.haigaiapp.cn

Py:   str(42)
来源：http://vc.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://by.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://tn.chemitech.net.cn

TS:   String(42)
来源：http://nb.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://we.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ib.jctech888.com.cn

Ruby: 42.to_s
来源：http://xj.9csxet.cn

C#:   42.ToString()
来源：http://zz.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://db.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bx.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zj.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qv.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jt.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zm.newstarts.cn


<!-- 参考信息 -->