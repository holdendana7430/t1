代发 wailian999

[U57] PHP：字符串插值
来源：http://eq.nicolike.cn

"值: {$a}"
来源：http://pj.nicolike.cn

[U58] PHP：数组三件套
来源：http://jm.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zh.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://ky.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uz.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://xy.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pd.shxzukj.cn

[U61] PHP：正则
来源：http://hh.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bh.szsharing.cn

[U62] PHP：日期对象
来源：http://vs.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gw.shxzukj.cn

[U63] PHP：文件读写
来源：http://by.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cz.colortex.cn

[U64] PHP：目录遍历
来源：http://mm.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://hy.asd995.cn

[U65] PHP：会话
来源：http://nr.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lf.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://ah.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gl.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://of.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rm.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://sw.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mv.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://dx.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xj.9csxet.cn

[U70] PHP：PDO 事务
来源：http://qk.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qy.huanxung.cn

[U71] PHP：抛出异常
来源：http://xg.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://hl.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://yu.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://ui.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://di.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://rr.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ch.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://oj.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://zv.shxzukj.cn

composer require psr/container
来源：http://sy.hnjuh.cn

[U76] PHP：简单路由
来源：http://py.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pe.szxytkj.cn

[U77] PHP：模板渲染
来源：http://sc.nszjky.cn

composer require twig/twig
来源：http://ll.lnxyls.cn

[U78] PHP：单元测试
来源：http://zg.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://nv.muxihuayi.cn

[U79] PHP：静态分析
来源：http://lo.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://ub.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://lc.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tg.hnjuh.cn

[U81] JS：初始化项目
来源：http://cw.9csxet.cn

npm init -y;  npm i express
来源：http://rj.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://zx.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ik.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://pl.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ys.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://kt.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cf.jctech888.com.cn

[U85] JS：可选链
来源：http://ea.shxzukj.cn

a?.b?.c
来源：http://ma.shtwfgs.cn

[U86] JS：空值合并
来源：http://pc.chemitech.net.cn

a ?? b
来源：http://gh.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://re.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://eo.nicolike.cn

[U88] JS：对象展开合并
来源：http://gd.nicolike.cn

{ ...a, ...b }
来源：http://zw.chemitech.net.cn

[U89] JS：数组去重
来源：http://bk.asd995.cn

[...new Set(arr)]
来源：http://wi.lnxyls.cn

[U90] JS：数字数组排序
来源：http://oj.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ka.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://tx.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qf.muxihuayi.cn

[U92] JS：深拷贝
来源：http://ob.huanxung.cn

structuredClone(obj)
来源：http://wj.shxzukj.cn

[U93] JS：模板字符串
来源：http://qb.wgjwhj.cn

`共 ${n} 条`
来源：http://ck.muxihuayi.cn

[U94] JS：箭头函数
来源：http://tu.muxihuayi.cn

const double = x => x * 2;
来源：http://wd.hnjuh.cn

[U95] JS：Promise 包装
来源：http://pf.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://bn.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://nb.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://as.wgjwhj.cn

[U97] JS：并发请求
来源：http://le.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vf.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://cl.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ro.muxihuayi.cn

[U99] JS：事件监听
来源：http://eb.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://bj.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://mo.huixiangedu.cn

document.querySelector(".item")
来源：http://jp.hahajie.cn

[U101] JS：classList 操作
来源：http://sa.bjjhwx.cn

el.classList.toggle("active")
来源：http://qs.lnxyls.cn

[U102] JS：本地存储
来源：http://mg.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mc.wgjwhj.cn

[U103] JS：定时器
来源：http://ms.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nx.bookmarksfly.cn

[U104] JS：防抖
来源：http://ma.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aw.shxzukj.cn

[U105] JS：节流
来源：http://sn.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://un.asd995.cn

[U106] JS：日期格式化
来源：http://rc.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gf.chemitech.net.cn

[U107] JS：数字千分位
来源：http://pf.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xa.nicolike.cn

[U108] JS：随机整数
来源：http://oj.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gh.muxihuayi.cn

[U109] JS：数组分组
来源：http://py.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://gz.nszjky.cn

[U110] JS：数组分块
来源：http://tp.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bn.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://kx.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://vk.hahajie.cn

[U112] JS：字符串补位
来源：http://pf.hnjuh.cn

"7".padStart(3, "0")
来源：http://dl.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://iy.asd995.cn

s.replaceAll("a", "b")
来源：http://en.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://fr.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jg.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://bn.panjiajie.cn

crypto.randomUUID()
来源：http://rs.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://fi.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://xk.bookmarksfly.cn

[U117] JS：单元测试
来源：http://dh.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://zy.nicolike.cn

[U118] JS：开发服务器
来源：http://wa.gzmigu.cn

npm i -D vite;  npx vite
来源：http://do.shxzukj.cn

[U119] JS：生产构建
来源：http://zr.jctech888.com.cn

npx vite build
来源：http://ur.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://oc.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://po.521024.cn

================================================================================
来源：http://sa.szsharing.cn

