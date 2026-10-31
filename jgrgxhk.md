代发 wailian999

[U31] Py：单测
来源：http://fi.panjiajie.cn

python -m pytest -q
来源：http://yu.9csxet.cn

[U32] Py：代码格式化
来源：http://gp.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://ip.colortex.cn

[U33] Py：打包发布
来源：http://el.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://co.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://rh.gzmigu.cn

chardet.detect(raw)
来源：http://ij.wgjwhj.cn

[U35] Py：发送邮件
来源：http://wv.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xu.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://ab.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://yt.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://we.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rv.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://qp.521024.cn

Path(__file__).resolve().parent
来源：http://rh.521024.cn

[U39] Py：判断是否在交互环境
来源：http://je.9csxet.cn

sys.stdout.isatty()
来源：http://xt.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://iv.szxytkj.cn

print("err", file=sys.stderr)
来源：http://my.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://iq.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://di.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://zh.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ws.huanxung.cn

[U43] PHP：声明命名空间
来源：http://kn.panjiajie.cn

namespace App\Http;
来源：http://gn.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://fa.wgjwhj.cn

declare(strict_types=1);
来源：http://sm.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://wl.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ud.9csxet.cn

[U46] PHP：可空类型
来源：http://wu.wgjwhj.cn

?string $name = null
来源：http://ya.521024.cn

[U47] PHP：联合类型
来源：http://mw.newstarts.cn

int|string $id
来源：http://rj.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://pf.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://as.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ut.nszjky.cn

public readonly string $name
来源：http://yy.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ii.colortex.cn

public function __construct(private int $id) {}
来源：http://kf.asd995.cn

[U51] PHP：数组解构
来源：http://wt.nszjky.cn

[$a, $b] = $arr;
来源：http://xg.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://jj.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://fy.9csxet.cn

[U53] PHP：空合并运算符
来源：http://qq.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://bp.szsharing.cn

[U54] PHP：空安全调用
来源：http://mt.lnxyls.cn

$obj?->method()
来源：http://wf.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://rk.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://me.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://yo.asd995.cn

f(a: 1, b: 2)
来源：http://kk.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://ar.shtwfgs.cn

"值: {$a}"
来源：http://aq.lnxyls.cn

[U58] PHP：数组三件套
来源：http://mv.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gx.shxzukj.cn

[U59] PHP：自定义排序
来源：http://sg.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ol.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://uz.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uo.wgjwhj.cn

[U61] PHP：正则
来源：http://cb.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cf.9csxet.cn

[U62] PHP：日期对象
来源：http://av.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cq.jctech888.com.cn

[U63] PHP：文件读写
来源：http://jj.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qs.szsharing.cn

[U64] PHP：目录遍历
来源：http://xe.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://wk.bookmarksfly.cn

[U65] PHP：会话
来源：http://sn.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oa.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://ml.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jx.newstarts.cn

[U67] PHP：处理文件上传
来源：http://vn.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://py.9csxet.cn

[U68] PHP：PDO 连接
来源：http://ve.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xt.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://ae.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://is.asd995.cn

[U70] PHP：PDO 事务
来源：http://xy.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kv.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://cx.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://fh.nszjky.cn

[U72] PHP：写错误日志
来源：http://gp.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://en.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://lg.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://oe.huanxung.cn

[U74] PHP：读取环境变量
来源：http://hs.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://gs.lnxyls.cn

[U75] PHP：依赖注入
来源：http://ed.jianghongdianzi.cn

composer require psr/container
来源：http://id.gzmigu.cn

[U76] PHP：简单路由
来源：http://ag.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zm.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://rx.yuntaijiaju.cn

composer require twig/twig
来源：http://er.szxytkj.cn

[U78] PHP：单元测试
来源：http://fb.asd995.cn

composer require --dev phpunit/phpunit
来源：http://on.huixiangedu.cn

[U79] PHP：静态分析
来源：http://ct.colortex.cn

composer require --dev phpstan/phpstan
来源：http://jq.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://fv.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://io.nicolike.cn

[U81] JS：初始化项目
来源：http://ho.newstarts.cn

npm init -y;  npm i express
来源：http://vv.colortex.cn

[U82] JS：package.json 脚本
来源：http://xg.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sb.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ya.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gw.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://po.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vu.nicolike.cn

[U85] JS：可选链
来源：http://eo.huixiangedu.cn

a?.b?.c
来源：http://yn.szxytkj.cn

[U86] JS：空值合并
来源：http://mm.asd995.cn

a ?? b
来源：http://ev.521024.cn

[U87] JS：解构默认值
来源：http://ue.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://pu.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://mr.haigaiapp.cn

{ ...a, ...b }
来源：http://cf.chemitech.net.cn

[U89] JS：数组去重
来源：http://is.shxzskj.cn

[...new Set(arr)]
来源：http://nn.szsharing.cn

[U90] JS：数字数组排序
来源：http://fc.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://fe.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://yg.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qh.asd995.cn

[U92] JS：深拷贝
来源：http://cs.huanxung.cn

structuredClone(obj)
来源：http://np.hnjuh.cn

[U93] JS：模板字符串
来源：http://tz.521024.cn

`共 ${n} 条`
来源：http://ef.szxytkj.cn

[U94] JS：箭头函数
来源：http://qq.szsharing.cn

const double = x => x * 2;
来源：http://dh.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://lf.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://gv.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://op.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sb.bookmarksfly.cn

[U97] JS：并发请求
来源：http://dy.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vx.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://lc.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kv.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://pd.huanxung.cn

