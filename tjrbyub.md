代发 wailian999

[U47] PHP：联合类型
来源：http://yg.szsharing.cn

int|string $id
来源：http://qd.colortex.cn

[U48] PHP：纯枚举
来源：http://mp.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hy.shtwfgs.cn

[U49] PHP：只读属性
来源：http://lw.muxihuayi.cn

public readonly string $name
来源：http://ya.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://is.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://dl.muxihuayi.cn

[U51] PHP：数组解构
来源：http://mr.bjjhwx.cn

[$a, $b] = $arr;
来源：http://cq.gzmigu.cn

[U52] PHP：箭头函数
来源：http://ba.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://uw.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://wy.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://nj.hahajie.cn

[U54] PHP：空安全调用
来源：http://ac.panjiajie.cn

$obj?->method()
来源：http://dg.szxytkj.cn

[U55] PHP：match 表达式
来源：http://od.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://su.shxzukj.cn

[U56] PHP：命名参数
来源：http://hl.shtwfgs.cn

f(a: 1, b: 2)
来源：http://gz.huanxung.cn

[U57] PHP：字符串插值
来源：http://zt.lnxyls.cn

"值: {$a}"
来源：http://zj.asd995.cn

[U58] PHP：数组三件套
来源：http://ao.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ql.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://ys.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rj.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://ja.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dk.bookmarksfly.cn

[U61] PHP：正则
来源：http://bl.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wl.chemitech.net.cn

[U62] PHP：日期对象
来源：http://md.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hi.yuexingan06.cn

[U63] PHP：文件读写
来源：http://ph.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yu.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://ef.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://he.chemitech.net.cn

[U65] PHP：会话
来源：http://bx.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sd.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://az.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jo.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://up.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kb.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://vu.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wi.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://ut.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ya.9csxet.cn

[U70] PHP：PDO 事务
来源：http://mi.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ws.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://qn.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://qc.szsharing.cn

[U72] PHP：写错误日志
来源：http://yh.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://uj.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://wi.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://ff.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://xj.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://ml.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://dv.shxzskj.cn

composer require psr/container
来源：http://bh.hahajie.cn

[U76] PHP：简单路由
来源：http://gz.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ax.szsharing.cn

[U77] PHP：模板渲染
来源：http://ce.newstarts.cn

composer require twig/twig
来源：http://ff.haigaiapp.cn

[U78] PHP：单元测试
来源：http://aa.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://vg.huixiangedu.cn

[U79] PHP：静态分析
来源：http://rs.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://np.newstarts.cn

[U80] PHP：代码规范修复
来源：http://bp.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ac.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://cv.lnxyls.cn

npm init -y;  npm i express
来源：http://mp.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://iu.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uo.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://fa.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kg.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://ah.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yl.szxytkj.cn

[U85] JS：可选链
来源：http://sp.haigaiapp.cn

a?.b?.c
来源：http://cy.hahajie.cn

[U86] JS：空值合并
来源：http://vx.shxzukj.cn

a ?? b
来源：http://xe.hahajie.cn

[U87] JS：解构默认值
来源：http://hi.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://fv.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://nq.muxihuayi.cn

{ ...a, ...b }
来源：http://fb.jctech888.com.cn

[U89] JS：数组去重
来源：http://km.huixiangedu.cn

[...new Set(arr)]
来源：http://vc.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://wn.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://pg.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://vo.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fi.shtwfgs.cn

[U92] JS：深拷贝
来源：http://cv.lnxyls.cn

structuredClone(obj)
来源：http://ek.huanxung.cn

[U93] JS：模板字符串
来源：http://gc.szsharing.cn

`共 ${n} 条`
来源：http://ug.panjiajie.cn

[U94] JS：箭头函数
来源：http://tl.yuexingan06.cn

const double = x => x * 2;
来源：http://di.szsharing.cn

[U95] JS：Promise 包装
来源：http://bi.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://hi.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://cu.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eh.chemitech.net.cn

[U97] JS：并发请求
来源：http://sl.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oz.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://dx.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ec.asd995.cn

[U99] JS：事件监听
来源：http://lc.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://op.9csxet.cn

[U100] JS：DOM 查询
来源：http://sa.huixiangedu.cn

document.querySelector(".item")
来源：http://bo.hnjuh.cn

[U101] JS：classList 操作
来源：http://xl.jctech888.com.cn

el.classList.toggle("active")
来源：http://qi.bjjhwx.cn

[U102] JS：本地存储
来源：http://ht.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://um.wgjwhj.cn

[U103] JS：定时器
来源：http://gm.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bb.shxzskj.cn

[U104] JS：防抖
来源：http://zv.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mt.521024.cn

[U105] JS：节流
来源：http://wx.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://um.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://dz.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yt.chemitech.net.cn

[U107] JS：数字千分位
来源：http://bw.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rd.newstarts.cn

[U108] JS：随机整数
来源：http://ts.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jc.chemitech.net.cn

[U109] JS：数组分组
来源：http://ht.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://id.asd995.cn

[U110] JS：数组分块
来源：http://us.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ri.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://ek.nicolike.cn

new Map(Object.entries(obj))
来源：http://sq.gzmigu.cn

