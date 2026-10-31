代发 wailian999

[U57] PHP：字符串插值
来源：http://jr.yuntaijiaju.cn

"值: {$a}"
来源：http://jw.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://yg.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://te.asd995.cn

[U59] PHP：自定义排序
来源：http://fe.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hx.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://gy.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rg.jianghongdianzi.cn

[U61] PHP：正则
来源：http://bf.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://md.hahajie.cn

[U62] PHP：日期对象
来源：http://bo.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xf.chemitech.net.cn

[U63] PHP：文件读写
来源：http://ha.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kd.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://is.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://tf.nicolike.cn

[U65] PHP：会话
来源：http://bg.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ra.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://rf.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fc.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://tk.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tt.521024.cn

[U68] PHP：PDO 连接
来源：http://fs.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wf.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://jr.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ui.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://ge.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zk.nszjky.cn

[U71] PHP：抛出异常
来源：http://ye.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://rp.panjiajie.cn

[U72] PHP：写错误日志
来源：http://ws.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://da.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://by.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://uh.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://xn.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://hw.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://yh.szsharing.cn

composer require psr/container
来源：http://tm.huanxung.cn

[U76] PHP：简单路由
来源：http://lb.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xf.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://dp.bookmarksfly.cn

composer require twig/twig
来源：http://be.521024.cn

[U78] PHP：单元测试
来源：http://xh.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://jn.shtwfgs.cn

[U79] PHP：静态分析
来源：http://jb.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://yk.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://fl.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fj.521024.cn

[U81] JS：初始化项目
来源：http://nk.chemitech.net.cn

npm init -y;  npm i express
来源：http://is.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://pr.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vb.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://jo.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pc.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://dy.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://he.asd995.cn

[U85] JS：可选链
来源：http://qa.yuntaijiaju.cn

a?.b?.c
来源：http://ly.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://cv.jctech888.com.cn

a ?? b
来源：http://gz.chemitech.net.cn

[U87] JS：解构默认值
来源：http://vl.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://jg.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://fg.shxzskj.cn

{ ...a, ...b }
来源：http://hu.jctech888.com.cn

[U89] JS：数组去重
来源：http://xs.shxzskj.cn

[...new Set(arr)]
来源：http://tj.nicolike.cn

[U90] JS：数字数组排序
来源：http://mf.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://yo.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://oe.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jl.nicolike.cn

[U92] JS：深拷贝
来源：http://zn.szxytkj.cn

structuredClone(obj)
来源：http://ha.newstarts.cn

[U93] JS：模板字符串
来源：http://lz.bookmarksfly.cn

`共 ${n} 条`
来源：http://vj.colortex.cn

[U94] JS：箭头函数
来源：http://jd.shxzukj.cn

const double = x => x * 2;
来源：http://gs.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://na.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://zy.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://zb.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xy.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://fl.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jm.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://cq.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xn.shxzskj.cn

[U99] JS：事件监听
来源：http://ym.nszjky.cn

el.addEventListener("click", e => {})
来源：http://if.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://lx.jctech888.com.cn

document.querySelector(".item")
来源：http://wp.asd995.cn

[U101] JS：classList 操作
来源：http://kk.colortex.cn

el.classList.toggle("active")
来源：http://ha.wgjwhj.cn

[U102] JS：本地存储
来源：http://kg.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uj.szsharing.cn

[U103] JS：定时器
来源：http://dd.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ks.szxytkj.cn

[U104] JS：防抖
来源：http://qr.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.huixiangedu.cn

[U105] JS：节流
来源：http://ch.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xc.szxytkj.cn

[U106] JS：日期格式化
来源：http://ru.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ag.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://tv.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ny.huixiangedu.cn

[U108] JS：随机整数
来源：http://np.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://og.shxzskj.cn

[U109] JS：数组分组
来源：http://nv.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://qe.bookmarksfly.cn

[U110] JS：数组分块
来源：http://zk.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xc.hahajie.cn

[U111] JS：对象转 Map
来源：http://ja.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://xt.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://cb.nicolike.cn

"7".padStart(3, "0")
来源：http://kt.lnxyls.cn

[U113] JS：正则替换全部
来源：http://lb.panjiajie.cn

s.replaceAll("a", "b")
来源：http://wt.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://ur.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://od.9csxet.cn

[U115] JS：生成 UUID
来源：http://go.szxytkj.cn

crypto.randomUUID()
来源：http://kp.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://on.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://ck.gzmigu.cn

[U117] JS：单元测试
来源：http://ex.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://je.shxzskj.cn

[U118] JS：开发服务器
来源：http://qz.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://ch.shtwfgs.cn

[U119] JS：生产构建
来源：http://nc.yuexingan06.cn

npx vite build
来源：http://va.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://xy.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://bc.521024.cn

