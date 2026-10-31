代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://he.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ps.colortex.cn

[U40] Py：打印到标准错误
来源：http://li.asd995.cn

print("err", file=sys.stderr)
来源：http://rl.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ok.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nn.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://zy.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jl.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://ey.hnjuh.cn

namespace App\Http;
来源：http://da.newstarts.cn

[U44] PHP：开启严格类型
来源：http://tm.colortex.cn

declare(strict_types=1);
来源：http://pa.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://et.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bz.panjiajie.cn

[U46] PHP：可空类型
来源：http://qv.asd995.cn

?string $name = null
来源：http://nh.jctech888.com.cn

[U47] PHP：联合类型
来源：http://qo.bookmarksfly.cn

int|string $id
来源：http://av.shxzukj.cn

[U48] PHP：纯枚举
来源：http://ex.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xi.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://kd.gzmigu.cn

public readonly string $name
来源：http://oz.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://ro.colortex.cn

public function __construct(private int $id) {}
来源：http://eo.bjjhwx.cn

[U51] PHP：数组解构
来源：http://lf.haigaiapp.cn

[$a, $b] = $arr;
来源：http://ny.huanxung.cn

[U52] PHP：箭头函数
来源：http://ix.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://xw.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://ca.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://su.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://ex.shxzukj.cn

$obj?->method()
来源：http://lp.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ov.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ch.gzmigu.cn

[U56] PHP：命名参数
来源：http://ag.szxytkj.cn

f(a: 1, b: 2)
来源：http://ud.colortex.cn

[U57] PHP：字符串插值
来源：http://ix.yuexingan06.cn

"值: {$a}"
来源：http://cs.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://qe.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ba.gzmigu.cn

[U59] PHP：自定义排序
来源：http://oa.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qg.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://iu.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bw.521024.cn

[U61] PHP：正则
来源：http://mw.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nb.szsharing.cn

[U62] PHP：日期对象
来源：http://qo.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qq.shxzukj.cn

[U63] PHP：文件读写
来源：http://do.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xh.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://gj.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://bm.yuntaijiaju.cn

[U65] PHP：会话
来源：http://kq.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://np.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://uu.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cb.hahajie.cn

[U67] PHP：处理文件上传
来源：http://pd.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nw.newstarts.cn

[U68] PHP：PDO 连接
来源：http://uv.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ne.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://zy.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://io.nszjky.cn

[U70] PHP：PDO 事务
来源：http://cu.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dd.asd995.cn

[U71] PHP：抛出异常
来源：http://kg.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://pz.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://qg.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://bh.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://aj.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://gb.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://st.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://re.shxzskj.cn

[U75] PHP：依赖注入
来源：http://mk.gzmigu.cn

composer require psr/container
来源：http://kf.hahajie.cn

[U76] PHP：简单路由
来源：http://qm.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qy.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://ub.lnxyls.cn

composer require twig/twig
来源：http://nf.jctech888.com.cn

[U78] PHP：单元测试
来源：http://hk.asd995.cn

composer require --dev phpunit/phpunit
来源：http://mz.521024.cn

[U79] PHP：静态分析
来源：http://qq.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://le.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://ux.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vm.newstarts.cn

[U81] JS：初始化项目
来源：http://uo.nicolike.cn

npm init -y;  npm i express
来源：http://xq.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://oz.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fj.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://yp.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hs.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://eh.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tp.nicolike.cn

[U85] JS：可选链
来源：http://oe.bjjhwx.cn

a?.b?.c
来源：http://sx.huixiangedu.cn

[U86] JS：空值合并
来源：http://ew.shxzskj.cn

a ?? b
来源：http://qv.wgjwhj.cn

[U87] JS：解构默认值
来源：http://xz.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://je.9csxet.cn

[U88] JS：对象展开合并
来源：http://gv.bookmarksfly.cn

{ ...a, ...b }
来源：http://qc.hnjuh.cn

[U89] JS：数组去重
来源：http://ad.bookmarksfly.cn

[...new Set(arr)]
来源：http://ho.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://pc.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://eq.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://mc.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tm.szxytkj.cn

[U92] JS：深拷贝
来源：http://ic.hahajie.cn

structuredClone(obj)
来源：http://go.9csxet.cn

[U93] JS：模板字符串
来源：http://et.yuexingan06.cn

`共 ${n} 条`
来源：http://nk.huixiangedu.cn

[U94] JS：箭头函数
来源：http://yf.521024.cn

const double = x => x * 2;
来源：http://zd.hahajie.cn

[U95] JS：Promise 包装
来源：http://mn.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://kx.nicolike.cn

[U96] JS：async/await 与异常
来源：http://gs.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sw.shxzskj.cn

[U97] JS：并发请求
来源：http://cc.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uh.521024.cn

[U98] JS：fetch 带 JSON
来源：http://yx.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xu.szsharing.cn

[U99] JS：事件监听
来源：http://va.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://tk.szsharing.cn

[U100] JS：DOM 查询
来源：http://ao.asd995.cn

document.querySelector(".item")
来源：http://ec.colortex.cn

[U101] JS：classList 操作
来源：http://cz.shxzukj.cn

el.classList.toggle("active")
来源：http://zm.shxzukj.cn

[U102] JS：本地存储
来源：http://tf.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rh.szsharing.cn

[U103] JS：定时器
来源：http://yp.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oz.szxytkj.cn

