代发 wailian999

[U57] PHP：字符串插值
来源：http://pd.lnxyls.cn

"值: {$a}"
来源：http://uf.colortex.cn

[U58] PHP：数组三件套
来源：http://rv.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://te.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://he.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zg.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://rz.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ge.hnjuh.cn

[U61] PHP：正则
来源：http://zn.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lt.nszjky.cn

[U62] PHP：日期对象
来源：http://xs.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ho.nszjky.cn

[U63] PHP：文件读写
来源：http://zj.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://de.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://lv.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://zm.asd995.cn

[U65] PHP：会话
来源：http://md.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kq.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://iu.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hb.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://zr.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sp.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://lo.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bb.asd995.cn

[U69] PHP：PDO 预处理
来源：http://yv.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mi.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://gk.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hj.hnjuh.cn

[U71] PHP：抛出异常
来源：http://iv.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://ed.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://op.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://mb.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://zc.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://ra.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://bq.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://hy.hnjuh.cn

[U75] PHP：依赖注入
来源：http://ux.9csxet.cn

composer require psr/container
来源：http://uj.panjiajie.cn

[U76] PHP：简单路由
来源：http://jh.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pb.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://zy.yuexingan06.cn

composer require twig/twig
来源：http://rg.panjiajie.cn

[U78] PHP：单元测试
来源：http://uv.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://rz.yuexingan06.cn

[U79] PHP：静态分析
来源：http://we.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://jl.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://gf.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ld.huixiangedu.cn

[U81] JS：初始化项目
来源：http://wf.hahajie.cn

npm init -y;  npm i express
来源：http://se.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://zj.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kj.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://bv.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ay.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ze.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vb.hnjuh.cn

[U85] JS：可选链
来源：http://dg.huixiangedu.cn

a?.b?.c
来源：http://qo.shxzukj.cn

[U86] JS：空值合并
来源：http://ym.lnxyls.cn

a ?? b
来源：http://dr.szxytkj.cn

[U87] JS：解构默认值
来源：http://kx.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://zi.hahajie.cn

[U88] JS：对象展开合并
来源：http://je.wgjwhj.cn

{ ...a, ...b }
来源：http://um.asd995.cn

[U89] JS：数组去重
来源：http://ot.szsharing.cn

[...new Set(arr)]
来源：http://ex.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://yd.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://dt.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://au.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bh.521024.cn

[U92] JS：深拷贝
来源：http://xe.szsharing.cn

structuredClone(obj)
来源：http://mp.9csxet.cn

[U93] JS：模板字符串
来源：http://df.shxzskj.cn

`共 ${n} 条`
来源：http://gj.panjiajie.cn

[U94] JS：箭头函数
来源：http://ek.szxytkj.cn

const double = x => x * 2;
来源：http://lh.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://nr.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://ya.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://tg.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ju.wgjwhj.cn

[U97] JS：并发请求
来源：http://qg.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oz.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://uo.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ro.gzmigu.cn

[U99] JS：事件监听
来源：http://oj.szsharing.cn

el.addEventListener("click", e => {})
来源：http://vb.hnjuh.cn

[U100] JS：DOM 查询
来源：http://op.chemitech.net.cn

document.querySelector(".item")
来源：http://hy.bjjhwx.cn

[U101] JS：classList 操作
来源：http://iv.521024.cn

el.classList.toggle("active")
来源：http://fy.nicolike.cn

[U102] JS：本地存储
来源：http://rl.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ks.szsharing.cn

[U103] JS：定时器
来源：http://vo.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lh.shxzukj.cn

[U104] JS：防抖
来源：http://ir.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hk.9csxet.cn

[U105] JS：节流
来源：http://kg.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xj.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://eu.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ti.chemitech.net.cn

[U107] JS：数字千分位
来源：http://ki.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://os.chemitech.net.cn

[U108] JS：随机整数
来源：http://rt.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://by.asd995.cn

[U109] JS：数组分组
来源：http://mf.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://lb.nszjky.cn

[U110] JS：数组分块
来源：http://lo.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uj.newstarts.cn

[U111] JS：对象转 Map
来源：http://ku.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://rt.haigaiapp.cn

[U112] JS：字符串补位
来源：http://af.colortex.cn

"7".padStart(3, "0")
来源：http://ee.shxzukj.cn

[U113] JS：正则替换全部
来源：http://fb.hnjuh.cn

s.replaceAll("a", "b")
来源：http://cb.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://ew.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xk.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://ih.haigaiapp.cn

crypto.randomUUID()
来源：http://qd.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://vh.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://jz.szxytkj.cn

[U117] JS：单元测试
来源：http://ev.colortex.cn

npm i -D vitest;  npx vitest
来源：http://nx.haigaiapp.cn

[U118] JS：开发服务器
来源：http://rw.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://ew.chemitech.net.cn

[U119] JS：生产构建
来源：http://li.jctech888.com.cn

npx vite build
来源：http://te.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://jq.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://oj.9csxet.cn

================================================================================
来源：http://cg.shxzskj.cn

统计汇总
来源：http://bf.wgjwhj.cn

