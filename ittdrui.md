代发 wailian999

[U55] PHP：match 表达式
来源：http://ch.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kz.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://hy.shxzskj.cn

f(a: 1, b: 2)
来源：http://kr.hahajie.cn

[U57] PHP：字符串插值
来源：http://vh.szsharing.cn

"值: {$a}"
来源：http://hf.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://ta.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uo.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://rz.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bt.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://mu.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ww.yuexingan06.cn

[U61] PHP：正则
来源：http://wo.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tl.shtwfgs.cn

[U62] PHP：日期对象
来源：http://in.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ru.9csxet.cn

[U63] PHP：文件读写
来源：http://om.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zd.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://lm.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://tp.yuexingan06.cn

[U65] PHP：会话
来源：http://fe.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ud.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://yu.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dh.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://gk.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rt.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://ej.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mq.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://vf.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://km.colortex.cn

[U70] PHP：PDO 事务
来源：http://ht.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wm.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://pa.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://ty.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://bc.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://gg.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://pc.521024.cn

parse_ini_file("config.ini", true)
来源：http://as.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://uq.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://vc.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://vx.jianghongdianzi.cn

composer require psr/container
来源：http://ds.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://zj.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xv.hahajie.cn

[U77] PHP：模板渲染
来源：http://sj.nszjky.cn

composer require twig/twig
来源：http://wv.szsharing.cn

[U78] PHP：单元测试
来源：http://ge.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://wk.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://zd.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://zb.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ni.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://be.hnjuh.cn

[U81] JS：初始化项目
来源：http://ku.hnjuh.cn

npm init -y;  npm i express
来源：http://pt.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://ic.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wt.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://mf.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fr.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://ky.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kt.bjjhwx.cn

[U85] JS：可选链
来源：http://rj.chemitech.net.cn

a?.b?.c
来源：http://sc.shtwfgs.cn

[U86] JS：空值合并
来源：http://jv.jianghongdianzi.cn

a ?? b
来源：http://ow.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://dt.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://dc.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://gt.jianghongdianzi.cn

{ ...a, ...b }
来源：http://yk.jctech888.com.cn

[U89] JS：数组去重
来源：http://hx.yuexingan06.cn

[...new Set(arr)]
来源：http://ep.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://rs.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://cb.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://hm.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cb.haigaiapp.cn

[U92] JS：深拷贝
来源：http://nq.muxihuayi.cn

structuredClone(obj)
来源：http://ia.chemitech.net.cn

[U93] JS：模板字符串
来源：http://vz.9csxet.cn

`共 ${n} 条`
来源：http://qr.jctech888.com.cn

[U94] JS：箭头函数
来源：http://ux.9csxet.cn

const double = x => x * 2;
来源：http://kn.asd995.cn

[U95] JS：Promise 包装
来源：http://hm.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://cm.nicolike.cn

[U96] JS：async/await 与异常
来源：http://qf.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aa.wgjwhj.cn

[U97] JS：并发请求
来源：http://wh.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eg.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://fa.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yr.shtwfgs.cn

[U99] JS：事件监听
来源：http://di.szsharing.cn

el.addEventListener("click", e => {})
来源：http://wl.asd995.cn

[U100] JS：DOM 查询
来源：http://di.chemitech.net.cn

document.querySelector(".item")
来源：http://px.nszjky.cn

[U101] JS：classList 操作
来源：http://dq.jctech888.com.cn

el.classList.toggle("active")
来源：http://rj.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://ks.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lj.panjiajie.cn

[U103] JS：定时器
来源：http://us.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nc.nicolike.cn

[U104] JS：防抖
来源：http://fj.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lv.nicolike.cn

[U105] JS：节流
来源：http://rx.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iw.huixiangedu.cn

[U106] JS：日期格式化
来源：http://vq.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sa.panjiajie.cn

[U107] JS：数字千分位
来源：http://jg.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lf.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ns.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xs.hahajie.cn

[U109] JS：数组分组
来源：http://tv.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://sw.szxytkj.cn

[U110] JS：数组分块
来源：http://tl.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://di.huanxung.cn

[U111] JS：对象转 Map
来源：http://ck.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://cj.yuexingan06.cn

[U112] JS：字符串补位
来源：http://dq.hnjuh.cn

"7".padStart(3, "0")
来源：http://em.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://jf.szsharing.cn

s.replaceAll("a", "b")
来源：http://gy.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://it.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ob.colortex.cn

[U115] JS：生成 UUID
来源：http://wv.9csxet.cn

crypto.randomUUID()
来源：http://vc.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://kp.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://pe.shxzskj.cn

[U117] JS：单元测试
来源：http://dd.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://li.asd995.cn

[U118] JS：开发服务器
来源：http://bm.szxytkj.cn

npm i -D vite;  npx vite
来源：http://sz.gzmigu.cn

[U119] JS：生产构建
来源：http://ju.szsharing.cn

npx vite build
来源：http://vg.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://db.colortex.cn