[U104] JS：防抖
来源：http://xw.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fz.bjjhwx.cn

[U105] JS：节流
来源：http://bn.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ly.asd995.cn

[U106] JS：日期格式化
来源：http://lk.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hi.521024.cn

[U107] JS：数字千分位
来源：http://pe.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xc.szxytkj.cn

[U108] JS：随机整数
来源：http://ps.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ik.nicolike.cn

[U109] JS：数组分组
来源：http://ff.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://ue.szsharing.cn

[U110] JS：数组分块
来源：http://ru.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zs.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://il.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://bp.bjjhwx.cn

[U112] JS：字符串补位
来源：http://dj.lnxyls.cn

"7".padStart(3, "0")
来源：http://ij.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://mx.shxzukj.cn

s.replaceAll("a", "b")
来源：http://bh.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://hu.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nc.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ob.shxzskj.cn

crypto.randomUUID()
来源：http://zv.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://an.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://fa.szsharing.cn

[U117] JS：单元测试
来源：http://cj.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://iq.521024.cn

[U118] JS：开发服务器
来源：http://fs.huanxung.cn

npm i -D vite;  npx vite
来源：http://mv.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://jz.huixiangedu.cn

npx vite build
来源：http://tg.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://qo.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://kl.chemitech.net.cn

================================================================================
来源：http://ow.nicolike.cn

统计汇总
来源：http://il.szsharing.cn

================================================================================
来源：http://hp.asd995.cn

按语言统计（条）：
来源：http://rq.szsharing.cn

Python ......... 252
来源：http://lh.shxzskj.cn

PHP ............ 252
来源：http://cw.yuntaijiaju.cn

JavaScript ..... 252
来源：http://gw.chemitech.net.cn

TypeScript ..... 212
来源：http://aa.asd995.cn

Java ........... 212
来源：http://bh.hnjuh.cn

Go ............. 212
来源：http://bi.shxzskj.cn

Ruby ........... 212
来源：http://rz.huixiangedu.cn

C# ............. 212
来源：http://yw.huixiangedu.cn

C .............. 30
来源：http://iy.yuntaijiaju.cn

C++ ............ 30
来源：http://rk.szxytkj.cn

SQL ............ 90
来源：http://bq.9csxet.cn

Bash ........... 80
来源：http://sm.hahajie.cn

Kotlin ......... 15
来源：http://sy.newstarts.cn

Swift .......... 15
来源：http://zg.szxytkj.cn

Lua ............ 10
来源：http://qd.huanxung.cn

Perl ........... 10
来源：http://cz.chemitech.net.cn

Scala .......... 10
来源：http://yr.haigaiapp.cn

------------------------------------
来源：http://ab.hnjuh.cn

合计 ........... 2106 条
来源：http://pa.nszjky.cn

按章节统计：
来源：http://ol.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qu.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xv.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kp.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ux.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ry.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nw.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rb.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gq.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sx.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://my.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sa.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jl.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://io.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yr.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ur.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ik.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://hi.huanxung.cn

R Bash 专题                             80
来源：http://sg.lnxyls.cn

S C / C++ 专题                          60
来源：http://yl.chemitech.net.cn

T 其他语言补充                          60
来源：http://pe.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://qf.yuexingan06.cn

------------------------------------
来源：http://ix.chemitech.net.cn

合计                                  2106 条
来源：http://mb.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://zi.huanxung.cn

使用提醒
来源：http://ls.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://bq.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kb.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zm.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gg.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xv.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fo.huixiangedu.cn

—— 文件结束 ——
来源：http://vv.shxzukj.cn

================================================================================
来源：http://pv.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://zd.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://fz.wgjwhj.cn

================================================================================
来源：http://pm.yuntaijiaju.cn

【收录内容】
来源：http://tr.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://in.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ok.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://jd.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wl.colortex.cn

【使用说明】
来源：http://ic.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vq.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ca.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hy.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dv.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://th.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hk.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nz.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pz.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ar.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pz.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://my.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mt.bookmarksfly.cn

【文件统计】
来源：http://qv.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xq.hahajie.cn

--------------------------------------------------------------------------------
来源：http://oy.newstarts.cn

目  录
来源：http://zi.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://gu.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cp.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://st.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qs.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sn.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wa.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kt.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aw.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ur.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xd.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ov.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mj.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eh.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nk.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ml.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rh.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dk.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gn.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cp.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qy.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xf.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vi.colortex.cn

================================================================================
来源：http://in.bookmarksfly.cn

A. 基础语法与类型
来源：http://my.asd995.cn

================================================================================
来源：http://ee.szxytkj.cn

[A01] Hello World
来源：http://an.asd995.cn

Py:   print("Hello, World!")
来源：http://mr.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://nc.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://zx.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wr.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://yv.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://ly.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://df.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ko.hnjuh.cn

[A02] 变量声明与赋值
来源：http://di.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xv.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zx.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ui.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sn.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://qb.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ec.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://hz.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nm.hnjuh.cn

[A03] 常量定义
来源：http://nh.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fj.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://no.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://hm.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://jb.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://vr.nszjky.cn

Go:   const PI = 3.14159
来源：http://zu.9csxet.cn

Ruby: PI = 3.14159
来源：http://kg.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://rh.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://sp.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wp.szsharing.cn


<!-- 参考信息 -->