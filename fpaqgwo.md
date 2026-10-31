代发 wailian999

[U51] PHP：数组解构
来源：http://cx.chemitech.net.cn

[$a, $b] = $arr;
来源：http://vj.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://xw.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://dm.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://uc.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://ap.521024.cn

[U54] PHP：空安全调用
来源：http://qx.szxytkj.cn

$obj?->method()
来源：http://ez.nszjky.cn

[U55] PHP：match 表达式
来源：http://gx.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yy.hnjuh.cn

[U56] PHP：命名参数
来源：http://at.yuexingan06.cn

f(a: 1, b: 2)
来源：http://mg.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://wl.newstarts.cn

"值: {$a}"
来源：http://jz.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://ay.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jz.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://pl.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zl.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://uj.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eq.haigaiapp.cn

[U61] PHP：正则
来源：http://pd.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sr.hahajie.cn

[U62] PHP：日期对象
来源：http://be.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nx.szsharing.cn

[U63] PHP：文件读写
来源：http://dq.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fe.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://ir.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://uj.shxzukj.cn

[U65] PHP：会话
来源：http://eo.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mh.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://sc.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ip.asd995.cn

[U67] PHP：处理文件上传
来源：http://pv.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cw.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ij.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mc.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://su.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mh.huanxung.cn

[U70] PHP：PDO 事务
来源：http://ca.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gf.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://wu.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://hg.lnxyls.cn

[U72] PHP：写错误日志
来源：http://tb.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://lp.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://xu.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://ed.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://hh.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://cd.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://yb.9csxet.cn

composer require psr/container
来源：http://cm.shtwfgs.cn

[U76] PHP：简单路由
来源：http://vi.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ag.newstarts.cn

[U77] PHP：模板渲染
来源：http://mt.asd995.cn

composer require twig/twig
来源：http://zm.nicolike.cn

[U78] PHP：单元测试
来源：http://md.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://yx.panjiajie.cn

[U79] PHP：静态分析
来源：http://eb.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://hi.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://ip.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ym.bjjhwx.cn

[U81] JS：初始化项目
来源：http://qv.panjiajie.cn

npm init -y;  npm i express
来源：http://pf.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://oz.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oa.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://rx.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rk.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://mq.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gv.newstarts.cn

[U85] JS：可选链
来源：http://js.huanxung.cn

a?.b?.c
来源：http://dw.bjjhwx.cn

[U86] JS：空值合并
来源：http://ou.hahajie.cn

a ?? b
来源：http://oy.hnjuh.cn

[U87] JS：解构默认值
来源：http://ei.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://oi.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://rm.9csxet.cn

{ ...a, ...b }
来源：http://yi.jctech888.com.cn

[U89] JS：数组去重
来源：http://af.521024.cn

[...new Set(arr)]
来源：http://im.521024.cn

[U90] JS：数字数组排序
来源：http://wu.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://so.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://za.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fd.huanxung.cn

[U92] JS：深拷贝
来源：http://tk.gzmigu.cn

structuredClone(obj)
来源：http://gw.haigaiapp.cn

[U93] JS：模板字符串
来源：http://ey.yuntaijiaju.cn

`共 ${n} 条`
来源：http://yg.shtwfgs.cn

[U94] JS：箭头函数
来源：http://va.shxzskj.cn

const double = x => x * 2;
来源：http://rh.shxzskj.cn

[U95] JS：Promise 包装
来源：http://qp.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://gv.newstarts.cn

[U96] JS：async/await 与异常
来源：http://ze.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ok.panjiajie.cn

[U97] JS：并发请求
来源：http://tz.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lk.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ag.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cj.chemitech.net.cn

[U99] JS：事件监听
来源：http://tw.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://xi.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://nn.huixinmuqiang.cn

document.querySelector(".item")
来源：http://og.shxzskj.cn

[U101] JS：classList 操作
来源：http://fn.9csxet.cn

el.classList.toggle("active")
来源：http://xx.hnjuh.cn

[U102] JS：本地存储
来源：http://fa.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ak.asd995.cn

[U103] JS：定时器
来源：http://ft.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kp.bookmarksfly.cn

[U104] JS：防抖
来源：http://kp.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jl.shtwfgs.cn

[U105] JS：节流
来源：http://sa.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://li.huanxung.cn

[U106] JS：日期格式化
来源：http://vh.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bm.521024.cn

[U107] JS：数字千分位
来源：http://oh.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://na.wgjwhj.cn

[U108] JS：随机整数
来源：http://cx.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wt.asd995.cn

[U109] JS：数组分组
来源：http://bq.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://gq.9csxet.cn

[U110] JS：数组分块
来源：http://on.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zr.521024.cn

[U111] JS：对象转 Map
来源：http://nd.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://vf.hnjuh.cn

[U112] JS：字符串补位
来源：http://ak.szsharing.cn

"7".padStart(3, "0")
来源：http://az.gzmigu.cn

[U113] JS：正则替换全部
来源：http://vq.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://dc.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://af.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rp.szxytkj.cn

[U115] JS：生成 UUID
来源：http://fu.newstarts.cn

