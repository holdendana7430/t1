代发 wailian999

[U29] Py：属性校验
来源：http://dx.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://ar.shxzskj.cn

[U30] Py：数据类
来源：http://mc.chemitech.net.cn

@dataclass(slots=True)
来源：http://fx.newstarts.cn

[U31] Py：单测
来源：http://io.yuntaijiaju.cn

python -m pytest -q
来源：http://cg.wgjwhj.cn

[U32] Py：代码格式化
来源：http://uo.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://rp.yuexingan06.cn

[U33] Py：打包发布
来源：http://ch.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ol.szsharing.cn

[U34] Py：判断编码
来源：http://im.huanxung.cn

chardet.detect(raw)
来源：http://pg.haigaiapp.cn

[U35] Py：发送邮件
来源：http://yh.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eq.wgjwhj.cn

[U36] Py：定时任务
来源：http://oo.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://wj.9csxet.cn

[U37] Py：读写 Excel
来源：http://pb.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xe.521024.cn

[U38] Py：获取脚本所在目录
来源：http://vy.gzmigu.cn

Path(__file__).resolve().parent
来源：http://fo.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://gd.nszjky.cn

sys.stdout.isatty()
来源：http://sk.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://al.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://ga.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://bu.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jx.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://ah.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wi.szsharing.cn

[U43] PHP：声明命名空间
来源：http://un.bjjhwx.cn

namespace App\Http;
来源：http://pn.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://rl.yuntaijiaju.cn

declare(strict_types=1);
来源：http://nn.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://ft.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nn.bjjhwx.cn

[U46] PHP：可空类型
来源：http://dv.yuexingan06.cn

?string $name = null
来源：http://bg.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://vj.jianghongdianzi.cn

int|string $id
来源：http://iv.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://qx.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ii.colortex.cn

[U49] PHP：只读属性
来源：http://wj.wgjwhj.cn

public readonly string $name
来源：http://mc.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://hq.asd995.cn

public function __construct(private int $id) {}
来源：http://dq.hahajie.cn

[U51] PHP：数组解构
来源：http://rc.lnxyls.cn

[$a, $b] = $arr;
来源：http://ah.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ss.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://th.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://ma.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://hr.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://bx.chemitech.net.cn

$obj?->method()
来源：http://cq.szsharing.cn

[U55] PHP：match 表达式
来源：http://rt.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nk.yuexingan06.cn

[U56] PHP：命名参数
来源：http://il.lnxyls.cn

f(a: 1, b: 2)
来源：http://zm.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://ey.newstarts.cn

"值: {$a}"
来源：http://ko.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://ir.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ex.nszjky.cn

[U59] PHP：自定义排序
来源：http://pg.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hn.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://va.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tt.huixinmuqiang.cn

[U61] PHP：正则
来源：http://bc.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ra.521024.cn

[U62] PHP：日期对象
来源：http://pu.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ie.hnjuh.cn

[U63] PHP：文件读写
来源：http://zw.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fo.asd995.cn

[U64] PHP：目录遍历
来源：http://bj.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://lb.bjjhwx.cn

[U65] PHP：会话
来源：http://rh.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ik.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://mn.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lv.asd995.cn

[U67] PHP：处理文件上传
来源：http://wr.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gv.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://wn.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oh.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://qg.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ti.nicolike.cn

[U70] PHP：PDO 事务
来源：http://pf.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://at.newstarts.cn

[U71] PHP：抛出异常
来源：http://bb.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://wm.szxytkj.cn

[U72] PHP：写错误日志
来源：http://rl.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://am.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://zv.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://hr.huanxung.cn

[U74] PHP：读取环境变量
来源：http://fw.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://qg.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ss.nicolike.cn

composer require psr/container
来源：http://cb.haigaiapp.cn

[U76] PHP：简单路由
来源：http://zz.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://px.jctech888.com.cn

composer require twig/twig
来源：http://mz.colortex.cn

[U78] PHP：单元测试
来源：http://xk.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://gu.panjiajie.cn

[U79] PHP：静态分析
来源：http://cv.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://dp.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://zg.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wx.nszjky.cn

[U81] JS：初始化项目
来源：http://bn.bjjhwx.cn

npm init -y;  npm i express
来源：http://ty.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://mh.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ct.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://ny.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ak.521024.cn

[U84] JS：CommonJS 写法
来源：http://nr.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ll.szsharing.cn

[U85] JS：可选链
来源：http://rj.bjjhwx.cn

a?.b?.c
来源：http://ih.muxihuayi.cn

[U86] JS：空值合并
来源：http://bc.szxytkj.cn

a ?? b
来源：http://na.nszjky.cn

[U87] JS：解构默认值
来源：http://tv.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://xy.521024.cn

[U88] JS：对象展开合并
来源：http://qg.chemitech.net.cn

{ ...a, ...b }
来源：http://ma.hahajie.cn

[U89] JS：数组去重
来源：http://xp.szsharing.cn

[...new Set(arr)]
来源：http://ej.szxytkj.cn

[U90] JS：数字数组排序
来源：http://to.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://vu.9csxet.cn

[U91] JS：对象键值遍历
来源：http://co.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cf.nicolike.cn

[U92] JS：深拷贝
来源：http://la.bjjhwx.cn

structuredClone(obj)
来源：http://bp.huanxung.cn

[U93] JS：模板字符串
来源：http://we.jianghongdianzi.cn

`共 ${n} 条`
来源：http://fn.bjjhwx.cn

[U94] JS：箭头函数
来源：http://lw.asd995.cn

const double = x => x * 2;
来源：http://ga.asd995.cn

