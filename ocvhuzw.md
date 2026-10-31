代发 wailian999

[U33] Py：打包发布
来源：http://ur.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://gf.shxzskj.cn

[U34] Py：判断编码
来源：http://zf.szxytkj.cn

chardet.detect(raw)
来源：http://rb.wgjwhj.cn

[U35] Py：发送邮件
来源：http://dl.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gz.huanxung.cn

[U36] Py：定时任务
来源：http://fh.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://su.newstarts.cn

[U37] Py：读写 Excel
来源：http://wq.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hi.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://vv.newstarts.cn

Path(__file__).resolve().parent
来源：http://bt.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://kd.hahajie.cn

sys.stdout.isatty()
来源：http://bb.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://kd.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://jq.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://ad.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yd.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://mr.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iq.szsharing.cn

[U43] PHP：声明命名空间
来源：http://xu.huanxung.cn

namespace App\Http;
来源：http://lx.szsharing.cn

[U44] PHP：开启严格类型
来源：http://lo.bjjhwx.cn

declare(strict_types=1);
来源：http://qd.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://ux.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zv.yuexingan06.cn

[U46] PHP：可空类型
来源：http://jy.szxytkj.cn

?string $name = null
来源：http://mw.muxihuayi.cn

[U47] PHP：联合类型
来源：http://bp.9csxet.cn

int|string $id
来源：http://fj.shxzukj.cn

[U48] PHP：纯枚举
来源：http://wu.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ou.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://br.huanxung.cn

public readonly string $name
来源：http://ny.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://gk.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://xj.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://lv.shxzukj.cn

[$a, $b] = $arr;
来源：http://ef.szxytkj.cn

[U52] PHP：箭头函数
来源：http://ol.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://xt.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://bj.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://gd.huanxung.cn

[U54] PHP：空安全调用
来源：http://ns.muxihuayi.cn

$obj?->method()
来源：http://sx.shxzskj.cn

[U55] PHP：match 表达式
来源：http://rd.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cx.yuexingan06.cn

[U56] PHP：命名参数
来源：http://zp.9csxet.cn

f(a: 1, b: 2)
来源：http://uv.hnjuh.cn

[U57] PHP：字符串插值
来源：http://br.newstarts.cn

"值: {$a}"
来源：http://vv.shxzukj.cn

[U58] PHP：数组三件套
来源：http://mg.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xn.9csxet.cn

[U59] PHP：自定义排序
来源：http://ni.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tt.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://tg.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xy.wgjwhj.cn

[U61] PHP：正则
来源：http://wp.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xv.colortex.cn

[U62] PHP：日期对象
来源：http://hu.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ne.bjjhwx.cn

[U63] PHP：文件读写
来源：http://vh.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dr.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://jk.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://oy.hahajie.cn

[U65] PHP：会话
来源：http://vz.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://co.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://lq.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wp.newstarts.cn

[U67] PHP：处理文件上传
来源：http://cp.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ki.nicolike.cn

[U68] PHP：PDO 连接
来源：http://mg.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mg.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://dh.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bt.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://cf.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qv.521024.cn

[U71] PHP：抛出异常
来源：http://oq.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://rj.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://ed.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://cf.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://ci.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://er.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://sl.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://ok.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://yf.huixinmuqiang.cn

composer require psr/container
来源：http://qk.panjiajie.cn

[U76] PHP：简单路由
来源：http://yp.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vr.gzmigu.cn

[U77] PHP：模板渲染
来源：http://iw.nicolike.cn

composer require twig/twig
来源：http://tm.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://jk.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://tt.wgjwhj.cn

[U79] PHP：静态分析
来源：http://mn.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://rr.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ys.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mb.nicolike.cn

[U81] JS：初始化项目
来源：http://wf.bjjhwx.cn

npm init -y;  npm i express
来源：http://ud.nicolike.cn

[U82] JS：package.json 脚本
来源：http://vv.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mu.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://em.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vs.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://fp.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bw.huixiangedu.cn

[U85] JS：可选链
来源：http://nc.yuntaijiaju.cn

a?.b?.c
来源：http://as.szsharing.cn

[U86] JS：空值合并
来源：http://hs.wgjwhj.cn

a ?? b
来源：http://tm.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://nj.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://lf.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://ak.hahajie.cn

{ ...a, ...b }
来源：http://ll.hnjuh.cn

[U89] JS：数组去重
来源：http://tu.asd995.cn

[...new Set(arr)]
来源：http://ie.9csxet.cn

[U90] JS：数字数组排序
来源：http://ro.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://uh.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://gp.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ww.chemitech.net.cn

[U92] JS：深拷贝
来源：http://ll.shxzskj.cn

structuredClone(obj)
来源：http://hk.newstarts.cn

[U93] JS：模板字符串
来源：http://lw.yuexingan06.cn

`共 ${n} 条`
来源：http://yl.nszjky.cn

[U94] JS：箭头函数
来源：http://wa.panjiajie.cn

const double = x => x * 2;
来源：http://aq.newstarts.cn

[U95] JS：Promise 包装
来源：http://uh.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://zx.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://zc.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://go.shxzskj.cn

[U97] JS：并发请求
来源：http://vi.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zx.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://sb.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ow.szxytkj.cn

[U99] JS：事件监听
来源：http://so.521024.cn

el.addEventListener("click", e => {})
来源：http://bz.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://ck.nicolike.cn

document.querySelector(".item")
来源：http://id.asd995.cn

[U101] JS：classList 操作
来源：http://hk.hnjuh.cn