================================================================================
来源：http://wm.bookmarksfly.cn

按语言统计（条）：
来源：http://nt.huixinmuqiang.cn

Python ......... 252
来源：http://yv.jianghongdianzi.cn

PHP ............ 252
来源：http://zw.newstarts.cn

JavaScript ..... 252
来源：http://me.asd995.cn

TypeScript ..... 212
来源：http://fv.huixinmuqiang.cn

Java ........... 212
来源：http://pl.nicolike.cn

Go ............. 212
来源：http://rw.bookmarksfly.cn

Ruby ........... 212
来源：http://wl.chemitech.net.cn

C# ............. 212
来源：http://yj.huanxung.cn

C .............. 30
来源：http://xy.szxytkj.cn

C++ ............ 30
来源：http://fp.szsharing.cn

SQL ............ 90
来源：http://uo.shtwfgs.cn

Bash ........... 80
来源：http://ok.panjiajie.cn

Kotlin ......... 15
来源：http://rm.muxihuayi.cn

Swift .......... 15
来源：http://no.hahajie.cn

Lua ............ 10
来源：http://zl.shtwfgs.cn

Perl ........... 10
来源：http://ob.haigaiapp.cn

Scala .......... 10
来源：http://ca.jianghongdianzi.cn

------------------------------------
来源：http://od.newstarts.cn

合计 ........... 2106 条
来源：http://pi.hnjuh.cn

按章节统计：
来源：http://uh.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pk.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nz.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xa.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kh.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vv.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lz.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://co.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tn.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jk.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fa.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tw.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eq.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ib.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wu.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://om.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fn.shtwfgs.cn

Q SQL 专题                              90
来源：http://dp.szxytkj.cn

R Bash 专题                             80
来源：http://gx.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://rs.shtwfgs.cn

T 其他语言补充                          60
来源：http://pk.yuexingan06.cn

U 高频实用片段                         120
来源：http://de.hahajie.cn

------------------------------------
来源：http://cn.huixiangedu.cn

合计                                  2106 条
来源：http://ab.huanxung.cn

--------------------------------------------------------------------------------
来源：http://dg.shxzukj.cn

使用提醒
来源：http://ih.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://hu.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kq.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ji.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://je.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ji.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mu.nicolike.cn

—— 文件结束 ——
来源：http://sc.lnxyls.cn

================================================================================
来源：http://mn.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://cv.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://ig.yuexingan06.cn

================================================================================
来源：http://lj.huanxung.cn

【收录内容】
来源：http://gl.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zo.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://es.panjiajie.cn

SQL · Bash · C · C++
来源：http://vy.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://np.shxzskj.cn

【使用说明】
来源：http://pb.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ig.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qw.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mz.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ww.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bb.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sa.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lh.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wv.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mj.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bm.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yw.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hx.nszjky.cn

【文件统计】
来源：http://fr.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vk.nicolike.cn

--------------------------------------------------------------------------------
来源：http://aw.yuntaijiaju.cn

目  录
来源：http://rm.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://zv.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lf.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://us.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kj.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ca.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uy.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qh.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yj.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ek.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lp.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tm.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jw.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cz.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lm.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vp.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eb.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ms.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ry.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kx.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://if.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dw.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dw.bookmarksfly.cn

================================================================================
来源：http://mj.9csxet.cn

A. 基础语法与类型
来源：http://ef.bjjhwx.cn

================================================================================
来源：http://le.yuexingan06.cn

[A01] Hello World
来源：http://ii.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://pg.asd995.cn

PHP:  echo "Hello, World!";
来源：http://ou.asd995.cn

JS:   console.log("Hello, World!");
来源：http://hm.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gq.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://wn.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://oi.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://lf.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yp.newstarts.cn

[A02] 变量声明与赋值
来源：http://tm.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bt.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jr.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vc.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://on.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://el.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://ji.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://qk.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ou.huanxung.cn

[A03] 常量定义
来源：http://un.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xw.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://rp.huanxung.cn

JS:   const PI = 3.14159;
来源：http://da.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://wy.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://ng.szsharing.cn

Go:   const PI = 3.14159
来源：http://er.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://ji.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://im.shtwfgs.cn

[A04] 判断变量类型
来源：http://nk.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xq.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fm.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xk.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://mt.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lv.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hu.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fo.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://cw.haigaiapp.cn

[A05] 整数除法与取模
来源：http://fs.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zk.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kv.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oh.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vk.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://ms.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://hu.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://si.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://lk.nszjky.cn

[A06] 字符串转数字
来源：http://no.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://it.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mq.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yf.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://py.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ut.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oi.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ne.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sy.szxytkj.cn

[A07] 数字转字符串
来源：http://qo.hahajie.cn

Py:   str(42)
来源：http://vj.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://nw.521024.cn

JS:   String(42); (42).toString()
来源：http://qg.asd995.cn

TS:   String(42)
来源：http://wy.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qh.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://gn.gzmigu.cn

Ruby: 42.to_s
来源：http://jn.lnxyls.cn

C#:   42.ToString()
来源：http://wu.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://li.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mn.shtwfgs.cn


<!-- 参考信息 -->