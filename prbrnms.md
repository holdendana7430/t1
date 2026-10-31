代发 wailian999

[U49] PHP：只读属性
来源：http://sa.huanxung.cn

public readonly string $name
来源：http://oz.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ik.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ml.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ns.chemitech.net.cn

[$a, $b] = $arr;
来源：http://ll.nicolike.cn

[U52] PHP：箭头函数
来源：http://lg.asd995.cn

$double = fn($x) => $x * 2;
来源：http://ky.colortex.cn

[U53] PHP：空合并运算符
来源：http://ce.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://xg.nicolike.cn

[U54] PHP：空安全调用
来源：http://cv.hahajie.cn

$obj?->method()
来源：http://ro.szsharing.cn

[U55] PHP：match 表达式
来源：http://uw.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iz.bjjhwx.cn

[U56] PHP：命名参数
来源：http://ax.wgjwhj.cn

f(a: 1, b: 2)
来源：http://ur.panjiajie.cn

[U57] PHP：字符串插值
来源：http://mv.shtwfgs.cn

"值: {$a}"
来源：http://wq.hnjuh.cn

[U58] PHP：数组三件套
来源：http://jc.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nq.lnxyls.cn

[U59] PHP：自定义排序
来源：http://im.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gn.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://kt.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ra.chemitech.net.cn

[U61] PHP：正则
来源：http://uy.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pn.panjiajie.cn

[U62] PHP：日期对象
来源：http://gp.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ch.szxytkj.cn

[U63] PHP：文件读写
来源：http://vu.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mw.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://sa.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://sf.shxzukj.cn

[U65] PHP：会话
来源：http://xb.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yc.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://bn.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nk.newstarts.cn

[U67] PHP：处理文件上传
来源：http://xh.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tc.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://pt.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gw.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://io.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://me.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://um.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cy.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://pf.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://cz.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://no.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://za.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://fj.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://bm.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://lh.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://bm.asd995.cn

[U75] PHP：依赖注入
来源：http://pb.muxihuayi.cn

composer require psr/container
来源：http://ki.9csxet.cn

[U76] PHP：简单路由
来源：http://li.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uy.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://um.asd995.cn

composer require twig/twig
来源：http://hx.shtwfgs.cn

[U78] PHP：单元测试
来源：http://vi.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://gl.huixiangedu.cn

[U79] PHP：静态分析
来源：http://cm.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://mb.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://jg.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xv.muxihuayi.cn

[U81] JS：初始化项目
来源：http://bl.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://ae.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://ea.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ba.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://sz.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tu.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://gk.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://va.shtwfgs.cn

[U85] JS：可选链
来源：http://uy.nszjky.cn

a?.b?.c
来源：http://ae.nicolike.cn

[U86] JS：空值合并
来源：http://cj.wgjwhj.cn

a ?? b
来源：http://kw.jctech888.com.cn

[U87] JS：解构默认值
来源：http://oe.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://gr.shxzukj.cn

[U88] JS：对象展开合并
来源：http://xo.huixiangedu.cn

{ ...a, ...b }
来源：http://hg.haigaiapp.cn

[U89] JS：数组去重
来源：http://ef.lnxyls.cn

[...new Set(arr)]
来源：http://ci.nicolike.cn

[U90] JS：数字数组排序
来源：http://om.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://pt.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://vc.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nf.huanxung.cn

[U92] JS：深拷贝
来源：http://pq.jctech888.com.cn

structuredClone(obj)
来源：http://jc.hahajie.cn

[U93] JS：模板字符串
来源：http://ua.bookmarksfly.cn

`共 ${n} 条`
来源：http://kf.hahajie.cn

[U94] JS：箭头函数
来源：http://dr.jianghongdianzi.cn

const double = x => x * 2;
来源：http://uy.panjiajie.cn

[U95] JS：Promise 包装
来源：http://jp.521024.cn

new Promise((resolve, reject) => {})
来源：http://by.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://cc.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tp.szsharing.cn

[U97] JS：并发请求
来源：http://hq.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gf.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ou.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sh.colortex.cn

[U99] JS：事件监听
来源：http://ed.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://nw.9csxet.cn

[U100] JS：DOM 查询
来源：http://zg.panjiajie.cn

document.querySelector(".item")
来源：http://rv.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://pq.hnjuh.cn

el.classList.toggle("active")
来源：http://cj.colortex.cn

[U102] JS：本地存储
来源：http://nl.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gn.jianghongdianzi.cn

[U103] JS：定时器
来源：http://dp.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yj.newstarts.cn

[U104] JS：防抖
来源：http://gi.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.jianghongdianzi.cn

[U105] JS：节流
来源：http://nh.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uf.chemitech.net.cn

[U106] JS：日期格式化
来源：http://ro.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ro.wgjwhj.cn

[U107] JS：数字千分位
来源：http://gj.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vv.colortex.cn

[U108] JS：随机整数
来源：http://kz.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bw.shxzskj.cn

[U109] JS：数组分组
来源：http://pf.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://uo.hnjuh.cn

[U110] JS：数组分块
来源：http://ii.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pv.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://vm.newstarts.cn

new Map(Object.entries(obj))
来源：http://qv.colortex.cn