el.classList.toggle("active")
来源：http://et.jctech888.com.cn

[U102] JS：本地存储
来源：http://do.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ga.wgjwhj.cn

[U103] JS：定时器
来源：http://rn.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zl.wgjwhj.cn

[U104] JS：防抖
来源：http://mo.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lx.wgjwhj.cn

[U105] JS：节流
来源：http://ga.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fs.nicolike.cn

[U106] JS：日期格式化
来源：http://ba.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uv.muxihuayi.cn

[U107] JS：数字千分位
来源：http://kx.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nt.gzmigu.cn

[U108] JS：随机整数
来源：http://na.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://si.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://ud.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://by.haigaiapp.cn

[U110] JS：数组分块
来源：http://rw.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ln.521024.cn

[U111] JS：对象转 Map
来源：http://jk.9csxet.cn

new Map(Object.entries(obj))
来源：http://om.521024.cn

[U112] JS：字符串补位
来源：http://ji.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://kb.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://ue.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://ec.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://nd.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dn.shxzskj.cn

[U115] JS：生成 UUID
来源：http://an.szxytkj.cn

crypto.randomUUID()
来源：http://cu.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://yk.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://hz.panjiajie.cn

[U117] JS：单元测试
来源：http://qz.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://kc.wgjwhj.cn

[U118] JS：开发服务器
来源：http://fw.szxytkj.cn

npm i -D vite;  npx vite
来源：http://hy.szxytkj.cn

[U119] JS：生产构建
来源：http://xj.9csxet.cn

npx vite build
来源：http://qn.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://il.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://tc.bookmarksfly.cn

================================================================================
来源：http://pm.gzmigu.cn

统计汇总
来源：http://qd.yuexingan06.cn

================================================================================
来源：http://pz.shxzukj.cn

按语言统计（条）：
来源：http://sw.hahajie.cn

Python ......... 252
来源：http://ru.huanxung.cn

PHP ............ 252
来源：http://wr.bookmarksfly.cn

JavaScript ..... 252
来源：http://lp.jianghongdianzi.cn

TypeScript ..... 212
来源：http://qf.colortex.cn

Java ........... 212
来源：http://rg.9csxet.cn

Go ............. 212
来源：http://ct.huixiangedu.cn

Ruby ........... 212
来源：http://jv.nicolike.cn

C# ............. 212
来源：http://rj.huixiangedu.cn

C .............. 30
来源：http://jl.bjjhwx.cn

C++ ............ 30
来源：http://py.chemitech.net.cn

SQL ............ 90
来源：http://pc.jianghongdianzi.cn

Bash ........... 80
来源：http://rj.9csxet.cn

Kotlin ......... 15
来源：http://ms.newstarts.cn

Swift .......... 15
来源：http://ql.shxzskj.cn

Lua ............ 10
来源：http://ja.asd995.cn

Perl ........... 10
来源：http://ib.shxzskj.cn

Scala .......... 10
来源：http://cq.nszjky.cn

------------------------------------
来源：http://zn.hahajie.cn

合计 ........... 2106 条
来源：http://px.bookmarksfly.cn

按章节统计：
来源：http://nk.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kd.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jh.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ax.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ip.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bi.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iv.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://md.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://if.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ec.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kw.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wn.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zi.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dz.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ex.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ez.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kb.muxihuayi.cn

Q SQL 专题                              90
来源：http://lu.szsharing.cn

R Bash 专题                             80
来源：http://ns.huanxung.cn

S C / C++ 专题                          60
来源：http://tj.hahajie.cn

T 其他语言补充                          60
来源：http://kn.bjjhwx.cn

U 高频实用片段                         120
来源：http://hz.lnxyls.cn

------------------------------------
来源：http://is.bjjhwx.cn

合计                                  2106 条
来源：http://ox.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://lz.lnxyls.cn

使用提醒
来源：http://ly.huanxung.cn

--------------------------------------------------------------------------------
来源：http://fu.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://em.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mr.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tm.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wa.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lk.huixiangedu.cn

—— 文件结束 ——
来源：http://ez.lnxyls.cn

================================================================================
来源：http://ti.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ui.hahajie.cn

Common Programming Examples Cheat Book
来源：http://tu.lnxyls.cn

================================================================================
来源：http://ed.newstarts.cn

【收录内容】
来源：http://wb.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sg.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cg.huixiangedu.cn

SQL · Bash · C · C++
来源：http://zr.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pk.panjiajie.cn

【使用说明】
来源：http://cn.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hv.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ti.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://is.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ig.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cx.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ep.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tw.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gh.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oe.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mg.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fi.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bf.hahajie.cn

【文件统计】
来源：http://hp.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ym.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://md.bookmarksfly.cn

目  录
来源：http://om.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://pg.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pk.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ft.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fs.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vy.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tq.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ou.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xz.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ch.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ay.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fl.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hw.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zq.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jw.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oy.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xf.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uo.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hj.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jb.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ap.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jw.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tl.szsharing.cn

================================================================================
来源：http://gg.asd995.cn

A. 基础语法与类型
来源：http://ix.asd995.cn

================================================================================
来源：http://zl.huixinmuqiang.cn

[A01] Hello World
来源：http://wh.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://hn.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://vf.asd995.cn

JS:   console.log("Hello, World!");
来源：http://hs.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pj.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://ty.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://ph.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://zi.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wn.szxytkj.cn

[A02] 变量声明与赋值
来源：http://pl.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://id.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dz.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hd.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ku.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://dh.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://qz.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://bl.hnjuh.cn


<!-- 参考信息 -->