import.meta.env.VITE_API_URL
来源：http://ck.yuntaijiaju.cn

================================================================================
来源：http://gh.gzmigu.cn

统计汇总
来源：http://su.bookmarksfly.cn

================================================================================
来源：http://py.panjiajie.cn

按语言统计（条）：
来源：http://pe.asd995.cn

Python ......... 252
来源：http://so.chemitech.net.cn

PHP ............ 252
来源：http://ph.szsharing.cn

JavaScript ..... 252
来源：http://bb.521024.cn

TypeScript ..... 212
来源：http://yn.chemitech.net.cn

Java ........... 212
来源：http://hi.colortex.cn

Go ............. 212
来源：http://rs.colortex.cn

Ruby ........... 212
来源：http://up.huixiangedu.cn

C# ............. 212
来源：http://nj.gzmigu.cn

C .............. 30
来源：http://du.jctech888.com.cn

C++ ............ 30
来源：http://pd.huanxung.cn

SQL ............ 90
来源：http://oz.yuntaijiaju.cn

Bash ........... 80
来源：http://df.bookmarksfly.cn

Kotlin ......... 15
来源：http://ik.hahajie.cn

Swift .......... 15
来源：http://ax.panjiajie.cn

Lua ............ 10
来源：http://zq.newstarts.cn

Perl ........... 10
来源：http://sy.colortex.cn

Scala .......... 10
来源：http://co.muxihuayi.cn

------------------------------------
来源：http://bz.shtwfgs.cn

合计 ........... 2106 条
来源：http://wo.bjjhwx.cn

按章节统计：
来源：http://uf.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fz.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yo.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ue.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jk.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zp.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tk.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fe.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zq.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gj.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ln.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lh.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sw.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://np.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hh.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wu.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qn.gzmigu.cn

Q SQL 专题                              90
来源：http://ew.newstarts.cn

R Bash 专题                             80
来源：http://kk.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://hv.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://qx.hahajie.cn

U 高频实用片段                         120
来源：http://lm.gzmigu.cn

------------------------------------
来源：http://lb.colortex.cn

合计                                  2106 条
来源：http://tx.newstarts.cn

--------------------------------------------------------------------------------
来源：http://bk.asd995.cn

使用提醒
来源：http://yf.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://zf.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dx.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ma.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mr.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ye.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kg.huanxung.cn

—— 文件结束 ——
来源：http://gs.521024.cn

================================================================================
来源：http://bb.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://bq.521024.cn

Common Programming Examples Cheat Book
来源：http://ln.shxzukj.cn

================================================================================
来源：http://uo.hnjuh.cn

【收录内容】
来源：http://zk.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ld.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zg.jctech888.com.cn

SQL · Bash · C · C++
来源：http://bh.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ux.shxzskj.cn

【使用说明】
来源：http://fs.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cq.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lj.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wg.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pb.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jx.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wo.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mw.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hr.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wp.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bk.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lq.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nm.wgjwhj.cn

【文件统计】
来源：http://lw.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ol.szsharing.cn

--------------------------------------------------------------------------------
来源：http://op.hahajie.cn

目  录
来源：http://nq.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://og.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hl.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yt.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dc.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cn.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ah.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jm.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://er.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zr.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kw.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kr.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ik.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rs.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jh.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fm.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gw.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yn.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jz.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oh.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ip.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qp.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pb.szsharing.cn

================================================================================
来源：http://be.shxzukj.cn

A. 基础语法与类型
来源：http://zm.bookmarksfly.cn

================================================================================
来源：http://ga.szxytkj.cn

[A01] Hello World
来源：http://cl.newstarts.cn

Py:   print("Hello, World!")
来源：http://ew.colortex.cn

PHP:  echo "Hello, World!";
来源：http://cz.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://yi.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ti.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://oa.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://dz.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://zk.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nl.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://yu.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sc.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wq.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zz.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zx.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://kn.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://pz.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://ki.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pf.huixinmuqiang.cn

[A03] 常量定义
来源：http://ha.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kr.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://dz.newstarts.cn

JS:   const PI = 3.14159;
来源：http://fg.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://co.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://gi.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://uc.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://fv.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://jy.wgjwhj.cn

[A04] 判断变量类型
来源：http://bh.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pd.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qr.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ol.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://kp.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yh.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kg.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zd.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://vs.colortex.cn

[A05] 整数除法与取模
来源：http://cd.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lv.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bz.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gw.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sa.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://dz.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://tw.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://vm.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://vc.huanxung.cn

[A06] 字符串转数字
来源：http://rc.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://ul.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yy.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ly.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rj.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xj.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://at.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cj.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eu.hnjuh.cn

[A07] 数字转字符串
来源：http://gb.9csxet.cn

Py:   str(42)
来源：http://fp.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://bo.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://ae.colortex.cn

TS:   String(42)
来源：http://nw.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qp.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://gs.bookmarksfly.cn


<!-- 参考信息 -->