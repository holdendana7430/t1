代发 wailian999

[U57] PHP：字符串插值
来源：http://vy.yuntaijiaju.cn

"值: {$a}"
来源：http://fy.shxzskj.cn

[U58] PHP：数组三件套
来源：http://xv.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gv.huanxung.cn

[U59] PHP：自定义排序
来源：http://bn.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://da.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://vi.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kw.haigaiapp.cn

[U61] PHP：正则
来源：http://tg.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ke.panjiajie.cn

[U62] PHP：日期对象
来源：http://zq.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hb.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://jv.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ch.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://wi.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://ck.wgjwhj.cn

[U65] PHP：会话
来源：http://zn.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pl.colortex.cn

[U66] PHP：设置 Cookie
来源：http://co.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nj.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://bh.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wu.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://vr.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uj.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://qs.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cn.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://xd.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jq.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://bg.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://zy.nszjky.cn

[U72] PHP：写错误日志
来源：http://lw.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://tu.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://ft.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://yi.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://sb.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://yq.asd995.cn

[U75] PHP：依赖注入
来源：http://oa.muxihuayi.cn

composer require psr/container
来源：http://ep.shtwfgs.cn

[U76] PHP：简单路由
来源：http://rl.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kn.shxzukj.cn

[U77] PHP：模板渲染
来源：http://qy.newstarts.cn

composer require twig/twig
来源：http://bx.panjiajie.cn

[U78] PHP：单元测试
来源：http://bm.asd995.cn

composer require --dev phpunit/phpunit
来源：http://lj.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://dn.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://bn.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://id.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lu.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://xw.hnjuh.cn

npm init -y;  npm i express
来源：http://ul.9csxet.cn

[U82] JS：package.json 脚本
来源：http://ej.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://px.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ix.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kf.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://ye.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bj.bookmarksfly.cn

[U85] JS：可选链
来源：http://mw.haigaiapp.cn

a?.b?.c
来源：http://pl.szxytkj.cn

[U86] JS：空值合并
来源：http://go.nicolike.cn

a ?? b
来源：http://rx.bjjhwx.cn

[U87] JS：解构默认值
来源：http://wz.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://nb.9csxet.cn

[U88] JS：对象展开合并
来源：http://qj.jctech888.com.cn

{ ...a, ...b }
来源：http://hi.shxzukj.cn

[U89] JS：数组去重
来源：http://ll.panjiajie.cn

[...new Set(arr)]
来源：http://zz.huanxung.cn

[U90] JS：数字数组排序
来源：http://vu.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://ub.521024.cn

[U91] JS：对象键值遍历
来源：http://se.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uj.lnxyls.cn

[U92] JS：深拷贝
来源：http://vc.haigaiapp.cn

structuredClone(obj)
来源：http://yh.muxihuayi.cn

[U93] JS：模板字符串
来源：http://ft.9csxet.cn

`共 ${n} 条`
来源：http://tj.colortex.cn

[U94] JS：箭头函数
来源：http://mu.bookmarksfly.cn

const double = x => x * 2;
来源：http://xc.szsharing.cn

[U95] JS：Promise 包装
来源：http://vv.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://lp.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ku.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mq.asd995.cn

[U97] JS：并发请求
来源：http://ni.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qx.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://oc.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rh.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://ag.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://is.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://ek.521024.cn

document.querySelector(".item")
来源：http://wg.muxihuayi.cn

[U101] JS：classList 操作
来源：http://id.bookmarksfly.cn

el.classList.toggle("active")
来源：http://kh.gzmigu.cn

[U102] JS：本地存储
来源：http://iy.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ko.jianghongdianzi.cn

[U103] JS：定时器
来源：http://gx.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fh.jianghongdianzi.cn

[U104] JS：防抖
来源：http://cn.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qf.hnjuh.cn

[U105] JS：节流
来源：http://uo.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fu.asd995.cn

[U106] JS：日期格式化
来源：http://cj.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xp.521024.cn

[U107] JS：数字千分位
来源：http://rd.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://px.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://sm.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ik.asd995.cn

[U109] JS：数组分组
来源：http://ql.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://lv.521024.cn

[U110] JS：数组分块
来源：http://iz.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://an.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://pj.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://rw.nicolike.cn

[U112] JS：字符串补位
来源：http://kh.yuexingan06.cn

"7".padStart(3, "0")
来源：http://ff.gzmigu.cn

[U113] JS：正则替换全部
来源：http://ds.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://kz.9csxet.cn

[U114] JS：JSON 深比较
来源：http://qn.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vv.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://pc.haigaiapp.cn

crypto.randomUUID()
来源：http://fk.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://wv.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://zt.gzmigu.cn

[U117] JS：单元测试
来源：http://ur.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://rn.nicolike.cn

[U118] JS：开发服务器
来源：http://fm.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://jg.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://yk.wgjwhj.cn

npx vite build
来源：http://iv.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://ye.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://fd.nicolike.cn

================================================================================
来源：http://ip.muxihuayi.cn

