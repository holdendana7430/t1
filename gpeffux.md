代发 wailian999

[U25] Py：CSV 按字典读
来源：http://pb.chemitech.net.cn

csv.DictReader(f)
来源：http://je.jctech888.com.cn

[U26] Py：并发下载
来源：http://iz.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gu.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://ww.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://sx.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://pt.shxzskj.cn

UserId = int
来源：http://to.szxytkj.cn

[U29] Py：属性校验
来源：http://re.9csxet.cn

@property 与 @x.setter 配合
来源：http://qr.shxzskj.cn

[U30] Py：数据类
来源：http://pt.shxzukj.cn

@dataclass(slots=True)
来源：http://eo.hahajie.cn

[U31] Py：单测
来源：http://tk.521024.cn

python -m pytest -q
来源：http://oa.shxzukj.cn

[U32] Py：代码格式化
来源：http://nw.huanxung.cn

ruff format . && ruff check --fix .
来源：http://is.521024.cn

[U33] Py：打包发布
来源：http://ap.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://sr.gzmigu.cn

[U34] Py：判断编码
来源：http://bm.muxihuayi.cn

chardet.detect(raw)
来源：http://cf.panjiajie.cn

[U35] Py：发送邮件
来源：http://wd.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ho.haigaiapp.cn

[U36] Py：定时任务
来源：http://gy.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://rf.gzmigu.cn

[U37] Py：读写 Excel
来源：http://km.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fp.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://kf.colortex.cn

Path(__file__).resolve().parent
来源：http://qk.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://xz.huixiangedu.cn

sys.stdout.isatty()
来源：http://ut.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ep.huanxung.cn

print("err", file=sys.stderr)
来源：http://pv.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://ir.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lo.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://he.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ur.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://fa.huanxung.cn

namespace App\Http;
来源：http://uh.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://pg.bjjhwx.cn

declare(strict_types=1);
来源：http://yh.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://wp.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yu.hnjuh.cn

[U46] PHP：可空类型
来源：http://gt.yuexingan06.cn

?string $name = null
来源：http://ba.nicolike.cn

[U47] PHP：联合类型
来源：http://fp.shxzukj.cn

int|string $id
来源：http://vl.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://iu.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tl.panjiajie.cn

[U49] PHP：只读属性
来源：http://ub.yuntaijiaju.cn

public readonly string $name
来源：http://li.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://cp.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://sa.9csxet.cn

[U51] PHP：数组解构
来源：http://xr.asd995.cn

[$a, $b] = $arr;
来源：http://hx.hnjuh.cn

[U52] PHP：箭头函数
来源：http://cf.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://hi.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://hj.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://vi.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://lm.panjiajie.cn

$obj?->method()
来源：http://ej.lnxyls.cn

[U55] PHP：match 表达式
来源：http://mo.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://la.szxytkj.cn

[U56] PHP：命名参数
来源：http://tn.gzmigu.cn

f(a: 1, b: 2)
来源：http://jl.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://jy.hahajie.cn

"值: {$a}"
来源：http://uz.gzmigu.cn

[U58] PHP：数组三件套
来源：http://pc.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dz.nicolike.cn

[U59] PHP：自定义排序
来源：http://cl.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yi.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://zh.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cv.shxzukj.cn

[U61] PHP：正则
来源：http://vv.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wq.shxzskj.cn

[U62] PHP：日期对象
来源：http://hm.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bh.haigaiapp.cn

[U63] PHP：文件读写
来源：http://uw.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oe.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ud.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://bk.hnjuh.cn

[U65] PHP：会话
来源：http://qs.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kj.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://tz.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vw.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://zc.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hu.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://hj.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ey.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://lq.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bi.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://je.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ui.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://fj.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://nc.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://of.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://jg.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://jw.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://hf.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ne.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://xm.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://gr.shxzukj.cn

composer require psr/container
来源：http://gj.asd995.cn

[U76] PHP：简单路由
来源：http://hi.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xs.gzmigu.cn

[U77] PHP：模板渲染
来源：http://xp.muxihuayi.cn

composer require twig/twig
来源：http://ck.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://ik.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://sj.szxytkj.cn

[U79] PHP：静态分析
来源：http://oq.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://ud.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://my.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vq.wgjwhj.cn

[U81] JS：初始化项目
来源：http://tm.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://qe.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://lu.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hl.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://rm.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jc.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://xq.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ys.shxzskj.cn

[U85] JS：可选链
来源：http://ye.shtwfgs.cn

a?.b?.c
来源：http://fi.newstarts.cn

[U86] JS：空值合并
来源：http://nf.hnjuh.cn

a ?? b
来源：http://du.yuexingan06.cn

[U87] JS：解构默认值
来源：http://ec.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://zy.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://eu.panjiajie.cn

{ ...a, ...b }
来源：http://uj.hahajie.cn

[U89] JS：数组去重
来源：http://hm.nszjky.cn

[...new Set(arr)]
来源：http://sq.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://vw.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://bp.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://rd.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ch.newstarts.cn

[U92] JS：深拷贝
来源：http://ex.hnjuh.cn

structuredClone(obj)
来源：http://kf.hnjuh.cn

[U93] JS：模板字符串
来源：http://ui.bjjhwx.cn

`共 ${n} 条`
来源：http://in.521024.cn

[U94] JS：箭头函数
来源：http://cs.bjjhwx.cn

const double = x => x * 2;
来源：http://mn.panjiajie.cn

[U95] JS：Promise 包装
来源：http://lp.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://eb.521024.cn

[U96] JS：async/await 与异常
来源：http://zm.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vu.nicolike.cn

