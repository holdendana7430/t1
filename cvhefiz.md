代发 wailian999

[U63] PHP：文件读写
来源：http://rd.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xz.gzmigu.cn

[U64] PHP：目录遍历
来源：http://cc.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ap.panjiajie.cn

[U65] PHP：会话
来源：http://ej.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://px.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://im.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bw.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://pb.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xe.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://uw.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wf.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://wm.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qh.521024.cn

[U70] PHP：PDO 事务
来源：http://ej.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nf.hnjuh.cn

[U71] PHP：抛出异常
来源：http://gv.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://gr.newstarts.cn

[U72] PHP：写错误日志
来源：http://vu.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://ll.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://az.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://dr.9csxet.cn

[U74] PHP：读取环境变量
来源：http://kt.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://sn.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://ni.hahajie.cn

composer require psr/container
来源：http://fj.jctech888.com.cn

[U76] PHP：简单路由
来源：http://uv.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kf.panjiajie.cn

[U77] PHP：模板渲染
来源：http://pr.panjiajie.cn

composer require twig/twig
来源：http://tx.gzmigu.cn

[U78] PHP：单元测试
来源：http://gb.521024.cn

composer require --dev phpunit/phpunit
来源：http://my.colortex.cn

[U79] PHP：静态分析
来源：http://fe.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://qx.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://hl.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bb.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://ye.haigaiapp.cn

npm init -y;  npm i express
来源：http://gz.nicolike.cn

[U82] JS：package.json 脚本
来源：http://lt.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zs.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://hp.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vt.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://jk.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ua.shtwfgs.cn

[U85] JS：可选链
来源：http://lo.shxzukj.cn

a?.b?.c
来源：http://ax.gzmigu.cn

[U86] JS：空值合并
来源：http://vf.chemitech.net.cn

a ?? b
来源：http://xv.szsharing.cn

[U87] JS：解构默认值
来源：http://wz.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://nt.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://ot.bookmarksfly.cn

{ ...a, ...b }
来源：http://hh.gzmigu.cn

[U89] JS：数组去重
来源：http://fv.521024.cn

[...new Set(arr)]
来源：http://bd.521024.cn

[U90] JS：数字数组排序
来源：http://js.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://bn.newstarts.cn

[U91] JS：对象键值遍历
来源：http://kd.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zw.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://qr.bookmarksfly.cn

structuredClone(obj)
来源：http://pb.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://cq.shtwfgs.cn

`共 ${n} 条`
来源：http://wb.nicolike.cn

[U94] JS：箭头函数
来源：http://mp.panjiajie.cn

const double = x => x * 2;
来源：http://qf.shxzukj.cn

[U95] JS：Promise 包装
来源：http://ct.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://cw.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://qb.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nm.huanxung.cn

[U97] JS：并发请求
来源：http://ue.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uq.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://uf.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rn.huanxung.cn

[U99] JS：事件监听
来源：http://mh.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://or.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://sr.szsharing.cn

document.querySelector(".item")
来源：http://ro.hahajie.cn

[U101] JS：classList 操作
来源：http://ed.shtwfgs.cn

el.classList.toggle("active")
来源：http://rn.panjiajie.cn

[U102] JS：本地存储
来源：http://vk.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ep.muxihuayi.cn

[U103] JS：定时器
来源：http://ww.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nl.huanxung.cn

[U104] JS：防抖
来源：http://au.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xy.521024.cn

[U105] JS：节流
来源：http://iw.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fl.asd995.cn

[U106] JS：日期格式化
来源：http://oe.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fq.shxzskj.cn

[U107] JS：数字千分位
来源：http://yo.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tn.huanxung.cn

[U108] JS：随机整数
来源：http://ns.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xp.huanxung.cn

[U109] JS：数组分组
来源：http://nb.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://qr.yuexingan06.cn

[U110] JS：数组分块
来源：http://in.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ob.hnjuh.cn

[U111] JS：对象转 Map
来源：http://iv.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://qz.panjiajie.cn

[U112] JS：字符串补位
来源：http://wq.hnjuh.cn

"7".padStart(3, "0")
来源：http://pk.hahajie.cn

[U113] JS：正则替换全部
来源：http://uw.gzmigu.cn

s.replaceAll("a", "b")
来源：http://ki.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://fj.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://du.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://fh.muxihuayi.cn

crypto.randomUUID()
来源：http://wb.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://nm.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://bt.panjiajie.cn

[U117] JS：单元测试
来源：http://su.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://yr.chemitech.net.cn

[U118] JS：开发服务器
来源：http://rb.nszjky.cn

npm i -D vite;  npx vite
来源：http://xa.colortex.cn

[U119] JS：生产构建
来源：http://ax.asd995.cn

npx vite build
来源：http://rd.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://ru.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://un.jctech888.com.cn

================================================================================
来源：http://de.gzmigu.cn

统计汇总
来源：http://ct.gzmigu.cn

================================================================================
来源：http://vo.gzmigu.cn

