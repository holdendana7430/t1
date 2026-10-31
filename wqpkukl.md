代发 wailian999

[U47] PHP：联合类型
来源：http://tj.hnjuh.cn

int|string $id
来源：http://av.szsharing.cn

[U48] PHP：纯枚举
来源：http://zd.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dy.521024.cn

[U49] PHP：只读属性
来源：http://pl.shtwfgs.cn

public readonly string $name
来源：http://or.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://kg.shxzskj.cn

public function __construct(private int $id) {}
来源：http://vw.yuexingan06.cn

[U51] PHP：数组解构
来源：http://py.panjiajie.cn

[$a, $b] = $arr;
来源：http://hw.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://hp.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://zo.hahajie.cn

[U53] PHP：空合并运算符
来源：http://qd.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://ks.asd995.cn

[U54] PHP：空安全调用
来源：http://bp.shtwfgs.cn

$obj?->method()
来源：http://zh.colortex.cn

[U55] PHP：match 表达式
来源：http://fq.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rd.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://ii.shxzskj.cn

f(a: 1, b: 2)
来源：http://fq.lnxyls.cn

[U57] PHP：字符串插值
来源：http://mz.muxihuayi.cn

"值: {$a}"
来源：http://pb.newstarts.cn

[U58] PHP：数组三件套
来源：http://yp.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yq.hnjuh.cn

[U59] PHP：自定义排序
来源：http://ws.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ui.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://xv.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sa.nszjky.cn

[U61] PHP：正则
来源：http://sl.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fy.haigaiapp.cn

[U62] PHP：日期对象
来源：http://ib.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pr.nicolike.cn

[U63] PHP：文件读写
来源：http://nz.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ni.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://kl.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ws.nszjky.cn

[U65] PHP：会话
来源：http://nm.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kn.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://ze.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fp.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://qm.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nx.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://mj.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ow.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://lf.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ik.nicolike.cn

[U70] PHP：PDO 事务
来源：http://sn.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tf.nicolike.cn

[U71] PHP：抛出异常
来源：http://dm.521024.cn

throw new RuntimeException("失败", 500);
来源：http://ma.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://my.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://il.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://dv.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://iq.szsharing.cn

[U74] PHP：读取环境变量
来源：http://fq.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://fo.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://ga.yuexingan06.cn

composer require psr/container
来源：http://bq.521024.cn

[U76] PHP：简单路由
来源：http://ms.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gz.szsharing.cn

[U77] PHP：模板渲染
来源：http://xv.bjjhwx.cn

composer require twig/twig
来源：http://pp.bjjhwx.cn

[U78] PHP：单元测试
来源：http://qf.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://pt.shxzskj.cn

[U79] PHP：静态分析
来源：http://uv.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://mk.asd995.cn

[U80] PHP：代码规范修复
来源：http://mr.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pe.muxihuayi.cn

[U81] JS：初始化项目
来源：http://pq.hahajie.cn

npm init -y;  npm i express
来源：http://ne.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://rz.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kt.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://tf.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vl.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://di.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://be.muxihuayi.cn

[U85] JS：可选链
来源：http://zf.asd995.cn

a?.b?.c
来源：http://kl.panjiajie.cn

[U86] JS：空值合并
来源：http://pb.nicolike.cn

a ?? b
来源：http://qq.bjjhwx.cn

[U87] JS：解构默认值
来源：http://qj.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://xw.lnxyls.cn

[U88] JS：对象展开合并
来源：http://jo.shxzskj.cn

{ ...a, ...b }
来源：http://xv.jctech888.com.cn

[U89] JS：数组去重
来源：http://fy.bookmarksfly.cn

[...new Set(arr)]
来源：http://cx.lnxyls.cn

[U90] JS：数字数组排序
来源：http://gv.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://tw.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://ez.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vt.shxzukj.cn

[U92] JS：深拷贝
来源：http://ue.nicolike.cn

structuredClone(obj)
来源：http://jj.nicolike.cn

[U93] JS：模板字符串
来源：http://hg.hahajie.cn

`共 ${n} 条`
来源：http://aa.lnxyls.cn

[U94] JS：箭头函数
来源：http://gc.yuntaijiaju.cn

const double = x => x * 2;
来源：http://fe.hnjuh.cn

[U95] JS：Promise 包装
来源：http://vr.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://uh.hahajie.cn

[U96] JS：async/await 与异常
来源：http://hs.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ki.nicolike.cn

[U97] JS：并发请求
来源：http://mw.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mj.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://jz.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wz.colortex.cn

[U99] JS：事件监听
来源：http://qw.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://ei.szsharing.cn

[U100] JS：DOM 查询
来源：http://id.szsharing.cn

document.querySelector(".item")
来源：http://wu.szxytkj.cn

[U101] JS：classList 操作
来源：http://mu.hahajie.cn

el.classList.toggle("active")
来源：http://hs.yuexingan06.cn

[U102] JS：本地存储
来源：http://hi.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dp.shtwfgs.cn

[U103] JS：定时器
来源：http://vg.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ac.yuntaijiaju.cn

[U104] JS：防抖
来源：http://uy.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vq.huixiangedu.cn

[U105] JS：节流
来源：http://nv.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zy.shxzukj.cn

[U106] JS：日期格式化
来源：http://jb.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zv.newstarts.cn

[U107] JS：数字千分位
来源：http://ck.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ta.muxihuayi.cn

[U108] JS：随机整数
来源：http://zn.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fh.newstarts.cn