[U112] JS：字符串补位
来源：http://dn.nszjky.cn

"7".padStart(3, "0")
来源：http://rc.9csxet.cn

[U113] JS：正则替换全部
来源：http://al.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://eb.nicolike.cn

[U114] JS：JSON 深比较
来源：http://qk.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eo.521024.cn

[U115] JS：生成 UUID
来源：http://af.panjiajie.cn

crypto.randomUUID()
来源：http://ga.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://tu.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://vb.panjiajie.cn

[U117] JS：单元测试
来源：http://rf.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://bs.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://at.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://od.panjiajie.cn

[U119] JS：生产构建
来源：http://gq.szxytkj.cn

npx vite build
来源：http://xb.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://yw.colortex.cn

import.meta.env.VITE_API_URL
来源：http://ys.muxihuayi.cn

================================================================================
来源：http://ph.hahajie.cn

统计汇总
来源：http://er.lnxyls.cn

================================================================================
来源：http://dy.jianghongdianzi.cn

按语言统计（条）：
来源：http://lu.jctech888.com.cn

Python ......... 252
来源：http://hx.asd995.cn

PHP ............ 252
来源：http://cc.huixiangedu.cn

JavaScript ..... 252
来源：http://oq.szsharing.cn

TypeScript ..... 212
来源：http://gx.521024.cn

Java ........... 212
来源：http://wm.9csxet.cn

Go ............. 212
来源：http://rg.hahajie.cn

Ruby ........... 212
来源：http://at.newstarts.cn

C# ............. 212
来源：http://lq.asd995.cn

C .............. 30
来源：http://iv.nszjky.cn

C++ ............ 30
来源：http://mz.huixinmuqiang.cn

SQL ............ 90
来源：http://fl.shxzukj.cn

Bash ........... 80
来源：http://ll.yuntaijiaju.cn

Kotlin ......... 15
来源：http://sl.szsharing.cn

Swift .......... 15
来源：http://zc.huanxung.cn

Lua ............ 10
来源：http://mx.nicolike.cn

Perl ........... 10
来源：http://xi.hahajie.cn

Scala .......... 10
来源：http://qv.bookmarksfly.cn

------------------------------------
来源：http://mo.bookmarksfly.cn

合计 ........... 2106 条
来源：http://fq.yuexingan06.cn

按章节统计：
来源：http://pk.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qe.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ix.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://op.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dd.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cy.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ws.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xi.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vp.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fd.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bb.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ke.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sr.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wg.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bt.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://er.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bd.gzmigu.cn

Q SQL 专题                              90
来源：http://gr.szsharing.cn

R Bash 专题                             80
来源：http://uf.hnjuh.cn

S C / C++ 专题                          60
来源：http://qs.haigaiapp.cn

T 其他语言补充                          60
来源：http://mg.wgjwhj.cn

U 高频实用片段                         120
来源：http://bs.colortex.cn

------------------------------------
来源：http://av.szsharing.cn

合计                                  2106 条
来源：http://pa.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://fz.szxytkj.cn

使用提醒
来源：http://kz.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ht.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ju.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ro.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lh.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ok.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nj.gzmigu.cn

—— 文件结束 ——
来源：http://ue.wgjwhj.cn

================================================================================
来源：http://qk.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://nz.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://ci.asd995.cn

================================================================================
来源：http://gs.huanxung.cn

【收录内容】
来源：http://tt.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://br.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xb.colortex.cn

SQL · Bash · C · C++
来源：http://hq.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uu.haigaiapp.cn

【使用说明】
来源：http://fn.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xx.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vv.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oz.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qj.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qm.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lp.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rk.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vn.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tv.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wi.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qe.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ue.jctech888.com.cn

【文件统计】
来源：http://qz.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hb.9csxet.cn

--------------------------------------------------------------------------------
来源：http://lq.hahajie.cn

目  录
来源：http://pd.521024.cn

--------------------------------------------------------------------------------
来源：http://wr.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hu.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vz.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qb.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://il.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ig.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sn.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ys.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xy.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lr.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ck.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yh.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://za.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ix.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tb.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ah.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ao.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yp.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tu.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://om.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kh.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ke.bjjhwx.cn

================================================================================
来源：http://mj.asd995.cn

A. 基础语法与类型
来源：http://gn.huixiangedu.cn

================================================================================
来源：http://vs.huixiangedu.cn

[A01] Hello World
来源：http://wy.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ii.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://ck.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://dp.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zv.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://ep.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://iu.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://dp.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kp.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://mn.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ri.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tr.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zx.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wg.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://sy.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ge.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://yt.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gk.wgjwhj.cn

[A03] 常量定义
来源：http://ru.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zm.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://oi.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://fb.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://zm.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://js.huanxung.cn

Go:   const PI = 3.14159
来源：http://yn.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://lo.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://rj.colortex.cn

[A04] 判断变量类型
来源：http://bp.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hw.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hs.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kb.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://ge.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cn.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ko.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vn.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://je.nicolike.cn

[A05] 整数除法与取模
来源：http://nx.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lq.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xp.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ub.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rb.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://zr.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://pt.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://ex.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://ml.chemitech.net.cn


<!-- 参考信息 -->