================================================================================
来源：http://xc.haigaiapp.cn

统计汇总
来源：http://qx.newstarts.cn

================================================================================
来源：http://nx.hnjuh.cn

按语言统计（条）：
来源：http://ad.nszjky.cn

Python ......... 252
来源：http://fl.asd995.cn

PHP ............ 252
来源：http://gu.muxihuayi.cn

JavaScript ..... 252
来源：http://tn.szsharing.cn

TypeScript ..... 212
来源：http://za.jianghongdianzi.cn

Java ........... 212
来源：http://vb.nszjky.cn

Go ............. 212
来源：http://dn.muxihuayi.cn

Ruby ........... 212
来源：http://fj.asd995.cn

C# ............. 212
来源：http://qp.szsharing.cn

C .............. 30
来源：http://qt.shxzukj.cn

C++ ............ 30
来源：http://ny.9csxet.cn

SQL ............ 90
来源：http://fu.asd995.cn

Bash ........... 80
来源：http://nv.shtwfgs.cn

Kotlin ......... 15
来源：http://ex.huixinmuqiang.cn

Swift .......... 15
来源：http://ki.nicolike.cn

Lua ............ 10
来源：http://it.nszjky.cn

Perl ........... 10
来源：http://xa.shtwfgs.cn

Scala .......... 10
来源：http://cc.szsharing.cn

------------------------------------
来源：http://mv.nicolike.cn

合计 ........... 2106 条
来源：http://sd.yuexingan06.cn

按章节统计：
来源：http://vk.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sl.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oc.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qd.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pq.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yc.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cq.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oi.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bq.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pq.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xf.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ed.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nr.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gl.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wc.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://un.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sa.bjjhwx.cn

Q SQL 专题                              90
来源：http://wi.521024.cn

R Bash 专题                             80
来源：http://tf.hahajie.cn

S C / C++ 专题                          60
来源：http://tt.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://ed.haigaiapp.cn

U 高频实用片段                         120
来源：http://xt.hahajie.cn

------------------------------------
来源：http://yl.9csxet.cn

合计                                  2106 条
来源：http://kz.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://vu.huixiangedu.cn

使用提醒
来源：http://fi.521024.cn

--------------------------------------------------------------------------------
来源：http://sv.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jh.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yl.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bi.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xs.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ys.9csxet.cn

—— 文件结束 ——
来源：http://qf.nicolike.cn

================================================================================
来源：http://mz.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://te.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://lt.jctech888.com.cn

================================================================================
来源：http://hw.nszjky.cn

【收录内容】
来源：http://xo.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qk.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yf.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://on.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gl.huixinmuqiang.cn

【使用说明】
来源：http://lv.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ha.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://io.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fo.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gb.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://co.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nw.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ye.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tx.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lc.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qq.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hi.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yj.yuntaijiaju.cn

【文件统计】
来源：http://od.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tt.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://gm.huanxung.cn

目  录
来源：http://gn.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ix.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hd.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wb.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sp.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://py.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sm.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://za.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rh.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vo.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wr.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rl.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://go.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jo.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kd.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pr.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hg.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://et.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://so.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ff.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fz.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yq.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pz.muxihuayi.cn

================================================================================
来源：http://lx.nicolike.cn

A. 基础语法与类型
来源：http://hk.chemitech.net.cn

================================================================================
来源：http://zd.hahajie.cn

[A01] Hello World
来源：http://iz.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ni.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://np.521024.cn

JS:   console.log("Hello, World!");
来源：http://rc.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zv.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://dx.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://bq.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://te.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://df.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://er.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iw.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rs.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ph.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cw.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://pu.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://mj.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://vt.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kh.shxzskj.cn

[A03] 常量定义
来源：http://en.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ga.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://ti.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://gy.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://wr.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://jb.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://wz.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://ew.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://ln.bjjhwx.cn

[A04] 判断变量类型
来源：http://ht.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://af.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://co.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xa.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://eq.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://li.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jw.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ui.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://fk.szsharing.cn

[A05] 整数除法与取模
来源：http://is.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tx.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jk.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pk.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vq.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://db.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://zy.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://af.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://dn.szxytkj.cn

[A06] 字符串转数字
来源：http://nc.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://hb.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fq.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lw.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fq.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hb.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iy.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://le.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fx.hnjuh.cn

[A07] 数字转字符串
来源：http://mn.haigaiapp.cn

Py:   str(42)
来源：http://zw.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://zj.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://gv.huanxung.cn

TS:   String(42)
来源：http://as.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gd.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://sc.nszjky.cn

Ruby: 42.to_s
来源：http://zr.hahajie.cn

C#:   42.ToString()
来源：http://hh.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://sx.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sd.shtwfgs.cn


<!-- 参考信息 -->