[U97] JS：并发请求
来源：http://rs.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bn.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://un.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hd.bjjhwx.cn

[U99] JS：事件监听
来源：http://gv.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://jn.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://tj.wgjwhj.cn

document.querySelector(".item")
来源：http://na.jctech888.com.cn

[U101] JS：classList 操作
来源：http://aj.chemitech.net.cn

el.classList.toggle("active")
来源：http://et.szsharing.cn

[U102] JS：本地存储
来源：http://sb.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rq.muxihuayi.cn

[U103] JS：定时器
来源：http://uq.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kw.muxihuayi.cn

[U104] JS：防抖
来源：http://ui.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wa.jianghongdianzi.cn

[U105] JS：节流
来源：http://hz.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ks.lnxyls.cn

[U106] JS：日期格式化
来源：http://zw.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uw.shxzukj.cn

[U107] JS：数字千分位
来源：http://mj.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jh.jctech888.com.cn

[U108] JS：随机整数
来源：http://qv.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zf.colortex.cn

[U109] JS：数组分组
来源：http://vo.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://vn.gzmigu.cn

[U110] JS：数组分块
来源：http://dh.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://su.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://sx.hahajie.cn

new Map(Object.entries(obj))
来源：http://oc.wgjwhj.cn

[U112] JS：字符串补位
来源：http://vy.szxytkj.cn

"7".padStart(3, "0")
来源：http://eu.szxytkj.cn

[U113] JS：正则替换全部
来源：http://gs.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://hm.9csxet.cn

[U114] JS：JSON 深比较
来源：http://lz.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ts.shxzukj.cn

[U115] JS：生成 UUID
来源：http://oc.wgjwhj.cn

crypto.randomUUID()
来源：http://uc.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tz.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://de.newstarts.cn

[U117] JS：单元测试
来源：http://om.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://rw.wgjwhj.cn

[U118] JS：开发服务器
来源：http://jo.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://tt.nicolike.cn

[U119] JS：生产构建
来源：http://qt.szsharing.cn

npx vite build
来源：http://wy.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://zp.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://vt.yuexingan06.cn

================================================================================
来源：http://ac.colortex.cn

统计汇总
来源：http://gz.gzmigu.cn

================================================================================
来源：http://hq.gzmigu.cn

按语言统计（条）：
来源：http://ye.chemitech.net.cn

Python ......... 252
来源：http://lo.nicolike.cn

PHP ............ 252
来源：http://vp.nicolike.cn

JavaScript ..... 252
来源：http://ew.huanxung.cn

TypeScript ..... 212
来源：http://gk.bjjhwx.cn

Java ........... 212
来源：http://ip.jianghongdianzi.cn

Go ............. 212
来源：http://fj.nszjky.cn

Ruby ........... 212
来源：http://sj.szxytkj.cn

C# ............. 212
来源：http://nf.yuexingan06.cn

C .............. 30
来源：http://gm.gzmigu.cn

C++ ............ 30
来源：http://eu.gzmigu.cn

SQL ............ 90
来源：http://op.521024.cn

Bash ........... 80
来源：http://ih.haigaiapp.cn

Kotlin ......... 15
来源：http://zh.nszjky.cn

Swift .......... 15
来源：http://ks.shtwfgs.cn

Lua ............ 10
来源：http://cq.chemitech.net.cn

Perl ........... 10
来源：http://rb.asd995.cn

Scala .......... 10
来源：http://fs.yuexingan06.cn

------------------------------------
来源：http://uw.muxihuayi.cn

合计 ........... 2106 条
来源：http://cv.lnxyls.cn

按章节统计：
来源：http://en.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gd.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nd.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xa.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dq.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gm.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ch.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ie.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xf.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xz.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qx.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uq.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sh.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vc.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pi.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hw.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xh.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://kh.huixinmuqiang.cn

R Bash 专题                             80
来源：http://wm.hahajie.cn

S C / C++ 专题                          60
来源：http://bm.yuexingan06.cn

T 其他语言补充                          60
来源：http://if.nszjky.cn

U 高频实用片段                         120
来源：http://jf.bookmarksfly.cn

------------------------------------
来源：http://bj.shxzskj.cn

合计                                  2106 条
来源：http://vo.521024.cn

--------------------------------------------------------------------------------
来源：http://gb.newstarts.cn

使用提醒
来源：http://yk.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://wg.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yr.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vb.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tc.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nd.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rh.nszjky.cn

—— 文件结束 ——
来源：http://gd.521024.cn

================================================================================
来源：http://yk.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ny.hahajie.cn

Common Programming Examples Cheat Book
来源：http://sb.chemitech.net.cn

================================================================================
来源：http://yo.521024.cn

【收录内容】
来源：http://gd.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nk.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uw.panjiajie.cn

SQL · Bash · C · C++
来源：http://ks.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rt.gzmigu.cn

【使用说明】
来源：http://es.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xn.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uh.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ir.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qr.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jp.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xl.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://js.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dd.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nz.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lj.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xe.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yp.huixiangedu.cn

【文件统计】
来源：http://vm.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://na.521024.cn

--------------------------------------------------------------------------------
来源：http://kg.newstarts.cn

目  录
来源：http://dy.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://tc.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zq.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://we.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ft.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zi.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hb.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hi.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iu.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ks.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cn.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://if.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hw.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gu.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tj.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nu.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zg.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yo.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sa.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sq.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ls.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ss.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rk.muxihuayi.cn

================================================================================
来源：http://oq.huanxung.cn

A. 基础语法与类型
来源：http://sa.521024.cn

================================================================================
来源：http://ss.colortex.cn

[A01] Hello World
来源：http://ho.9csxet.cn


<!-- 参考信息 -->