[U112] JS：字符串补位
来源：http://ok.wgjwhj.cn

"7".padStart(3, "0")
来源：http://lt.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://bo.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://sa.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://ci.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mo.szxytkj.cn

[U115] JS：生成 UUID
来源：http://xp.bjjhwx.cn

crypto.randomUUID()
来源：http://vs.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://ol.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://iv.szxytkj.cn

[U117] JS：单元测试
来源：http://fd.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://yw.shxzskj.cn

[U118] JS：开发服务器
来源：http://ke.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://vx.szsharing.cn

[U119] JS：生产构建
来源：http://vo.huixiangedu.cn

npx vite build
来源：http://rb.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://kj.asd995.cn

import.meta.env.VITE_API_URL
来源：http://yv.huanxung.cn

================================================================================
来源：http://ex.hahajie.cn

统计汇总
来源：http://rp.yuexingan06.cn

================================================================================
来源：http://tg.colortex.cn

按语言统计（条）：
来源：http://fb.bookmarksfly.cn

Python ......... 252
来源：http://iq.huanxung.cn

PHP ............ 252
来源：http://my.szxytkj.cn

JavaScript ..... 252
来源：http://of.nicolike.cn

TypeScript ..... 212
来源：http://am.nszjky.cn

Java ........... 212
来源：http://bn.yuexingan06.cn

Go ............. 212
来源：http://um.9csxet.cn

Ruby ........... 212
来源：http://lm.nicolike.cn

C# ............. 212
来源：http://ej.shxzskj.cn

C .............. 30
来源：http://ld.nszjky.cn

C++ ............ 30
来源：http://ws.panjiajie.cn

SQL ............ 90
来源：http://ql.nszjky.cn

Bash ........... 80
来源：http://ft.lnxyls.cn

Kotlin ......... 15
来源：http://gx.szxytkj.cn

Swift .......... 15
来源：http://ww.shtwfgs.cn

Lua ............ 10
来源：http://kv.lnxyls.cn

Perl ........... 10
来源：http://fn.521024.cn

Scala .......... 10
来源：http://bl.shxzskj.cn

------------------------------------
来源：http://uw.shtwfgs.cn

合计 ........... 2106 条
来源：http://ek.shxzskj.cn

按章节统计：
来源：http://pp.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ta.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://if.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gx.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vu.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ml.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zo.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ci.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jt.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gw.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jl.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yv.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://go.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mj.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://al.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pu.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tf.lnxyls.cn

Q SQL 专题                              90
来源：http://vl.bjjhwx.cn

R Bash 专题                             80
来源：http://vm.shxzukj.cn

S C / C++ 专题                          60
来源：http://vp.9csxet.cn

T 其他语言补充                          60
来源：http://up.lnxyls.cn

U 高频实用片段                         120
来源：http://qh.hnjuh.cn

------------------------------------
来源：http://wh.lnxyls.cn

合计                                  2106 条
来源：http://xy.nszjky.cn

--------------------------------------------------------------------------------
来源：http://js.nszjky.cn

使用提醒
来源：http://lo.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://zh.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://or.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xj.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bi.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zw.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nz.gzmigu.cn

—— 文件结束 ——
来源：http://sc.bjjhwx.cn

================================================================================
来源：http://ep.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://kr.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://hx.nicolike.cn

================================================================================
来源：http://to.huanxung.cn

【收录内容】
来源：http://ou.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oj.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wx.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://bz.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ly.nicolike.cn

【使用说明】
来源：http://jy.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://av.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ux.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ql.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iu.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tm.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lz.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rj.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tt.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ik.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nx.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rg.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jh.bookmarksfly.cn

【文件统计】
来源：http://qh.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xv.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ib.colortex.cn

目  录
来源：http://dj.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://qa.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dv.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://po.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://th.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yt.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jr.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://in.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ni.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://un.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://np.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uj.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ma.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dx.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ev.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jf.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ik.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rl.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mn.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://et.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nk.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dq.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ca.shxzukj.cn

================================================================================
来源：http://mb.gzmigu.cn

A. 基础语法与类型
来源：http://ve.bjjhwx.cn

================================================================================
来源：http://bt.asd995.cn

[A01] Hello World
来源：http://sc.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://ad.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://wy.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://rf.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://re.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://tz.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://ys.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://jr.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://al.nszjky.cn

[A02] 变量声明与赋值
来源：http://cc.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://em.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kl.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tl.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ac.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://fw.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://wp.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://yb.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zj.szxytkj.cn

[A03] 常量定义
来源：http://nm.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lz.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://tj.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://kd.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://kb.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://io.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://og.hahajie.cn

Ruby: PI = 3.14159
来源：http://pe.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://hi.chemitech.net.cn

[A04] 判断变量类型
来源：http://iv.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nb.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xt.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rt.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://ki.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fy.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rw.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iw.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://os.shtwfgs.cn

[A05] 整数除法与取模
来源：http://ex.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yg.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sz.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lm.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yy.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://au.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://vf.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://eo.521024.cn

C#:   7 / 2; 7 % 2
来源：http://wl.jctech888.com.cn

[A06] 字符串转数字
来源：http://ha.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://dj.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ok.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cr.haigaiapp.cn


<!-- 参考信息 -->