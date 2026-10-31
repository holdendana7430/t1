代发 wailian999

[U59] PHP：自定义排序
来源：http://jh.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tp.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://df.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bc.szxytkj.cn

[U61] PHP：正则
来源：http://bc.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zb.lnxyls.cn

[U62] PHP：日期对象
来源：http://ag.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kj.haigaiapp.cn

[U63] PHP：文件读写
来源：http://ll.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://by.shxzskj.cn

[U64] PHP：目录遍历
来源：http://sz.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://hv.panjiajie.cn

[U65] PHP：会话
来源：http://zk.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jl.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ny.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bg.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://zc.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vg.colortex.cn

[U68] PHP：PDO 连接
来源：http://ff.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kt.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://mb.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vq.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://yf.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hh.lnxyls.cn

[U71] PHP：抛出异常
来源：http://vy.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://rf.hahajie.cn

[U72] PHP：写错误日志
来源：http://zw.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://qv.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://rc.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://fy.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://hn.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://on.panjiajie.cn

[U75] PHP：依赖注入
来源：http://pk.yuexingan06.cn

composer require psr/container
来源：http://bs.chemitech.net.cn

[U76] PHP：简单路由
来源：http://kb.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lk.colortex.cn

[U77] PHP：模板渲染
来源：http://es.jctech888.com.cn

composer require twig/twig
来源：http://kj.muxihuayi.cn

[U78] PHP：单元测试
来源：http://xz.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://cu.muxihuayi.cn

[U79] PHP：静态分析
来源：http://fg.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://rs.nszjky.cn

[U80] PHP：代码规范修复
来源：http://kb.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zd.szxytkj.cn

[U81] JS：初始化项目
来源：http://zq.szsharing.cn

npm init -y;  npm i express
来源：http://qp.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://hj.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tc.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://rb.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gi.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://xi.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wy.nicolike.cn

[U85] JS：可选链
来源：http://yw.9csxet.cn

a?.b?.c
来源：http://ld.shxzukj.cn

[U86] JS：空值合并
来源：http://gz.muxihuayi.cn

a ?? b
来源：http://sd.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://yk.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://wx.521024.cn

[U88] JS：对象展开合并
来源：http://lh.521024.cn

{ ...a, ...b }
来源：http://up.jctech888.com.cn

[U89] JS：数组去重
来源：http://zy.yuntaijiaju.cn

[...new Set(arr)]
来源：http://ll.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://wd.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://wn.asd995.cn

[U91] JS：对象键值遍历
来源：http://hv.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uc.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://wa.jctech888.com.cn

structuredClone(obj)
来源：http://xp.wgjwhj.cn

[U93] JS：模板字符串
来源：http://rq.nicolike.cn

`共 ${n} 条`
来源：http://sb.shtwfgs.cn

[U94] JS：箭头函数
来源：http://ny.9csxet.cn

const double = x => x * 2;
来源：http://yw.521024.cn

[U95] JS：Promise 包装
来源：http://dh.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://ka.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://qj.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jj.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://eb.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yf.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://gs.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lu.asd995.cn

[U99] JS：事件监听
来源：http://is.nszjky.cn

el.addEventListener("click", e => {})
来源：http://qr.9csxet.cn

[U100] JS：DOM 查询
来源：http://bf.huanxung.cn

document.querySelector(".item")
来源：http://qe.hnjuh.cn

[U101] JS：classList 操作
来源：http://uc.9csxet.cn

el.classList.toggle("active")
来源：http://uh.huixiangedu.cn

[U102] JS：本地存储
来源：http://ro.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pc.jctech888.com.cn

[U103] JS：定时器
来源：http://hx.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ft.huixiangedu.cn

[U104] JS：防抖
来源：http://ju.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oz.haigaiapp.cn

[U105] JS：节流
来源：http://by.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wx.jctech888.com.cn

[U106] JS：日期格式化
来源：http://lr.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xh.yuexingan06.cn

[U107] JS：数字千分位
来源：http://cj.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yk.521024.cn

[U108] JS：随机整数
来源：http://fa.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vn.9csxet.cn

[U109] JS：数组分组
来源：http://uy.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://kt.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://nx.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nt.521024.cn

[U111] JS：对象转 Map
来源：http://uy.521024.cn

new Map(Object.entries(obj))
来源：http://xf.asd995.cn

[U112] JS：字符串补位
来源：http://ay.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://lr.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://rj.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://ou.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ux.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nd.huanxung.cn

[U115] JS：生成 UUID
来源：http://lg.nicolike.cn

crypto.randomUUID()
来源：http://og.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://hp.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://jk.hahajie.cn

[U117] JS：单元测试
来源：http://wj.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://xj.shtwfgs.cn

[U118] JS：开发服务器
来源：http://ph.shxzskj.cn

npm i -D vite;  npx vite
来源：http://ci.hnjuh.cn

[U119] JS：生产构建
来源：http://xj.szsharing.cn

