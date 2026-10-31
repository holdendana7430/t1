代发 wailian999

[U49] PHP：只读属性
来源：http://pm.shxzskj.cn

public readonly string $name
来源：http://fg.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://zl.nszjky.cn

public function __construct(private int $id) {}
来源：http://yh.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://eg.jctech888.com.cn

[$a, $b] = $arr;
来源：http://tv.szxytkj.cn

[U52] PHP：箭头函数
来源：http://az.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://uq.9csxet.cn

[U53] PHP：空合并运算符
来源：http://dq.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://vx.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://mf.bookmarksfly.cn

$obj?->method()
来源：http://br.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://gg.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wp.shxzukj.cn

[U56] PHP：命名参数
来源：http://km.nicolike.cn

f(a: 1, b: 2)
来源：http://ut.hnjuh.cn

[U57] PHP：字符串插值
来源：http://lx.hnjuh.cn

"值: {$a}"
来源：http://hk.shxzukj.cn

[U58] PHP：数组三件套
来源：http://as.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://di.hahajie.cn

[U59] PHP：自定义排序
来源：http://er.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hi.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://gc.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jc.panjiajie.cn

[U61] PHP：正则
来源：http://lz.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bo.9csxet.cn

[U62] PHP：日期对象
来源：http://ni.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rj.jctech888.com.cn

[U63] PHP：文件读写
来源：http://gf.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pz.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://wi.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://wg.jianghongdianzi.cn

[U65] PHP：会话
来源：http://ym.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ke.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://yn.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://te.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://yo.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vs.hahajie.cn

[U68] PHP：PDO 连接
来源：http://bd.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://um.colortex.cn

[U69] PHP：PDO 预处理
来源：http://rs.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wu.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://nq.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wf.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://dv.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://st.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://rv.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://or.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://if.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://vs.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ca.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://dz.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://xd.jianghongdianzi.cn

composer require psr/container
来源：http://dj.bjjhwx.cn

[U76] PHP：简单路由
来源：http://zi.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://st.shxzskj.cn

[U77] PHP：模板渲染
来源：http://ie.wgjwhj.cn

composer require twig/twig
来源：http://ft.shtwfgs.cn

[U78] PHP：单元测试
来源：http://iq.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://pr.szsharing.cn

[U79] PHP：静态分析
来源：http://fo.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://to.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ix.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fo.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ay.yuexingan06.cn

npm init -y;  npm i express
来源：http://ar.hahajie.cn

[U82] JS：package.json 脚本
来源：http://ls.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wv.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://fe.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yv.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://qw.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://en.9csxet.cn

[U85] JS：可选链
来源：http://fe.panjiajie.cn

a?.b?.c
来源：http://kt.jctech888.com.cn

[U86] JS：空值合并
来源：http://wa.shxzukj.cn

a ?? b
来源：http://jv.szsharing.cn

[U87] JS：解构默认值
来源：http://jk.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://zv.shxzskj.cn

[U88] JS：对象展开合并
来源：http://fu.nicolike.cn

{ ...a, ...b }
来源：http://or.panjiajie.cn

[U89] JS：数组去重
来源：http://fn.jianghongdianzi.cn

[...new Set(arr)]
来源：http://ot.shxzukj.cn

[U90] JS：数字数组排序
来源：http://xs.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://nf.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://az.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zd.huanxung.cn

[U92] JS：深拷贝
来源：http://kf.shxzukj.cn

structuredClone(obj)
来源：http://cg.wgjwhj.cn

[U93] JS：模板字符串
来源：http://ly.colortex.cn

`共 ${n} 条`
来源：http://lk.nszjky.cn

[U94] JS：箭头函数
来源：http://rl.bjjhwx.cn

const double = x => x * 2;
来源：http://eq.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://cw.521024.cn

new Promise((resolve, reject) => {})
来源：http://fw.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://tz.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fh.szxytkj.cn

[U97] JS：并发请求
来源：http://gs.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ma.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://cm.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ce.muxihuayi.cn

[U99] JS：事件监听
来源：http://bt.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://fn.9csxet.cn

[U100] JS：DOM 查询
来源：http://wc.wgjwhj.cn

document.querySelector(".item")
来源：http://xx.haigaiapp.cn

[U101] JS：classList 操作
来源：http://lz.gzmigu.cn

el.classList.toggle("active")
来源：http://mk.shtwfgs.cn

[U102] JS：本地存储
来源：http://os.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sv.521024.cn

[U103] JS：定时器
来源：http://by.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kz.bjjhwx.cn

[U104] JS：防抖
来源：http://lb.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gk.huanxung.cn

[U105] JS：节流
来源：http://ds.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ua.yuexingan06.cn

[U106] JS：日期格式化
来源：http://qv.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pu.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://vs.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ch.haigaiapp.cn

[U108] JS：随机整数
来源：http://qx.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zp.gzmigu.cn

[U109] JS：数组分组
来源：http://wl.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://xw.nszjky.cn

[U110] JS：数组分块
来源：http://cs.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fo.hnjuh.cn

[U111] JS：对象转 Map
来源：http://rr.newstarts.cn

new Map(Object.entries(obj))
来源：http://fq.9csxet.cn

[U112] JS：字符串补位
来源：http://ij.yuexingan06.cn

"7".padStart(3, "0")
来源：http://xj.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://jg.gzmigu.cn

s.replaceAll("a", "b")
来源：http://em.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://xq.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xk.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://fv.nszjky.cn

