代发 wailian999

[U49] PHP：只读属性
来源：http://hg.nszjky.cn

public readonly string $name
来源：http://su.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ls.hahajie.cn

public function __construct(private int $id) {}
来源：http://ph.chemitech.net.cn

[U51] PHP：数组解构
来源：http://uj.newstarts.cn

[$a, $b] = $arr;
来源：http://bu.nicolike.cn

[U52] PHP：箭头函数
来源：http://kc.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://ym.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ak.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://tj.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://ip.panjiajie.cn

$obj?->method()
来源：http://th.asd995.cn

[U55] PHP：match 表达式
来源：http://nl.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jw.gzmigu.cn

[U56] PHP：命名参数
来源：http://lh.521024.cn

f(a: 1, b: 2)
来源：http://pr.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://lk.hahajie.cn

"值: {$a}"
来源：http://ho.nicolike.cn

[U58] PHP：数组三件套
来源：http://qg.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zi.lnxyls.cn

[U59] PHP：自定义排序
来源：http://yr.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mj.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://ne.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dl.colortex.cn

[U61] PHP：正则
来源：http://kj.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wg.panjiajie.cn

[U62] PHP：日期对象
来源：http://sj.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bk.colortex.cn

[U63] PHP：文件读写
来源：http://ap.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bs.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://ty.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://kk.hahajie.cn

[U65] PHP：会话
来源：http://fw.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zl.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://pg.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dm.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://if.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tn.9csxet.cn

[U68] PHP：PDO 连接
来源：http://er.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://un.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://wj.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zb.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://cs.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gg.521024.cn

[U71] PHP：抛出异常
来源：http://uj.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://we.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://sq.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://ul.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://yz.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://qu.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://qo.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://je.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://im.nszjky.cn

composer require psr/container
来源：http://hg.nszjky.cn

[U76] PHP：简单路由
来源：http://sa.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ya.hnjuh.cn

[U77] PHP：模板渲染
来源：http://at.gzmigu.cn

composer require twig/twig
来源：http://ja.shxzskj.cn

[U78] PHP：单元测试
来源：http://mf.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://hb.panjiajie.cn

[U79] PHP：静态分析
来源：http://my.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://px.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://yg.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://si.panjiajie.cn

[U81] JS：初始化项目
来源：http://yk.lnxyls.cn

npm init -y;  npm i express
来源：http://da.newstarts.cn

[U82] JS：package.json 脚本
来源：http://bv.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ul.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://cx.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fx.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://pk.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vn.colortex.cn

[U85] JS：可选链
来源：http://do.bookmarksfly.cn

a?.b?.c
来源：http://fa.hahajie.cn

[U86] JS：空值合并
来源：http://ji.asd995.cn

a ?? b
来源：http://zg.nszjky.cn

[U87] JS：解构默认值
来源：http://vy.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://fd.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://dp.wgjwhj.cn

{ ...a, ...b }
来源：http://sq.huanxung.cn

[U89] JS：数组去重
来源：http://wf.hnjuh.cn

[...new Set(arr)]
来源：http://ma.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ei.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://tm.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://da.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tp.huanxung.cn

[U92] JS：深拷贝
来源：http://nk.muxihuayi.cn

structuredClone(obj)
来源：http://qn.yuexingan06.cn

[U93] JS：模板字符串
来源：http://pt.szxytkj.cn

`共 ${n} 条`
来源：http://hg.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://gs.colortex.cn

const double = x => x * 2;
来源：http://hl.shxzukj.cn

[U95] JS：Promise 包装
来源：http://kl.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://ip.asd995.cn

[U96] JS：async/await 与异常
来源：http://gs.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ds.szsharing.cn

[U97] JS：并发请求
来源：http://sx.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sv.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://uu.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qa.panjiajie.cn

[U99] JS：事件监听
来源：http://sc.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://ft.huanxung.cn

[U100] JS：DOM 查询
来源：http://hv.521024.cn

document.querySelector(".item")
来源：http://pp.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://cg.jctech888.com.cn

el.classList.toggle("active")
来源：http://uo.asd995.cn

[U102] JS：本地存储
来源：http://zs.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ns.gzmigu.cn

[U103] JS：定时器
来源：http://fd.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nz.hnjuh.cn

[U104] JS：防抖
来源：http://po.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wa.521024.cn

[U105] JS：节流
来源：http://sv.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zb.haigaiapp.cn

[U106] JS：日期格式化
来源：http://gw.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xa.colortex.cn

[U107] JS：数字千分位
来源：http://yp.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bj.hnjuh.cn

[U108] JS：随机整数
来源：http://aq.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pl.shxzukj.cn

[U109] JS：数组分组
来源：http://tg.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ua.bjjhwx.cn

[U110] JS：数组分块
来源：http://ye.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xz.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ke.lnxyls.cn

new Map(Object.entries(obj))
来源：http://kh.muxihuayi.cn

[U112] JS：字符串补位
来源：http://po.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://th.asd995.cn

[U113] JS：正则替换全部
来源：http://kx.lnxyls.cn

s.replaceAll("a", "b")
来源：http://th.colortex.cn

[U114] JS：JSON 深比较
来源：http://eu.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jv.hnjuh.cn

