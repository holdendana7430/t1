代发 wailian999

[U55] PHP：match 表达式
来源：http://xf.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://de.hahajie.cn

[U56] PHP：命名参数
来源：http://ey.szxytkj.cn

f(a: 1, b: 2)
来源：http://nz.nicolike.cn

[U57] PHP：字符串插值
来源：http://hb.yuntaijiaju.cn

"值: {$a}"
来源：http://fx.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://sn.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rk.asd995.cn

[U59] PHP：自定义排序
来源：http://zt.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ep.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://ma.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wx.huanxung.cn

[U61] PHP：正则
来源：http://bm.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sh.shtwfgs.cn

[U62] PHP：日期对象
来源：http://rf.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wt.colortex.cn

[U63] PHP：文件读写
来源：http://lr.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ly.hahajie.cn

[U64] PHP：目录遍历
来源：http://dv.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://wy.521024.cn

[U65] PHP：会话
来源：http://lm.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eh.521024.cn

[U66] PHP：设置 Cookie
来源：http://lp.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ag.nszjky.cn

[U67] PHP：处理文件上传
来源：http://eq.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mf.szsharing.cn

[U68] PHP：PDO 连接
来源：http://xw.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cm.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://iy.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kq.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://vo.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gl.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://eu.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://mx.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://bi.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ch.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://ve.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://hq.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://yk.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://rb.nicolike.cn

[U75] PHP：依赖注入
来源：http://xw.shtwfgs.cn

composer require psr/container
来源：http://rp.jctech888.com.cn

[U76] PHP：简单路由
来源：http://su.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vf.shxzskj.cn

[U77] PHP：模板渲染
来源：http://fb.521024.cn

composer require twig/twig
来源：http://ut.bjjhwx.cn

[U78] PHP：单元测试
来源：http://ot.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://sy.hnjuh.cn

[U79] PHP：静态分析
来源：http://kk.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://qc.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://cm.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iv.newstarts.cn

[U81] JS：初始化项目
来源：http://jt.panjiajie.cn

npm init -y;  npm i express
来源：http://pu.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://mi.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xt.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://zb.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mc.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://tv.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mj.gzmigu.cn

[U85] JS：可选链
来源：http://od.huanxung.cn

a?.b?.c
来源：http://lh.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://ko.szsharing.cn

a ?? b
来源：http://zx.nicolike.cn

[U87] JS：解构默认值
来源：http://jh.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://wr.521024.cn

[U88] JS：对象展开合并
来源：http://pm.haigaiapp.cn

{ ...a, ...b }
来源：http://dt.shxzukj.cn

[U89] JS：数组去重
来源：http://sx.colortex.cn

[...new Set(arr)]
来源：http://zf.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://qw.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://jd.hahajie.cn

[U91] JS：对象键值遍历
来源：http://zr.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ip.wgjwhj.cn

[U92] JS：深拷贝
来源：http://ws.asd995.cn

structuredClone(obj)
来源：http://bh.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://ht.newstarts.cn

`共 ${n} 条`
来源：http://wg.newstarts.cn

[U94] JS：箭头函数
来源：http://ee.shxzskj.cn

const double = x => x * 2;
来源：http://to.lnxyls.cn

[U95] JS：Promise 包装
来源：http://ht.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://op.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://zv.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gl.asd995.cn

[U97] JS：并发请求
来源：http://nr.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://ue.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xq.shxzskj.cn

[U99] JS：事件监听
来源：http://eg.9csxet.cn

el.addEventListener("click", e => {})
来源：http://ut.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://nv.9csxet.cn

document.querySelector(".item")
来源：http://uh.colortex.cn

[U101] JS：classList 操作
来源：http://yw.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://wi.nicolike.cn

[U102] JS：本地存储
来源：http://vk.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ak.chemitech.net.cn

[U103] JS：定时器
来源：http://kd.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tj.nszjky.cn

[U104] JS：防抖
来源：http://yi.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xq.colortex.cn

[U105] JS：节流
来源：http://fi.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lb.colortex.cn

[U106] JS：日期格式化
来源：http://jq.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qi.gzmigu.cn

[U107] JS：数字千分位
来源：http://xe.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ev.gzmigu.cn

[U108] JS：随机整数
来源：http://lt.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oq.asd995.cn

[U109] JS：数组分组
来源：http://ia.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://hg.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://uv.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nz.lnxyls.cn

[U111] JS：对象转 Map
来源：http://uc.newstarts.cn

new Map(Object.entries(obj))
来源：http://pz.panjiajie.cn

[U112] JS：字符串补位
来源：http://uu.jctech888.com.cn

"7".padStart(3, "0")
来源：http://ph.asd995.cn

[U113] JS：正则替换全部
来源：http://xe.shxzukj.cn

s.replaceAll("a", "b")
来源：http://uz.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://vd.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://en.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://xz.hnjuh.cn

crypto.randomUUID()
来源：http://ff.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://fv.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://is.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://ld.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://rj.colortex.cn

[U118] JS：开发服务器
来源：http://rw.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://sq.szsharing.cn