crypto.randomUUID()
来源：http://fw.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://qd.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ta.521024.cn

[U117] JS：单元测试
来源：http://bu.colortex.cn

npm i -D vitest;  npx vitest
来源：http://eg.panjiajie.cn

[U118] JS：开发服务器
来源：http://vu.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://nm.9csxet.cn

[U119] JS：生产构建
来源：http://ot.huixiangedu.cn

npx vite build
来源：http://mv.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://sh.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://zf.szxytkj.cn

================================================================================
来源：http://xp.szxytkj.cn

统计汇总
来源：http://cf.bjjhwx.cn

================================================================================
来源：http://cq.wgjwhj.cn

按语言统计（条）：
来源：http://gt.muxihuayi.cn

Python ......... 252
来源：http://cu.shxzskj.cn

PHP ............ 252
来源：http://ik.yuexingan06.cn

JavaScript ..... 252
来源：http://ug.nszjky.cn

TypeScript ..... 212
来源：http://bs.gzmigu.cn

Java ........... 212
来源：http://ga.asd995.cn

Go ............. 212
来源：http://zj.wgjwhj.cn

Ruby ........... 212
来源：http://xp.huanxung.cn

C# ............. 212
来源：http://xj.nszjky.cn

C .............. 30
来源：http://mj.muxihuayi.cn

C++ ............ 30
来源：http://gv.colortex.cn

SQL ............ 90
来源：http://cu.szsharing.cn

Bash ........... 80
来源：http://bk.wgjwhj.cn

Kotlin ......... 15
来源：http://oj.hahajie.cn

Swift .......... 15
来源：http://ux.9csxet.cn

Lua ............ 10
来源：http://ge.asd995.cn

Perl ........... 10
来源：http://iy.chemitech.net.cn

Scala .......... 10
来源：http://hs.huixiangedu.cn

------------------------------------
来源：http://wc.shtwfgs.cn

合计 ........... 2106 条
来源：http://ib.szxytkj.cn

按章节统计：
来源：http://ev.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yn.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ee.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://am.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pc.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gj.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fi.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yi.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rg.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://od.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yp.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://av.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hw.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lt.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kq.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://al.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kr.nszjky.cn

Q SQL 专题                              90
来源：http://dm.huixinmuqiang.cn

R Bash 专题                             80
来源：http://uv.asd995.cn

S C / C++ 专题                          60
来源：http://rm.haigaiapp.cn

T 其他语言补充                          60
来源：http://eg.yuexingan06.cn

U 高频实用片段                         120
来源：http://aq.gzmigu.cn

------------------------------------
来源：http://ha.shxzskj.cn

合计                                  2106 条
来源：http://rq.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://pk.gzmigu.cn

使用提醒
来源：http://qb.hahajie.cn

--------------------------------------------------------------------------------
来源：http://yn.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yq.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://de.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hi.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qq.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fh.wgjwhj.cn

—— 文件结束 ——
来源：http://wp.521024.cn

================================================================================
来源：http://dr.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://va.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://yf.muxihuayi.cn

================================================================================
来源：http://ed.asd995.cn

【收录内容】
来源：http://mx.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dk.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rn.szxytkj.cn

SQL · Bash · C · C++
来源：http://jy.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zd.nszjky.cn

【使用说明】
来源：http://qc.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zz.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hd.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://im.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zt.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zt.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ub.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://re.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pd.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ny.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mw.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ex.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ax.newstarts.cn

【文件统计】
来源：http://zm.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xj.huanxung.cn

--------------------------------------------------------------------------------
来源：http://kz.nicolike.cn

目  录
来源：http://go.nicolike.cn

--------------------------------------------------------------------------------
来源：http://eq.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://db.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ng.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uu.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rg.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gy.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zf.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oi.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vn.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ku.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mn.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yu.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ol.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ny.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ly.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ex.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gu.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ik.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dz.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sk.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ha.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xr.huanxung.cn

================================================================================
来源：http://ij.newstarts.cn

A. 基础语法与类型
来源：http://ut.haigaiapp.cn

================================================================================
来源：http://ik.jianghongdianzi.cn

[A01] Hello World
来源：http://rw.nicolike.cn

Py:   print("Hello, World!")
来源：http://pi.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://qj.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://bl.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nj.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://qx.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://uy.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://yc.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sk.szxytkj.cn

[A02] 变量声明与赋值
来源：http://ie.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://no.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ri.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://om.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dt.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://nf.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://pr.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://zu.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zn.asd995.cn

[A03] 常量定义
来源：http://lz.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hx.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://xc.newstarts.cn

JS:   const PI = 3.14159;
来源：http://xb.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://we.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ko.nicolike.cn

Go:   const PI = 3.14159
来源：http://nu.lnxyls.cn

Ruby: PI = 3.14159
来源：http://hc.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://dz.bjjhwx.cn

[A04] 判断变量类型
来源：http://mf.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bv.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ro.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nq.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://tu.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wu.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oi.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tf.521024.cn

C#:   x.GetType().Name; x is int
来源：http://er.shtwfgs.cn

[A05] 整数除法与取模
来源：http://lf.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://td.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vh.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qq.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ll.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://th.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://vc.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://bt.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://by.hnjuh.cn

[A06] 字符串转数字
来源：http://pz.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://rb.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://da.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ax.jctech888.com.cn


<!-- 参考信息 -->