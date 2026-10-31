代发 wailian999

[U49] PHP：只读属性
来源：http://br.huixiangedu.cn

public readonly string $name
来源：http://jo.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://bh.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://uf.szsharing.cn

[U51] PHP：数组解构
来源：http://jy.newstarts.cn

[$a, $b] = $arr;
来源：http://tu.nicolike.cn

[U52] PHP：箭头函数
来源：http://wo.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://uf.newstarts.cn

[U53] PHP：空合并运算符
来源：http://px.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://cu.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://wc.huixinmuqiang.cn

$obj?->method()
来源：http://hj.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://vv.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ws.521024.cn

[U56] PHP：命名参数
来源：http://zf.panjiajie.cn

f(a: 1, b: 2)
来源：http://ma.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://it.shxzukj.cn

"值: {$a}"
来源：http://qj.asd995.cn

[U58] PHP：数组三件套
来源：http://kf.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yb.521024.cn

[U59] PHP：自定义排序
来源：http://cn.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nk.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://bw.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ty.hahajie.cn

[U61] PHP：正则
来源：http://qq.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://to.521024.cn

[U62] PHP：日期对象
来源：http://pu.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ct.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ix.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fw.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://jt.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://zq.bookmarksfly.cn

[U65] PHP：会话
来源：http://us.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cq.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://to.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sy.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://yx.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sw.huanxung.cn

[U68] PHP：PDO 连接
来源：http://xr.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xw.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://ue.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kt.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://gg.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qc.newstarts.cn

[U71] PHP：抛出异常
来源：http://rr.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://pi.asd995.cn

[U72] PHP：写错误日志
来源：http://tz.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://kg.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://be.asd995.cn

parse_ini_file("config.ini", true)
来源：http://oy.newstarts.cn

[U74] PHP：读取环境变量
来源：http://gj.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://ux.nicolike.cn

[U75] PHP：依赖注入
来源：http://rx.huixiangedu.cn

composer require psr/container
来源：http://eu.szsharing.cn

[U76] PHP：简单路由
来源：http://nb.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nt.gzmigu.cn

[U77] PHP：模板渲染
来源：http://be.shxzukj.cn

composer require twig/twig
来源：http://pt.hahajie.cn

[U78] PHP：单元测试
来源：http://pf.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://py.shxzukj.cn

[U79] PHP：静态分析
来源：http://cb.asd995.cn

composer require --dev phpstan/phpstan
来源：http://qk.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://td.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sg.muxihuayi.cn

[U81] JS：初始化项目
来源：http://lo.szsharing.cn

npm init -y;  npm i express
来源：http://kz.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://dc.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://un.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://kd.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://td.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://fa.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ie.gzmigu.cn

[U85] JS：可选链
来源：http://zr.muxihuayi.cn

a?.b?.c
来源：http://ml.huixiangedu.cn

[U86] JS：空值合并
来源：http://ot.szsharing.cn

a ?? b
来源：http://oa.shxzskj.cn

[U87] JS：解构默认值
来源：http://vh.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://zi.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://sz.shxzukj.cn

{ ...a, ...b }
来源：http://dj.bookmarksfly.cn

[U89] JS：数组去重
来源：http://cy.jianghongdianzi.cn

[...new Set(arr)]
来源：http://vm.asd995.cn

[U90] JS：数字数组排序
来源：http://mu.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ya.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://jn.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://my.bjjhwx.cn

[U92] JS：深拷贝
来源：http://hv.jianghongdianzi.cn

structuredClone(obj)
来源：http://ov.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://pg.hahajie.cn

`共 ${n} 条`
来源：http://un.hahajie.cn

[U94] JS：箭头函数
来源：http://fw.colortex.cn

const double = x => x * 2;
来源：http://nw.szsharing.cn

[U95] JS：Promise 包装
来源：http://oc.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://kl.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://eu.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://et.panjiajie.cn

[U97] JS：并发请求
来源：http://qq.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://un.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://uo.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rm.huanxung.cn

[U99] JS：事件监听
来源：http://ms.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://kf.lnxyls.cn

[U100] JS：DOM 查询
来源：http://hh.gzmigu.cn

document.querySelector(".item")
来源：http://ua.haigaiapp.cn

[U101] JS：classList 操作
来源：http://jc.newstarts.cn

el.classList.toggle("active")
来源：http://xw.nszjky.cn

[U102] JS：本地存储
来源：http://tb.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://am.bookmarksfly.cn

[U103] JS：定时器
来源：http://np.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mz.huanxung.cn

[U104] JS：防抖
来源：http://fw.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jd.wgjwhj.cn

[U105] JS：节流
来源：http://wp.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yt.wgjwhj.cn

[U106] JS：日期格式化
来源：http://qy.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cz.chemitech.net.cn

[U107] JS：数字千分位
来源：http://hw.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://su.hnjuh.cn

[U108] JS：随机整数
来源：http://gn.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dt.haigaiapp.cn

[U109] JS：数组分组
来源：http://zg.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://zr.panjiajie.cn

[U110] JS：数组分块
来源：http://xh.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qq.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://ww.nszjky.cn

new Map(Object.entries(obj))
来源：http://za.hnjuh.cn

[U112] JS：字符串补位
来源：http://pj.yuexingan06.cn