统计汇总
来源：http://eb.bookmarksfly.cn

================================================================================
来源：http://nz.bjjhwx.cn

按语言统计（条）：
来源：http://ql.huixiangedu.cn

Python ......... 252
来源：http://zq.huanxung.cn

PHP ............ 252
来源：http://fb.shtwfgs.cn

JavaScript ..... 252
来源：http://xd.muxihuayi.cn

TypeScript ..... 212
来源：http://hl.shxzukj.cn

Java ........... 212
来源：http://vb.newstarts.cn

Go ............. 212
来源：http://gd.szxytkj.cn

Ruby ........... 212
来源：http://zq.chemitech.net.cn

C# ............. 212
来源：http://tu.huixiangedu.cn

C .............. 30
来源：http://ma.gzmigu.cn

C++ ............ 30
来源：http://xy.shtwfgs.cn

SQL ............ 90
来源：http://up.chemitech.net.cn

Bash ........... 80
来源：http://ao.521024.cn

Kotlin ......... 15
来源：http://hb.9csxet.cn

Swift .......... 15
来源：http://qo.shxzukj.cn

Lua ............ 10
来源：http://be.yuexingan06.cn

Perl ........... 10
来源：http://uc.yuntaijiaju.cn

Scala .......... 10
来源：http://yl.bjjhwx.cn

------------------------------------
来源：http://xv.nicolike.cn

合计 ........... 2106 条
来源：http://nk.huixinmuqiang.cn

按章节统计：
来源：http://ke.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://go.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sj.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wd.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uu.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kp.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://do.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vu.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mm.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://na.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xw.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yv.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gb.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zk.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zt.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dz.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sa.lnxyls.cn

Q SQL 专题                              90
来源：http://cs.panjiajie.cn

R Bash 专题                             80
来源：http://id.newstarts.cn

S C / C++ 专题                          60
来源：http://nc.jctech888.com.cn

T 其他语言补充                          60
来源：http://ty.shxzskj.cn

U 高频实用片段                         120
来源：http://qw.chemitech.net.cn

------------------------------------
来源：http://tr.bookmarksfly.cn

合计                                  2106 条
来源：http://ny.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://vr.asd995.cn

使用提醒
来源：http://aj.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ph.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dc.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ry.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jy.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fg.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dw.nicolike.cn

—— 文件结束 ——
来源：http://qm.muxihuayi.cn

================================================================================
来源：http://uh.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://xo.asd995.cn

Common Programming Examples Cheat Book
来源：http://vu.shxzukj.cn

================================================================================
来源：http://xn.9csxet.cn

【收录内容】
来源：http://eg.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dv.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sq.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://zw.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jl.szsharing.cn

【使用说明】
来源：http://qh.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ik.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ht.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uj.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://td.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://if.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nr.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ug.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vn.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bl.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ij.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vw.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://we.shxzskj.cn

【文件统计】
来源：http://sq.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yh.asd995.cn

--------------------------------------------------------------------------------
来源：http://ti.lnxyls.cn

目  录
来源：http://st.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ef.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vv.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zi.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mi.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lt.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bs.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mr.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bb.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qa.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ab.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://do.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://my.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kr.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vw.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gg.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nf.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uk.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mu.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tm.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cu.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://te.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pg.shxzskj.cn

================================================================================
来源：http://fl.gzmigu.cn

A. 基础语法与类型
来源：http://ue.panjiajie.cn

================================================================================
来源：http://fz.hnjuh.cn

[A01] Hello World
来源：http://ro.shxzukj.cn

Py:   print("Hello, World!")
来源：http://md.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://mv.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://ak.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gn.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://iz.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://hb.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://el.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xw.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://ua.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fh.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hp.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gq.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fq.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://fk.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://qp.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://lw.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gu.shtwfgs.cn

[A03] 常量定义
来源：http://wz.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://to.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://mb.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://ux.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://bz.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://lp.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://hk.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://nj.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://bg.panjiajie.cn

[A04] 判断变量类型
来源：http://va.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hn.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hx.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yz.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://lx.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ps.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ne.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uv.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://kl.lnxyls.cn

[A05] 整数除法与取模
来源：http://xg.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kl.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nc.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vk.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ze.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://kb.521024.cn

Go:   7 / 2; 7 % 2
来源：http://fu.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://sc.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://mf.asd995.cn

[A06] 字符串转数字
来源：http://pr.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://lv.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bg.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nf.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fs.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://an.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jn.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://as.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ia.shtwfgs.cn

[A07] 数字转字符串
来源：http://gg.newstarts.cn

Py:   str(42)
来源：http://ir.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://fg.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://pi.shtwfgs.cn

TS:   String(42)
来源：http://ou.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ew.colortex.cn

Go:   strconv.Itoa(42)
来源：http://ap.nszjky.cn

Ruby: 42.to_s
来源：http://du.521024.cn

C#:   42.ToString()
来源：http://dn.asd995.cn

[A08] 取整与四舍五入
来源：http://ws.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eh.haigaiapp.cn


<!-- 参考信息 -->