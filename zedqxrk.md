代发 wailian999

[U29] Py：属性校验
来源：http://qe.521024.cn

@property 与 @x.setter 配合
来源：http://op.asd995.cn

[U30] Py：数据类
来源：http://ni.lnxyls.cn

@dataclass(slots=True)
来源：http://ao.jctech888.com.cn

[U31] Py：单测
来源：http://vy.huixinmuqiang.cn

python -m pytest -q
来源：http://bg.wgjwhj.cn

[U32] Py：代码格式化
来源：http://tf.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://cl.lnxyls.cn

[U33] Py：打包发布
来源：http://zl.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://ar.muxihuayi.cn

[U34] Py：判断编码
来源：http://vw.hnjuh.cn

chardet.detect(raw)
来源：http://xv.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://mw.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qd.shxzukj.cn

[U36] Py：定时任务
来源：http://qs.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://ws.panjiajie.cn

[U37] Py：读写 Excel
来源：http://ro.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qs.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://og.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://dk.521024.cn

[U39] Py：判断是否在交互环境
来源：http://lf.shtwfgs.cn

sys.stdout.isatty()
来源：http://ka.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://nd.hnjuh.cn

print("err", file=sys.stderr)
来源：http://lv.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://pf.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://av.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://jt.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kv.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://jm.wgjwhj.cn

namespace App\Http;
来源：http://lg.nszjky.cn

[U44] PHP：开启严格类型
来源：http://du.nszjky.cn

declare(strict_types=1);
来源：http://bn.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://pm.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fr.szxytkj.cn

[U46] PHP：可空类型
来源：http://zo.colortex.cn

?string $name = null
来源：http://ku.shtwfgs.cn

[U47] PHP：联合类型
来源：http://aj.panjiajie.cn

int|string $id
来源：http://lx.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://bm.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rq.asd995.cn

[U49] PHP：只读属性
来源：http://nj.jianghongdianzi.cn

public readonly string $name
来源：http://qc.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://cl.nszjky.cn

public function __construct(private int $id) {}
来源：http://aq.hnjuh.cn

[U51] PHP：数组解构
来源：http://kt.shtwfgs.cn

[$a, $b] = $arr;
来源：http://my.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://fh.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://wq.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://he.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://ij.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://dk.szxytkj.cn

$obj?->method()
来源：http://cq.hahajie.cn

[U55] PHP：match 表达式
来源：http://sd.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qg.wgjwhj.cn

[U56] PHP：命名参数
来源：http://sw.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://la.nicolike.cn

[U57] PHP：字符串插值
来源：http://xe.huanxung.cn

"值: {$a}"
来源：http://un.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://rl.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gd.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://wi.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ev.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://qz.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ga.yuexingan06.cn

[U61] PHP：正则
来源：http://ki.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qg.szsharing.cn

[U62] PHP：日期对象
来源：http://tw.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xn.jctech888.com.cn

[U63] PHP：文件读写
来源：http://ow.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ri.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://an.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://jz.huixinmuqiang.cn

[U65] PHP：会话
来源：http://fm.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cp.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://hh.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ox.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://nm.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yz.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://uq.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ew.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://hi.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sn.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://he.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vs.szxytkj.cn

[U71] PHP：抛出异常
来源：http://bp.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://ge.shxzskj.cn

[U72] PHP：写错误日志
来源：http://tk.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://fp.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://lv.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://wy.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://bn.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://gz.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://tj.yuntaijiaju.cn

composer require psr/container
来源：http://wm.hnjuh.cn

[U76] PHP：简单路由
来源：http://ov.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xc.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ld.shxzskj.cn

composer require twig/twig
来源：http://yg.chemitech.net.cn

[U78] PHP：单元测试
来源：http://ds.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://ra.shxzskj.cn

[U79] PHP：静态分析
来源：http://ug.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://yf.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://sn.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oz.shxzukj.cn

[U81] JS：初始化项目
来源：http://fw.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://ud.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://tw.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lp.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://bj.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dm.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://ue.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lf.9csxet.cn

[U85] JS：可选链
来源：http://sl.nszjky.cn

a?.b?.c
来源：http://oz.wgjwhj.cn

[U86] JS：空值合并
来源：http://ur.521024.cn

a ?? b
来源：http://nq.huanxung.cn

[U87] JS：解构默认值
来源：http://wj.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://fj.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://td.jctech888.com.cn

{ ...a, ...b }
来源：http://ve.szsharing.cn

[U89] JS：数组去重
来源：http://yz.muxihuayi.cn

[...new Set(arr)]
来源：http://sb.nicolike.cn

[U90] JS：数字数组排序
来源：http://qe.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://ts.asd995.cn

[U91] JS：对象键值遍历
来源：http://cy.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hm.shxzskj.cn

[U92] JS：深拷贝
来源：http://zt.huixiangedu.cn

structuredClone(obj)
来源：http://cm.jctech888.com.cn

[U93] JS：模板字符串
来源：http://md.newstarts.cn

`共 ${n} 条`
来源：http://lp.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://pm.huixiangedu.cn

const double = x => x * 2;
来源：http://cd.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://ul.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://tq.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://uj.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cy.jctech888.com.cn

[U97] JS：并发请求
来源：http://yk.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ks.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://lr.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qk.shxzukj.cn

[U99] JS：事件监听
来源：http://eh.nszjky.cn

el.addEventListener("click", e => {})
来源：http://zv.colortex.cn

[U100] JS：DOM 查询
来源：http://wv.shxzukj.cn

document.querySelector(".item")
来源：http://cj.chemitech.net.cn