统计汇总
来源：http://nm.bookmarksfly.cn

================================================================================
来源：http://jc.huixinmuqiang.cn

按语言统计（条）：
来源：http://md.huanxung.cn

Python ......... 252
来源：http://ko.panjiajie.cn

PHP ............ 252
来源：http://fk.yuntaijiaju.cn

JavaScript ..... 252
来源：http://bc.huanxung.cn

TypeScript ..... 212
来源：http://dn.bookmarksfly.cn

Java ........... 212
来源：http://pb.jctech888.com.cn

Go ............. 212
来源：http://yf.bookmarksfly.cn

Ruby ........... 212
来源：http://rj.huixiangedu.cn

C# ............. 212
来源：http://sx.yuntaijiaju.cn

C .............. 30
来源：http://mr.chemitech.net.cn

C++ ............ 30
来源：http://ie.haigaiapp.cn

SQL ............ 90
来源：http://oa.panjiajie.cn

Bash ........... 80
来源：http://kl.wgjwhj.cn

Kotlin ......... 15
来源：http://ah.huixiangedu.cn

Swift .......... 15
来源：http://dj.szsharing.cn

Lua ............ 10
来源：http://zd.newstarts.cn

Perl ........... 10
来源：http://qe.szsharing.cn

Scala .......... 10
来源：http://jf.chemitech.net.cn

------------------------------------
来源：http://dj.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://bo.yuntaijiaju.cn

按章节统计：
来源：http://mc.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cr.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zm.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bj.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lt.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mk.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lq.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aj.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wj.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xn.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://op.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ya.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://br.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ii.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tb.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uj.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vg.huixiangedu.cn

Q SQL 专题                              90
来源：http://cn.shtwfgs.cn

R Bash 专题                             80
来源：http://oz.muxihuayi.cn

S C / C++ 专题                          60
来源：http://xs.colortex.cn

T 其他语言补充                          60
来源：http://su.jctech888.com.cn

U 高频实用片段                         120
来源：http://mo.nszjky.cn

------------------------------------
来源：http://gu.asd995.cn

合计                                  2106 条
来源：http://zb.asd995.cn

--------------------------------------------------------------------------------
来源：http://dj.shtwfgs.cn

使用提醒
来源：http://uw.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ym.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mt.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ri.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vi.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ze.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gl.jianghongdianzi.cn

—— 文件结束 ——
来源：http://hk.shtwfgs.cn

================================================================================
来源：http://rd.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://kn.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://yt.jctech888.com.cn

================================================================================
来源：http://ww.shxzskj.cn

【收录内容】
来源：http://ob.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mx.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gz.szsharing.cn

SQL · Bash · C · C++
来源：http://lv.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://is.huixinmuqiang.cn

【使用说明】
来源：http://bj.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://su.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kl.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://js.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hh.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qt.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qf.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ro.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nz.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://st.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gh.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yk.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pg.521024.cn

【文件统计】
来源：http://zs.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ip.asd995.cn

--------------------------------------------------------------------------------
来源：http://oq.jianghongdianzi.cn

目  录
来源：http://mr.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://na.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hh.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ys.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uw.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gc.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://co.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bj.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tj.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wl.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dn.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rs.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://er.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dm.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zo.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ni.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ou.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ro.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kl.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nb.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zs.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sm.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sk.hnjuh.cn

================================================================================
来源：http://mt.wgjwhj.cn

A. 基础语法与类型
来源：http://oi.shxzskj.cn

================================================================================
来源：http://ev.muxihuayi.cn

[A01] Hello World
来源：http://lc.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://pc.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://fn.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://ih.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zb.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://fb.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://zt.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://au.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nk.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ku.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rx.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pw.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ic.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hp.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://kg.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://qz.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://ll.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ta.szxytkj.cn

[A03] 常量定义
来源：http://js.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hy.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://ek.colortex.cn

JS:   const PI = 3.14159;
来源：http://qn.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://ev.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://fg.huanxung.cn

Go:   const PI = 3.14159
来源：http://ye.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://ts.521024.cn

C#:   const double PI = 3.14159;
来源：http://iv.panjiajie.cn

[A04] 判断变量类型
来源：http://xx.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mq.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aa.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yv.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://vo.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ek.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dr.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mc.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://rd.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://hm.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kh.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fs.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bj.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lv.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://sp.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://xa.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://nv.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://yq.huanxung.cn

[A06] 字符串转数字
来源：http://zp.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://gy.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ly.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zm.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sv.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cd.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dp.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qx.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nf.shxzskj.cn

[A07] 数字转字符串
来源：http://vj.colortex.cn

Py:   str(42)
来源：http://mb.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://zx.szsharing.cn

JS:   String(42); (42).toString()
来源：http://ur.chemitech.net.cn

TS:   String(42)
来源：http://um.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xc.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://rs.newstarts.cn

Ruby: 42.to_s
来源：http://xt.huixiangedu.cn

C#:   42.ToString()
来源：http://uk.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://hs.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wl.shxzskj.cn


<!-- 参考信息 -->