npx vite build
来源：http://qr.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://sl.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://ic.szxytkj.cn

================================================================================
来源：http://em.nicolike.cn

统计汇总
来源：http://st.9csxet.cn

================================================================================
来源：http://ns.bookmarksfly.cn

按语言统计（条）：
来源：http://zm.lnxyls.cn

Python ......... 252
来源：http://au.huanxung.cn

PHP ............ 252
来源：http://dt.huixinmuqiang.cn

JavaScript ..... 252
来源：http://qc.nszjky.cn

TypeScript ..... 212
来源：http://db.asd995.cn

Java ........... 212
来源：http://qa.nicolike.cn

Go ............. 212
来源：http://sx.huanxung.cn

Ruby ........... 212
来源：http://rb.huanxung.cn

C# ............. 212
来源：http://hp.haigaiapp.cn

C .............. 30
来源：http://yq.lnxyls.cn

C++ ............ 30
来源：http://ib.newstarts.cn

SQL ............ 90
来源：http://le.muxihuayi.cn

Bash ........... 80
来源：http://tl.yuexingan06.cn

Kotlin ......... 15
来源：http://yb.lnxyls.cn

Swift .......... 15
来源：http://ok.huixinmuqiang.cn

Lua ............ 10
来源：http://jw.panjiajie.cn

Perl ........... 10
来源：http://do.wgjwhj.cn

Scala .......... 10
来源：http://ad.nszjky.cn

------------------------------------
来源：http://uc.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://cd.wgjwhj.cn

按章节统计：
来源：http://mi.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yn.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jj.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dw.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://id.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bp.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ha.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nk.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jt.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pn.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aq.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://of.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iw.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vs.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://be.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ya.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wh.huanxung.cn

Q SQL 专题                              90
来源：http://qx.jianghongdianzi.cn

R Bash 专题                             80
来源：http://mh.szsharing.cn

S C / C++ 专题                          60
来源：http://jd.huixiangedu.cn

T 其他语言补充                          60
来源：http://ip.chemitech.net.cn

U 高频实用片段                         120
来源：http://jh.asd995.cn

------------------------------------
来源：http://cv.chemitech.net.cn

合计                                  2106 条
来源：http://zn.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://av.gzmigu.cn

使用提醒
来源：http://sf.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://bk.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dr.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qo.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lq.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gm.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jm.bjjhwx.cn

—— 文件结束 ——
来源：http://wr.huixinmuqiang.cn

================================================================================
来源：http://rb.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://fm.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://hh.hnjuh.cn

================================================================================
来源：http://iz.huanxung.cn

【收录内容】
来源：http://zo.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sm.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ik.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://ar.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qm.shxzukj.cn

【使用说明】
来源：http://aj.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nq.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vm.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sf.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jg.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xf.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oo.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kv.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ky.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://os.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://as.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cq.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pi.jctech888.com.cn

【文件统计】
来源：http://we.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hb.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://vp.nicolike.cn

目  录
来源：http://qw.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://nv.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ab.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gl.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://es.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://da.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pu.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://up.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ug.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://um.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yt.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://at.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://om.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hu.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://je.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wz.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gb.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hn.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vu.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iv.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ge.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pr.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qb.521024.cn

================================================================================
来源：http://hv.shxzukj.cn

A. 基础语法与类型
来源：http://gp.jianghongdianzi.cn

================================================================================
来源：http://fw.colortex.cn

[A01] Hello World
来源：http://tm.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://mj.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://fv.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://gn.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hj.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://jk.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ms.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://rd.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dl.asd995.cn

[A02] 变量声明与赋值
来源：http://ll.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ti.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tn.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ay.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://as.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://xu.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://bd.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://tk.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ed.jctech888.com.cn

[A03] 常量定义
来源：http://jp.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yq.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://cw.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://ot.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://oz.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://vv.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://ar.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://qu.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://di.szsharing.cn

[A04] 判断变量类型
来源：http://mg.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xu.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dr.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aa.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://dg.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pm.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fk.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tg.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://qv.shxzukj.cn

[A05] 整数除法与取模
来源：http://yu.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oz.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://au.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cb.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vb.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://ao.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://bv.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://gm.521024.cn

C#:   7 / 2; 7 % 2
来源：http://ic.huixiangedu.cn

[A06] 字符串转数字
来源：http://ow.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://rf.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ge.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jd.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sj.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pc.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ne.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lr.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sa.asd995.cn

[A07] 数字转字符串
来源：http://wv.wgjwhj.cn

Py:   str(42)
来源：http://re.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://ec.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://ek.huanxung.cn

TS:   String(42)
来源：http://pk.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zq.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://zq.lnxyls.cn

Ruby: 42.to_s
来源：http://yk.colortex.cn

C#:   42.ToString()
来源：http://ji.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://th.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oz.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tu.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uf.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ne.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ca.wgjwhj.cn


<!-- 参考信息 -->