[U101] JS：classList 操作
来源：http://yo.szsharing.cn

el.classList.toggle("active")
来源：http://ep.szsharing.cn

[U102] JS：本地存储
来源：http://vh.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://en.asd995.cn

[U103] JS：定时器
来源：http://nh.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ye.lnxyls.cn

[U104] JS：防抖
来源：http://iz.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zp.huanxung.cn

[U105] JS：节流
来源：http://sz.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kr.panjiajie.cn

[U106] JS：日期格式化
来源：http://xs.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gq.jctech888.com.cn

[U107] JS：数字千分位
来源：http://iq.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ib.szxytkj.cn

[U108] JS：随机整数
来源：http://jm.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wt.panjiajie.cn

[U109] JS：数组分组
来源：http://qy.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://ow.shtwfgs.cn

[U110] JS：数组分块
来源：http://rt.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yf.lnxyls.cn

[U111] JS：对象转 Map
来源：http://vu.panjiajie.cn

new Map(Object.entries(obj))
来源：http://qd.lnxyls.cn

[U112] JS：字符串补位
来源：http://rk.panjiajie.cn

"7".padStart(3, "0")
来源：http://jb.hnjuh.cn

[U113] JS：正则替换全部
来源：http://pg.szxytkj.cn

s.replaceAll("a", "b")
来源：http://po.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://lg.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://im.nszjky.cn

[U115] JS：生成 UUID
来源：http://sy.huixiangedu.cn

crypto.randomUUID()
来源：http://ih.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://hf.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://yg.yuexingan06.cn

[U117] JS：单元测试
来源：http://mm.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://wm.szxytkj.cn

[U118] JS：开发服务器
来源：http://ri.nicolike.cn

npm i -D vite;  npx vite
来源：http://vq.yuexingan06.cn

[U119] JS：生产构建
来源：http://wp.bookmarksfly.cn

npx vite build
来源：http://oq.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://jq.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://cb.wgjwhj.cn

================================================================================
来源：http://ub.hahajie.cn

统计汇总
来源：http://vb.jctech888.com.cn

================================================================================
来源：http://vb.huixinmuqiang.cn

按语言统计（条）：
来源：http://rw.hahajie.cn

Python ......... 252
来源：http://dl.jianghongdianzi.cn

PHP ............ 252
来源：http://th.yuexingan06.cn

JavaScript ..... 252
来源：http://aw.haigaiapp.cn

TypeScript ..... 212
来源：http://gx.panjiajie.cn

Java ........... 212
来源：http://vw.lnxyls.cn

Go ............. 212
来源：http://cu.huanxung.cn

Ruby ........... 212
来源：http://vx.newstarts.cn

C# ............. 212
来源：http://od.shxzukj.cn

C .............. 30
来源：http://sp.szxytkj.cn

C++ ............ 30
来源：http://zf.huixinmuqiang.cn

SQL ............ 90
来源：http://rw.chemitech.net.cn

Bash ........... 80
来源：http://uv.chemitech.net.cn

Kotlin ......... 15
来源：http://vs.shxzskj.cn

Swift .......... 15
来源：http://be.huanxung.cn

Lua ............ 10
来源：http://qc.szsharing.cn

Perl ........... 10
来源：http://kf.szsharing.cn

Scala .......... 10
来源：http://tv.hahajie.cn

------------------------------------
来源：http://vf.panjiajie.cn

合计 ........... 2106 条
来源：http://he.hahajie.cn

按章节统计：
来源：http://cd.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zm.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cb.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://es.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ny.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wy.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sd.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://to.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jg.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://va.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hn.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dw.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vj.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ps.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iz.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zo.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xr.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://mw.yuntaijiaju.cn

R Bash 专题                             80
来源：http://fi.nicolike.cn

S C / C++ 专题                          60
来源：http://qy.hnjuh.cn

T 其他语言补充                          60
来源：http://xm.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://sw.shxzskj.cn

------------------------------------
来源：http://sa.bookmarksfly.cn

合计                                  2106 条
来源：http://wy.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ou.gzmigu.cn

使用提醒
来源：http://qz.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://rt.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wb.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ug.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sw.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vx.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bs.shtwfgs.cn

—— 文件结束 ——
来源：http://pv.nicolike.cn

================================================================================
来源：http://bp.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://nw.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://vr.haigaiapp.cn

================================================================================
来源：http://co.newstarts.cn

【收录内容】
来源：http://mh.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mn.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sx.521024.cn

SQL · Bash · C · C++
来源：http://bj.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kk.wgjwhj.cn

【使用说明】
来源：http://xe.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wf.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://el.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sj.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://br.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rz.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uu.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vr.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://by.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://af.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ox.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yt.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ni.huanxung.cn

【文件统计】
来源：http://cf.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zj.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ow.huanxung.cn

目  录
来源：http://di.9csxet.cn

--------------------------------------------------------------------------------
来源：http://hs.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dz.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vm.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zf.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://we.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yd.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hq.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lf.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cb.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kh.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qu.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zp.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pp.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ov.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rc.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lb.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fd.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nq.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xz.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fk.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tr.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dn.nicolike.cn

================================================================================
来源：http://gu.shxzukj.cn

A. 基础语法与类型
来源：http://ke.huixinmuqiang.cn

================================================================================
来源：http://lw.bookmarksfly.cn

[A01] Hello World
来源：http://qi.9csxet.cn

Py:   print("Hello, World!")
来源：http://sc.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://ff.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://tm.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ph.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://bh.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://oh.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://ef.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nu.jctech888.com.cn


<!-- 参考信息 -->