"7".padStart(3, "0")
来源：http://vq.lnxyls.cn

[U113] JS：正则替换全部
来源：http://jy.521024.cn

s.replaceAll("a", "b")
来源：http://zd.asd995.cn

[U114] JS：JSON 深比较
来源：http://qx.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://js.gzmigu.cn

[U115] JS：生成 UUID
来源：http://dq.hahajie.cn

crypto.randomUUID()
来源：http://yg.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://hf.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://lz.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://bz.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://we.szsharing.cn

[U118] JS：开发服务器
来源：http://ti.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://vc.lnxyls.cn

[U119] JS：生产构建
来源：http://wt.jctech888.com.cn

npx vite build
来源：http://ur.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://zu.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://wq.yuexingan06.cn

================================================================================
来源：http://oi.gzmigu.cn

统计汇总
来源：http://aa.szxytkj.cn

================================================================================
来源：http://yp.lnxyls.cn

按语言统计（条）：
来源：http://ny.colortex.cn

Python ......... 252
来源：http://ab.panjiajie.cn

PHP ............ 252
来源：http://bd.asd995.cn

JavaScript ..... 252
来源：http://wf.bookmarksfly.cn

TypeScript ..... 212
来源：http://zu.wgjwhj.cn

Java ........... 212
来源：http://iv.nszjky.cn

Go ............. 212
来源：http://nk.nicolike.cn

Ruby ........... 212
来源：http://oc.panjiajie.cn

C# ............. 212
来源：http://jm.szsharing.cn

C .............. 30
来源：http://bu.shxzukj.cn

C++ ............ 30
来源：http://ui.gzmigu.cn

SQL ............ 90
来源：http://nx.haigaiapp.cn

Bash ........... 80
来源：http://tz.bookmarksfly.cn

Kotlin ......... 15
来源：http://qa.hnjuh.cn

Swift .......... 15
来源：http://ab.shtwfgs.cn

Lua ............ 10
来源：http://dk.muxihuayi.cn

Perl ........... 10
来源：http://vz.yuntaijiaju.cn

Scala .......... 10
来源：http://vi.shtwfgs.cn

------------------------------------
来源：http://wg.gzmigu.cn

合计 ........... 2106 条
来源：http://aw.panjiajie.cn

按章节统计：
来源：http://ep.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kp.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yi.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bw.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sq.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ae.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ko.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uh.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ad.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tu.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ou.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oy.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rp.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ac.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vg.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gc.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ht.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://vk.hnjuh.cn

R Bash 专题                             80
来源：http://ms.9csxet.cn

S C / C++ 专题                          60
来源：http://ve.huanxung.cn

T 其他语言补充                          60
来源：http://ni.shxzskj.cn

U 高频实用片段                         120
来源：http://jl.yuexingan06.cn

------------------------------------
来源：http://ex.panjiajie.cn

合计                                  2106 条
来源：http://ud.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://is.hahajie.cn

使用提醒
来源：http://zf.szsharing.cn

--------------------------------------------------------------------------------
来源：http://zk.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ju.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dz.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cj.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sy.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iu.nicolike.cn

—— 文件结束 ——
来源：http://kj.bjjhwx.cn

================================================================================
来源：http://os.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://lg.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://zh.hnjuh.cn

================================================================================
来源：http://hv.yuntaijiaju.cn

【收录内容】
来源：http://ij.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sg.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ju.colortex.cn

SQL · Bash · C · C++
来源：http://ei.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kx.newstarts.cn

【使用说明】
来源：http://rt.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rm.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qr.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wn.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mt.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rt.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nf.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hq.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://py.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bi.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lm.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://py.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ic.huixiangedu.cn

【文件统计】
来源：http://wk.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yj.huanxung.cn

--------------------------------------------------------------------------------
来源：http://tx.gzmigu.cn

目  录
来源：http://iq.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://kn.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yt.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tx.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zn.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ts.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wq.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hq.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iu.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tk.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ss.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cm.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ol.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lc.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qm.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rt.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eb.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fy.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sv.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xz.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eo.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gm.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cy.bjjhwx.cn

================================================================================
来源：http://pk.shxzukj.cn

A. 基础语法与类型
来源：http://lk.wgjwhj.cn

================================================================================
来源：http://qo.nszjky.cn

[A01] Hello World
来源：http://mp.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://wu.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://dr.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://jw.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qq.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://fs.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://kb.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://am.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tf.9csxet.cn

[A02] 变量声明与赋值
来源：http://lr.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kk.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rs.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bw.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kc.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://co.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://su.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://uc.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bi.shxzskj.cn

[A03] 常量定义
来源：http://ad.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pm.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://dr.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://je.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://sw.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://vu.szxytkj.cn

Go:   const PI = 3.14159
来源：http://sa.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://vy.521024.cn

C#:   const double PI = 3.14159;
来源：http://on.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://qo.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mj.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sw.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ol.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://tr.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mc.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://by.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bx.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://hx.yuexingan06.cn

[A05] 整数除法与取模
来源：http://wu.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nv.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ar.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lb.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ww.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://nd.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://jw.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://tw.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://bs.lnxyls.cn

[A06] 字符串转数字
来源：http://fa.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://ay.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mg.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gz.shtwfgs.cn


<!-- 参考信息 -->