crypto.randomUUID()
来源：http://yz.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://zz.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ol.bookmarksfly.cn

[U117] JS：单元测试
来源：http://be.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://bb.newstarts.cn

[U118] JS：开发服务器
来源：http://ck.panjiajie.cn

npm i -D vite;  npx vite
来源：http://pa.wgjwhj.cn

[U119] JS：生产构建
来源：http://ab.shxzukj.cn

npx vite build
来源：http://lf.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://aj.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://oh.shtwfgs.cn

================================================================================
来源：http://io.nszjky.cn

统计汇总
来源：http://ut.bookmarksfly.cn

================================================================================
来源：http://ce.yuntaijiaju.cn

按语言统计（条）：
来源：http://ga.szsharing.cn

Python ......... 252
来源：http://gv.jianghongdianzi.cn

PHP ............ 252
来源：http://zl.bjjhwx.cn

JavaScript ..... 252
来源：http://we.szsharing.cn

TypeScript ..... 212
来源：http://rl.jianghongdianzi.cn

Java ........... 212
来源：http://gm.newstarts.cn

Go ............. 212
来源：http://jl.chemitech.net.cn

Ruby ........... 212
来源：http://lj.hahajie.cn

C# ............. 212
来源：http://cf.panjiajie.cn

C .............. 30
来源：http://cp.szxytkj.cn

C++ ............ 30
来源：http://kf.asd995.cn

SQL ............ 90
来源：http://ue.colortex.cn

Bash ........... 80
来源：http://ft.yuexingan06.cn

Kotlin ......... 15
来源：http://uz.bjjhwx.cn

Swift .......... 15
来源：http://vz.panjiajie.cn

Lua ............ 10
来源：http://fh.9csxet.cn

Perl ........... 10
来源：http://md.hahajie.cn

Scala .......... 10
来源：http://nq.yuexingan06.cn

------------------------------------
来源：http://qa.shtwfgs.cn

合计 ........... 2106 条
来源：http://yf.hahajie.cn

按章节统计：
来源：http://qj.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mz.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wd.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gv.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tu.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uz.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mf.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mj.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ol.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bm.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mi.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://at.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iw.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ij.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zk.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fk.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bz.asd995.cn

Q SQL 专题                              90
来源：http://hw.hahajie.cn

R Bash 专题                             80
来源：http://ay.lnxyls.cn

S C / C++ 专题                          60
来源：http://bm.szxytkj.cn

T 其他语言补充                          60
来源：http://wm.shxzukj.cn

U 高频实用片段                         120
来源：http://ya.9csxet.cn

------------------------------------
来源：http://sl.asd995.cn

合计                                  2106 条
来源：http://xc.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ao.jianghongdianzi.cn

使用提醒
来源：http://su.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://cv.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jw.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ms.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ld.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jc.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fo.shxzukj.cn

—— 文件结束 ——
来源：http://cs.shxzukj.cn

================================================================================
来源：http://ot.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://rf.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://wh.yuexingan06.cn

================================================================================
来源：http://hn.521024.cn

【收录内容】
来源：http://ch.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nl.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jm.bjjhwx.cn

SQL · Bash · C · C++
来源：http://pb.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pk.nicolike.cn

【使用说明】
来源：http://aj.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kz.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kk.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kr.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zk.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zu.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gl.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qy.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wm.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ch.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://os.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oj.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tl.panjiajie.cn

【文件统计】
来源：http://bl.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hb.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://tl.haigaiapp.cn

目  录
来源：http://ec.521024.cn

--------------------------------------------------------------------------------
来源：http://tl.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qt.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://di.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zb.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bq.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qh.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xg.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nl.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kn.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ui.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ok.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oa.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hi.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ur.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fm.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ne.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uv.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gb.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://go.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vm.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gu.yuntaijiaju.cn

================================================================================
来源：http://jw.bookmarksfly.cn

A. 基础语法与类型
来源：http://rg.nszjky.cn

================================================================================
来源：http://gn.hahajie.cn

[A01] Hello World
来源：http://vj.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://et.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://po.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://xj.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://th.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://hw.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://jx.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://af.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yv.colortex.cn

[A02] 变量声明与赋值
来源：http://pg.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vm.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kp.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vi.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pi.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://ip.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://rb.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://qk.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cp.wgjwhj.cn

[A03] 常量定义
来源：http://ql.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jc.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://vn.huanxung.cn

JS:   const PI = 3.14159;
来源：http://lm.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://hv.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://sm.szsharing.cn

Go:   const PI = 3.14159
来源：http://jj.shxzukj.cn

Ruby: PI = 3.14159
来源：http://we.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://mo.huanxung.cn

[A04] 判断变量类型
来源：http://ox.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fn.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://og.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zg.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://wr.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vl.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oc.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uo.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://gi.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://ye.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nm.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qf.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dh.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rh.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://nl.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://py.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://sj.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://il.9csxet.cn

[A06] 字符串转数字
来源：http://sp.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://ya.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wh.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wf.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bj.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wk.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ai.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uc.gzmigu.cn


<!-- 参考信息 -->