按语言统计（条）：
来源：http://to.yuntaijiaju.cn

Python ......... 252
来源：http://ji.521024.cn

PHP ............ 252
来源：http://sw.hahajie.cn

JavaScript ..... 252
来源：http://tn.shxzukj.cn

TypeScript ..... 212
来源：http://qi.wgjwhj.cn

Java ........... 212
来源：http://qa.colortex.cn

Go ............. 212
来源：http://cl.yuexingan06.cn

Ruby ........... 212
来源：http://qd.shxzskj.cn

C# ............. 212
来源：http://ni.gzmigu.cn

C .............. 30
来源：http://rc.jctech888.com.cn

C++ ............ 30
来源：http://yz.szsharing.cn

SQL ............ 90
来源：http://tr.chemitech.net.cn

Bash ........... 80
来源：http://vm.muxihuayi.cn

Kotlin ......... 15
来源：http://sq.bookmarksfly.cn

Swift .......... 15
来源：http://qs.muxihuayi.cn

Lua ............ 10
来源：http://uq.bookmarksfly.cn

Perl ........... 10
来源：http://im.yuexingan06.cn

Scala .......... 10
来源：http://zg.huixiangedu.cn

------------------------------------
来源：http://nd.shxzskj.cn

合计 ........... 2106 条
来源：http://vh.shtwfgs.cn

按章节统计：
来源：http://pt.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zf.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qu.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yl.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xy.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qm.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vk.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mm.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xq.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://op.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jd.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wr.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ee.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qi.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tr.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fv.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gh.hahajie.cn

Q SQL 专题                              90
来源：http://tl.chemitech.net.cn

R Bash 专题                             80
来源：http://wp.asd995.cn

S C / C++ 专题                          60
来源：http://yn.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://xr.bjjhwx.cn

U 高频实用片段                         120
来源：http://eb.shxzskj.cn

------------------------------------
来源：http://oe.shxzukj.cn

合计                                  2106 条
来源：http://xp.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ww.nicolike.cn

使用提醒
来源：http://uo.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://uf.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jv.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qz.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cv.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pi.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ip.huanxung.cn

—— 文件结束 ——
来源：http://av.shxzskj.cn

================================================================================
来源：http://jv.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://sb.asd995.cn

Common Programming Examples Cheat Book
来源：http://tx.521024.cn

================================================================================
来源：http://cd.asd995.cn

【收录内容】
来源：http://vc.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uc.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vu.gzmigu.cn

SQL · Bash · C · C++
来源：http://aj.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jb.nszjky.cn

【使用说明】
来源：http://xb.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lo.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bp.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rk.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bx.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fe.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zr.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sk.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://go.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://se.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sk.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gm.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dn.521024.cn

【文件统计】
来源：http://yb.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qx.hahajie.cn

--------------------------------------------------------------------------------
来源：http://zp.yuntaijiaju.cn

目  录
来源：http://ct.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://vv.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xs.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zc.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qn.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qe.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://up.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ay.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xf.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ec.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ig.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eo.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lh.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ms.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lr.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jo.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dr.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rg.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oa.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ep.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nj.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gn.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ce.muxihuayi.cn

================================================================================
来源：http://fw.colortex.cn

A. 基础语法与类型
来源：http://zs.hahajie.cn

================================================================================
来源：http://hr.gzmigu.cn

[A01] Hello World
来源：http://ki.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://vi.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://eo.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://ra.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hq.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ju.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://vi.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://ue.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ul.nicolike.cn

[A02] 变量声明与赋值
来源：http://dj.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kp.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rl.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oc.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eb.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://yq.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://lk.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://po.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cq.nicolike.cn

[A03] 常量定义
来源：http://dv.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://de.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://sn.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://wu.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://cn.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://th.nszjky.cn

Go:   const PI = 3.14159
来源：http://gy.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://do.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://tk.nicolike.cn

[A04] 判断变量类型
来源：http://fv.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uv.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oe.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zz.521024.cn

TS:   typeof x; x instanceof Date
来源：http://hm.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ge.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kp.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bw.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://bj.szxytkj.cn

[A05] 整数除法与取模
来源：http://et.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gx.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oq.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vg.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xw.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://uh.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://gk.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://vc.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://qj.wgjwhj.cn

[A06] 字符串转数字
来源：http://rs.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://ux.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://na.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ys.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bu.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://il.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xr.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gj.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hh.haigaiapp.cn

[A07] 数字转字符串
来源：http://on.bookmarksfly.cn

Py:   str(42)
来源：http://xm.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://do.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://uv.9csxet.cn

TS:   String(42)
来源：http://qd.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ss.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://gn.huanxung.cn

Ruby: 42.to_s
来源：http://yf.9csxet.cn

C#:   42.ToString()
来源：http://xt.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://az.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://en.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sm.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kb.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eu.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ue.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vb.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oh.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vi.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://pl.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rk.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://av.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wt.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tf.hnjuh.cn


<!-- 参考信息 -->