[U95] JS：Promise 包装
来源：http://dg.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://mr.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://gn.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kz.gzmigu.cn

[U97] JS：并发请求
来源：http://ov.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qr.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://fy.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pt.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://mx.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://tg.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://mw.colortex.cn

document.querySelector(".item")
来源：http://qz.lnxyls.cn

[U101] JS：classList 操作
来源：http://eh.szxytkj.cn

el.classList.toggle("active")
来源：http://cg.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://ct.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ot.shxzskj.cn

[U103] JS：定时器
来源：http://lp.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ma.521024.cn

[U104] JS：防抖
来源：http://cf.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yo.jctech888.com.cn

[U105] JS：节流
来源：http://hi.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ns.wgjwhj.cn

[U106] JS：日期格式化
来源：http://sr.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://um.jctech888.com.cn

[U107] JS：数字千分位
来源：http://hx.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iv.szsharing.cn

[U108] JS：随机整数
来源：http://do.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://al.szsharing.cn

[U109] JS：数组分组
来源：http://we.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://uh.nszjky.cn

[U110] JS：数组分块
来源：http://aq.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dq.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://yh.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://po.wgjwhj.cn

[U112] JS：字符串补位
来源：http://kh.shxzskj.cn

"7".padStart(3, "0")
来源：http://lj.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://zl.9csxet.cn

s.replaceAll("a", "b")
来源：http://bp.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://ys.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wr.9csxet.cn

[U115] JS：生成 UUID
来源：http://xm.huixiangedu.cn

crypto.randomUUID()
来源：http://bz.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://vy.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://am.shtwfgs.cn

[U117] JS：单元测试
来源：http://qe.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://ji.gzmigu.cn

[U118] JS：开发服务器
来源：http://wp.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://rh.panjiajie.cn

[U119] JS：生产构建
来源：http://ax.9csxet.cn

npx vite build
来源：http://xo.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://aj.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://ey.yuntaijiaju.cn

================================================================================
来源：http://oc.bjjhwx.cn

统计汇总
来源：http://xr.hahajie.cn

================================================================================
来源：http://ny.bjjhwx.cn

按语言统计（条）：
来源：http://fm.yuntaijiaju.cn

Python ......... 252
来源：http://ln.yuntaijiaju.cn

PHP ............ 252
来源：http://hc.huixinmuqiang.cn

JavaScript ..... 252
来源：http://wk.jianghongdianzi.cn

TypeScript ..... 212
来源：http://dh.bjjhwx.cn

Java ........... 212
来源：http://uh.newstarts.cn

Go ............. 212
来源：http://ee.hnjuh.cn

Ruby ........... 212
来源：http://fk.panjiajie.cn

C# ............. 212
来源：http://df.huixinmuqiang.cn

C .............. 30
来源：http://wz.huanxung.cn

C++ ............ 30
来源：http://xj.lnxyls.cn

SQL ............ 90
来源：http://ez.bookmarksfly.cn

Bash ........... 80
来源：http://vf.shxzskj.cn

Kotlin ......... 15
来源：http://os.shtwfgs.cn

Swift .......... 15
来源：http://uy.shxzskj.cn

Lua ............ 10
来源：http://me.huixiangedu.cn

Perl ........... 10
来源：http://uh.panjiajie.cn

Scala .......... 10
来源：http://tn.szsharing.cn

------------------------------------
来源：http://ba.nszjky.cn

合计 ........... 2106 条
来源：http://do.gzmigu.cn

按章节统计：
来源：http://qm.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vs.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tf.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cd.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mo.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://io.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ru.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sj.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hh.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ir.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yz.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ou.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sn.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://in.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tu.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nd.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mw.hahajie.cn

Q SQL 专题                              90
来源：http://gw.nszjky.cn

R Bash 专题                             80
来源：http://lw.szxytkj.cn

S C / C++ 专题                          60
来源：http://ef.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://sc.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://cm.panjiajie.cn

------------------------------------
来源：http://zq.huixiangedu.cn

合计                                  2106 条
来源：http://eq.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://hn.haigaiapp.cn

使用提醒
来源：http://tw.9csxet.cn

--------------------------------------------------------------------------------
来源：http://tt.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://um.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ov.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kv.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ya.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nq.haigaiapp.cn

—— 文件结束 ——
来源：http://il.colortex.cn

================================================================================
来源：http://oe.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://bn.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://on.yuntaijiaju.cn

================================================================================
来源：http://ou.asd995.cn

【收录内容】
来源：http://nb.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qr.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nv.szxytkj.cn

SQL · Bash · C · C++
来源：http://gs.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://or.panjiajie.cn

【使用说明】
来源：http://cu.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gc.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qp.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dt.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bt.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xu.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wu.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fs.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ht.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uz.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://co.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yw.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vz.szsharing.cn

【文件统计】
来源：http://ki.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fu.nicolike.cn

--------------------------------------------------------------------------------
来源：http://vt.newstarts.cn

目  录
来源：http://sh.521024.cn

--------------------------------------------------------------------------------
来源：http://ei.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://of.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zp.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://az.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://td.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mz.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://me.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wj.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qm.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://um.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oc.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://et.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ki.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tt.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wi.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rk.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uj.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pb.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cp.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lw.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lh.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fw.asd995.cn

================================================================================
来源：http://pn.shxzskj.cn

A. 基础语法与类型
来源：http://yu.yuexingan06.cn

================================================================================
来源：http://pe.bookmarksfly.cn

[A01] Hello World
来源：http://fc.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://xc.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://mh.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://ft.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tp.521024.cn

Java: System.out.println("Hello, World!");
来源：http://xh.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://vu.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://ck.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zd.shxzskj.cn


<!-- 参考信息 -->