el.addEventListener("click", e => {})
来源：http://qz.panjiajie.cn

[U100] JS：DOM 查询
来源：http://fc.lnxyls.cn

document.querySelector(".item")
来源：http://ht.haigaiapp.cn

[U101] JS：classList 操作
来源：http://ya.muxihuayi.cn

el.classList.toggle("active")
来源：http://fn.szxytkj.cn

[U102] JS：本地存储
来源：http://bm.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ar.szsharing.cn

[U103] JS：定时器
来源：http://ts.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mo.szxytkj.cn

[U104] JS：防抖
来源：http://hj.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sn.jctech888.com.cn

[U105] JS：节流
来源：http://wo.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ci.huanxung.cn

[U106] JS：日期格式化
来源：http://za.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vk.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://ec.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xk.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://wd.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qc.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://qy.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://gt.bookmarksfly.cn

[U110] JS：数组分块
来源：http://pf.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ry.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://tf.9csxet.cn

new Map(Object.entries(obj))
来源：http://qd.szxytkj.cn

[U112] JS：字符串补位
来源：http://ey.shtwfgs.cn

"7".padStart(3, "0")
来源：http://jo.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ak.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://lx.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://bg.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rl.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://ad.haigaiapp.cn

crypto.randomUUID()
来源：http://ig.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://th.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://au.szxytkj.cn

[U117] JS：单元测试
来源：http://iy.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://wb.521024.cn

[U118] JS：开发服务器
来源：http://fd.nszjky.cn

npm i -D vite;  npx vite
来源：http://yn.panjiajie.cn

[U119] JS：生产构建
来源：http://ew.shxzukj.cn

npx vite build
来源：http://xr.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://vf.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://iz.gzmigu.cn

================================================================================
来源：http://fh.asd995.cn

统计汇总
来源：http://gl.asd995.cn

================================================================================
来源：http://ra.chemitech.net.cn

按语言统计（条）：
来源：http://zn.hahajie.cn

Python ......... 252
来源：http://qb.colortex.cn

PHP ............ 252
来源：http://yp.shtwfgs.cn

JavaScript ..... 252
来源：http://ep.bookmarksfly.cn

TypeScript ..... 212
来源：http://cy.wgjwhj.cn

Java ........... 212
来源：http://no.szsharing.cn

Go ............. 212
来源：http://hp.muxihuayi.cn

Ruby ........... 212
来源：http://cq.huanxung.cn

C# ............. 212
来源：http://wr.huixinmuqiang.cn

C .............. 30
来源：http://he.521024.cn

C++ ............ 30
来源：http://zw.jctech888.com.cn

SQL ............ 90
来源：http://gr.wgjwhj.cn

Bash ........... 80
来源：http://up.shtwfgs.cn

Kotlin ......... 15
来源：http://xf.huixinmuqiang.cn

Swift .......... 15
来源：http://hp.szsharing.cn

Lua ............ 10
来源：http://cd.jianghongdianzi.cn

Perl ........... 10
来源：http://gz.haigaiapp.cn

Scala .......... 10
来源：http://tl.lnxyls.cn

------------------------------------
来源：http://pi.wgjwhj.cn

合计 ........... 2106 条
来源：http://ez.panjiajie.cn

按章节统计：
来源：http://ei.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ze.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oz.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aa.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://as.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tn.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ev.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bb.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rq.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ik.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oc.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xc.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tu.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yb.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://km.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yc.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bw.nszjky.cn

Q SQL 专题                              90
来源：http://yb.nicolike.cn

R Bash 专题                             80
来源：http://tf.chemitech.net.cn

S C / C++ 专题                          60
来源：http://qn.lnxyls.cn

T 其他语言补充                          60
来源：http://up.shtwfgs.cn

U 高频实用片段                         120
来源：http://wg.szsharing.cn

------------------------------------
来源：http://qj.asd995.cn

合计                                  2106 条
来源：http://hw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://op.muxihuayi.cn

使用提醒
来源：http://mc.szsharing.cn

--------------------------------------------------------------------------------
来源：http://yw.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yx.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://im.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mr.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vb.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xi.gzmigu.cn

—— 文件结束 ——
来源：http://cs.shxzukj.cn

================================================================================
来源：http://gn.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ue.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://te.muxihuayi.cn

================================================================================
来源：http://oo.yuexingan06.cn

【收录内容】
来源：http://ln.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bi.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nu.shtwfgs.cn

SQL · Bash · C · C++
来源：http://hv.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tp.shxzskj.cn

【使用说明】
来源：http://nw.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mm.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ql.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hs.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ml.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zb.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://au.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hg.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rk.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fq.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jj.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dp.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tp.haigaiapp.cn

【文件统计】
来源：http://sl.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lv.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://kr.huixinmuqiang.cn

目  录
来源：http://zr.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ua.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://va.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iz.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xs.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nm.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pz.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xf.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sq.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wo.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qm.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hr.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mi.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wa.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dq.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jv.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cf.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ad.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xq.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yp.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://et.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ry.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hv.gzmigu.cn

================================================================================
来源：http://pj.bookmarksfly.cn

A. 基础语法与类型
来源：http://by.hahajie.cn

================================================================================
来源：http://ud.nszjky.cn

[A01] Hello World
来源：http://lb.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://bm.asd995.cn

PHP:  echo "Hello, World!";
来源：http://bu.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://xk.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qt.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://oz.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://yc.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://ci.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://du.shxzskj.cn

[A02] 变量声明与赋值
来源：http://dc.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pz.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://em.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qp.nicolike.cn


<!-- 参考信息 -->