[U119] JS：生产构建
来源：http://hq.bjjhwx.cn

npx vite build
来源：http://jb.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://zy.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://en.bjjhwx.cn

================================================================================
来源：http://ld.huixinmuqiang.cn

统计汇总
来源：http://tf.jianghongdianzi.cn

================================================================================
来源：http://zj.newstarts.cn

按语言统计（条）：
来源：http://rk.hahajie.cn

Python ......... 252
来源：http://ic.muxihuayi.cn

PHP ............ 252
来源：http://eh.lnxyls.cn

JavaScript ..... 252
来源：http://xy.lnxyls.cn

TypeScript ..... 212
来源：http://mz.huixinmuqiang.cn

Java ........... 212
来源：http://sx.newstarts.cn

Go ............. 212
来源：http://hz.asd995.cn

Ruby ........... 212
来源：http://ws.gzmigu.cn

C# ............. 212
来源：http://jz.shxzukj.cn

C .............. 30
来源：http://kc.521024.cn

C++ ............ 30
来源：http://ia.chemitech.net.cn

SQL ............ 90
来源：http://op.panjiajie.cn

Bash ........... 80
来源：http://xa.lnxyls.cn

Kotlin ......... 15
来源：http://zp.szxytkj.cn

Swift .......... 15
来源：http://ym.haigaiapp.cn

Lua ............ 10
来源：http://eb.wgjwhj.cn

Perl ........... 10
来源：http://dp.shxzskj.cn

Scala .......... 10
来源：http://cg.nszjky.cn

------------------------------------
来源：http://vr.hnjuh.cn

合计 ........... 2106 条
来源：http://lq.wgjwhj.cn

按章节统计：
来源：http://st.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ss.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pu.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://by.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hn.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tf.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mn.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hh.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ep.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lh.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bq.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nv.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ww.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://js.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pp.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://er.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oz.newstarts.cn

Q SQL 专题                              90
来源：http://gi.nicolike.cn

R Bash 专题                             80
来源：http://kw.haigaiapp.cn

S C / C++ 专题                          60
来源：http://ld.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://go.hnjuh.cn

U 高频实用片段                         120
来源：http://gy.haigaiapp.cn

------------------------------------
来源：http://fg.szxytkj.cn

合计                                  2106 条
来源：http://am.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://qe.hnjuh.cn

使用提醒
来源：http://rv.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://vz.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pz.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kb.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ak.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dq.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gc.nicolike.cn

—— 文件结束 ——
来源：http://kc.nicolike.cn

================================================================================
来源：http://wy.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://cd.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://am.gzmigu.cn

================================================================================
来源：http://jf.yuntaijiaju.cn

【收录内容】
来源：http://dk.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jr.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qk.asd995.cn

SQL · Bash · C · C++
来源：http://xl.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pe.yuexingan06.cn

【使用说明】
来源：http://gs.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pq.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ik.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://la.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pj.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rl.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gc.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tx.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iu.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xh.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dn.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lr.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dk.chemitech.net.cn

【文件统计】
来源：http://pi.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rf.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://cu.shtwfgs.cn

目  录
来源：http://pq.hahajie.cn

--------------------------------------------------------------------------------
来源：http://tf.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cn.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zo.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oa.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fh.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rv.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rd.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yy.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wj.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://av.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gc.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mx.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ds.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rv.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lf.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://on.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pw.nicolike.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kx.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ny.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ua.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://za.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mv.nszjky.cn

================================================================================
来源：http://rp.newstarts.cn

A. 基础语法与类型
来源：http://qy.jianghongdianzi.cn

================================================================================
来源：http://cp.wgjwhj.cn

[A01] Hello World
来源：http://eo.szxytkj.cn

Py:   print("Hello, World!")
来源：http://jl.colortex.cn

PHP:  echo "Hello, World!";
来源：http://kp.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://im.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pl.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://sa.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://rl.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://lf.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fd.nszjky.cn

[A02] 变量声明与赋值
来源：http://mr.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://of.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ek.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ew.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hm.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://cs.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://op.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://gx.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pq.hahajie.cn

[A03] 常量定义
来源：http://pj.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://us.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://hb.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://ei.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://dz.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://yv.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://cp.shxzukj.cn

Ruby: PI = 3.14159
来源：http://hk.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://jw.szxytkj.cn

[A04] 判断变量类型
来源：http://jq.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xh.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wn.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pe.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://ah.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yr.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nk.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ju.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://tr.newstarts.cn

[A05] 整数除法与取模
来源：http://mv.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gj.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iv.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://av.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ou.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://yi.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://qg.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://jo.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://hh.panjiajie.cn

[A06] 字符串转数字
来源：http://hq.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://tn.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zh.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qo.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wg.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vv.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dy.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lw.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zr.huanxung.cn

[A07] 数字转字符串
来源：http://oe.nicolike.cn

Py:   str(42)
来源：http://ib.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://mw.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://sp.huixiangedu.cn

TS:   String(42)
来源：http://rw.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qv.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://xw.shtwfgs.cn


<!-- 参考信息 -->