[U109] JS：数组分组
来源：http://vj.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ct.yuexingan06.cn

[U110] JS：数组分块
来源：http://qn.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ip.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://cd.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://gc.chemitech.net.cn

[U112] JS：字符串补位
来源：http://zz.muxihuayi.cn

"7".padStart(3, "0")
来源：http://pj.shxzskj.cn

[U113] JS：正则替换全部
来源：http://vz.colortex.cn

s.replaceAll("a", "b")
来源：http://zv.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://ob.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hh.shxzskj.cn

[U115] JS：生成 UUID
来源：http://xp.colortex.cn

crypto.randomUUID()
来源：http://oi.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://po.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://ab.bookmarksfly.cn

[U117] JS：单元测试
来源：http://vn.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://cy.hahajie.cn

[U118] JS：开发服务器
来源：http://mw.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://vs.lnxyls.cn

[U119] JS：生产构建
来源：http://qx.lnxyls.cn

npx vite build
来源：http://we.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://tg.colortex.cn

import.meta.env.VITE_API_URL
来源：http://la.jctech888.com.cn

================================================================================
来源：http://te.huanxung.cn

统计汇总
来源：http://fv.bjjhwx.cn

================================================================================
来源：http://bu.wgjwhj.cn

按语言统计（条）：
来源：http://tj.jianghongdianzi.cn

Python ......... 252
来源：http://vy.szxytkj.cn

PHP ............ 252
来源：http://at.nicolike.cn

JavaScript ..... 252
来源：http://eq.szxytkj.cn

TypeScript ..... 212
来源：http://nj.hnjuh.cn

Java ........... 212
来源：http://ab.haigaiapp.cn

Go ............. 212
来源：http://ku.huixiangedu.cn

Ruby ........... 212
来源：http://yn.bookmarksfly.cn

C# ............. 212
来源：http://uz.haigaiapp.cn

C .............. 30
来源：http://fq.szxytkj.cn

C++ ............ 30
来源：http://wm.yuntaijiaju.cn

SQL ............ 90
来源：http://ye.szsharing.cn

Bash ........... 80
来源：http://yg.gzmigu.cn

Kotlin ......... 15
来源：http://xp.haigaiapp.cn

Swift .......... 15
来源：http://mu.haigaiapp.cn

Lua ............ 10
来源：http://di.shtwfgs.cn

Perl ........... 10
来源：http://cn.hnjuh.cn

Scala .......... 10
来源：http://cz.szsharing.cn

------------------------------------
来源：http://xg.9csxet.cn

合计 ........... 2106 条
来源：http://kv.521024.cn

按章节统计：
来源：http://dd.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ik.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://at.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ca.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tk.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fq.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sn.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lo.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://an.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://po.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qb.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rr.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ky.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dq.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ux.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uh.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vr.wgjwhj.cn

Q SQL 专题                              90
来源：http://he.521024.cn

R Bash 专题                             80
来源：http://rl.panjiajie.cn

S C / C++ 专题                          60
来源：http://xr.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://sm.nszjky.cn

U 高频实用片段                         120
来源：http://ka.shtwfgs.cn

------------------------------------
来源：http://ba.yuntaijiaju.cn

合计                                  2106 条
来源：http://hb.nicolike.cn

--------------------------------------------------------------------------------
来源：http://og.yuexingan06.cn

使用提醒
来源：http://vi.nszjky.cn

--------------------------------------------------------------------------------
来源：http://sr.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lf.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hx.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pq.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yb.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wh.9csxet.cn

—— 文件结束 ——
来源：http://to.bookmarksfly.cn

================================================================================
来源：http://tp.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://au.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://eu.hahajie.cn

================================================================================
来源：http://gf.bookmarksfly.cn

【收录内容】
来源：http://jm.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://po.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bg.jctech888.com.cn

SQL · Bash · C · C++
来源：http://xc.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rm.colortex.cn

【使用说明】
来源：http://cd.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vp.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pe.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pl.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ha.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rc.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://me.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://el.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lg.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uq.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jy.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qa.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zv.nicolike.cn

【文件统计】
来源：http://ez.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sl.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ei.bookmarksfly.cn

目  录
来源：http://dn.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ql.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ag.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wn.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ei.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nq.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nb.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iq.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://if.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yw.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qf.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fc.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zb.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sc.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wq.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rh.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pb.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://py.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ci.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eo.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://si.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zu.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iq.huixinmuqiang.cn

================================================================================
来源：http://yd.szxytkj.cn

A. 基础语法与类型
来源：http://iw.hahajie.cn

================================================================================
来源：http://ic.nszjky.cn

[A01] Hello World
来源：http://aq.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ru.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://vp.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://yj.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wa.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://fh.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://nt.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://dd.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yf.panjiajie.cn

[A02] 变量声明与赋值
来源：http://fj.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mt.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iy.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vx.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tg.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://ba.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://bu.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://lo.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kg.bookmarksfly.cn

[A03] 常量定义
来源：http://ja.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://mg.huanxung.cn

JS:   const PI = 3.14159;
来源：http://go.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://te.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://vn.hnjuh.cn

Go:   const PI = 3.14159
来源：http://gy.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://yk.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://nm.huixiangedu.cn

[A04] 判断变量类型
来源：http://gl.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yb.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zj.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jl.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://jq.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pi.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jd.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ux.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://ez.haigaiapp.cn

[A05] 整数除法与取模
来源：http://qw.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xd.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qk.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://za.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tt.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://en.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://vi.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://pd.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://ao.panjiajie.cn


<!-- 参考信息 -->