[U115] JS：生成 UUID
来源：http://xe.asd995.cn

crypto.randomUUID()
来源：http://kq.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://ld.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://vq.newstarts.cn

[U117] JS：单元测试
来源：http://gc.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://np.jctech888.com.cn

[U118] JS：开发服务器
来源：http://lk.newstarts.cn

npm i -D vite;  npx vite
来源：http://wl.jctech888.com.cn

[U119] JS：生产构建
来源：http://xb.jctech888.com.cn

npx vite build
来源：http://lj.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://yz.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://ua.szsharing.cn

================================================================================
来源：http://ey.huanxung.cn

统计汇总
来源：http://nr.colortex.cn

================================================================================
来源：http://nr.shtwfgs.cn

按语言统计（条）：
来源：http://go.hnjuh.cn

Python ......... 252
来源：http://yl.yuexingan06.cn

PHP ............ 252
来源：http://mt.huixinmuqiang.cn

JavaScript ..... 252
来源：http://zm.muxihuayi.cn

TypeScript ..... 212
来源：http://fc.jianghongdianzi.cn

Java ........... 212
来源：http://rr.shxzukj.cn

Go ............. 212
来源：http://xz.jctech888.com.cn

Ruby ........... 212
来源：http://yx.szsharing.cn

C# ............. 212
来源：http://pv.nszjky.cn

C .............. 30
来源：http://do.huixinmuqiang.cn

C++ ............ 30
来源：http://wl.huixiangedu.cn

SQL ............ 90
来源：http://tv.9csxet.cn

Bash ........... 80
来源：http://rv.chemitech.net.cn

Kotlin ......... 15
来源：http://ga.521024.cn

Swift .......... 15
来源：http://jt.yuexingan06.cn

Lua ............ 10
来源：http://dp.jctech888.com.cn

Perl ........... 10
来源：http://qp.shxzskj.cn

Scala .......... 10
来源：http://hb.huixinmuqiang.cn

------------------------------------
来源：http://tf.huixiangedu.cn

合计 ........... 2106 条
来源：http://xp.yuexingan06.cn

按章节统计：
来源：http://eu.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cv.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jh.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hb.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wo.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://an.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://an.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rp.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://df.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uy.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iw.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ct.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://em.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://td.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://td.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zd.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ln.lnxyls.cn

Q SQL 专题                              90
来源：http://cd.bjjhwx.cn

R Bash 专题                             80
来源：http://ct.colortex.cn

S C / C++ 专题                          60
来源：http://mm.chemitech.net.cn

T 其他语言补充                          60
来源：http://xi.hahajie.cn

U 高频实用片段                         120
来源：http://ut.lnxyls.cn

------------------------------------
来源：http://bv.chemitech.net.cn

合计                                  2106 条
来源：http://qz.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ke.jianghongdianzi.cn

使用提醒
来源：http://nc.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://hs.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yc.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ru.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://or.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iq.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qy.asd995.cn

—— 文件结束 ——
来源：http://ie.yuntaijiaju.cn

================================================================================
来源：http://ud.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://ee.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://nl.haigaiapp.cn

================================================================================
来源：http://ip.hnjuh.cn

【收录内容】
来源：http://ll.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fv.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fz.newstarts.cn

SQL · Bash · C · C++
来源：http://fx.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tk.gzmigu.cn

【使用说明】
来源：http://ne.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zj.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fb.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tl.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cr.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yl.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ph.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uo.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ur.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xr.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://it.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ev.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nv.bjjhwx.cn

【文件统计】
来源：http://uh.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://as.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://wz.yuntaijiaju.cn

目  录
来源：http://cz.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://uc.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hy.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zo.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ck.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tz.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uq.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kp.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vd.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wk.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ij.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://df.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mt.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gi.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vr.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qh.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nk.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xp.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tg.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bc.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://br.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lb.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cr.hahajie.cn

================================================================================
来源：http://lu.9csxet.cn

A. 基础语法与类型
来源：http://fj.colortex.cn

================================================================================
来源：http://er.colortex.cn

[A01] Hello World
来源：http://va.szsharing.cn

Py:   print("Hello, World!")
来源：http://ij.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://ch.colortex.cn

JS:   console.log("Hello, World!");
来源：http://fj.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wn.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://ws.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://hw.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://xe.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ax.huanxung.cn

[A02] 变量声明与赋值
来源：http://ey.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qx.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pr.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ut.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ck.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://kb.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://qw.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://wz.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rm.521024.cn

[A03] 常量定义
来源：http://jg.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bq.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://jy.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://wg.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ie.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://rh.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://zp.hahajie.cn

Ruby: PI = 3.14159
来源：http://pv.asd995.cn

C#:   const double PI = 3.14159;
来源：http://kb.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://vp.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ga.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uo.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ul.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://jk.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ar.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kb.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://du.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://ur.lnxyls.cn

[A05] 整数除法与取模
来源：http://if.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qu.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://js.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://md.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fi.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://iu.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://zo.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://ha.521024.cn

C#:   7 / 2; 7 % 2
来源：http://zy.jctech888.com.cn

[A06] 字符串转数字
来源：http://pe.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://su.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hk.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zz.huixinmuqiang.cn


<!-- 参考信息 -->