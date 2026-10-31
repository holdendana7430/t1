代发 wailian999

[U25] Py：CSV 按字典读
来源：http://no.yuntaijiaju.cn

csv.DictReader(f)
来源：http://lg.jctech888.com.cn

[U26] Py：并发下载
来源：http://th.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tl.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://lh.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://sf.nszjky.cn

[U28] Py：类型别名
来源：http://qh.huixiangedu.cn

UserId = int
来源：http://nu.newstarts.cn

[U29] Py：属性校验
来源：http://ff.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://ci.hahajie.cn

[U30] Py：数据类
来源：http://gv.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://lw.wgjwhj.cn

[U31] Py：单测
来源：http://dr.hnjuh.cn

python -m pytest -q
来源：http://hy.asd995.cn

[U32] Py：代码格式化
来源：http://sh.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://hw.huixiangedu.cn

[U33] Py：打包发布
来源：http://bb.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://lj.bjjhwx.cn

[U34] Py：判断编码
来源：http://pn.shxzskj.cn

chardet.detect(raw)
来源：http://xo.huixiangedu.cn

[U35] Py：发送邮件
来源：http://qk.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dq.bjjhwx.cn

[U36] Py：定时任务
来源：http://ca.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://kw.panjiajie.cn

[U37] Py：读写 Excel
来源：http://kf.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vi.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://sb.nicolike.cn

Path(__file__).resolve().parent
来源：http://tp.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://qa.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://ok.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://xo.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://wd.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://sj.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rl.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://jb.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ny.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://vm.huixinmuqiang.cn

namespace App\Http;
来源：http://rr.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://ar.huixinmuqiang.cn

declare(strict_types=1);
来源：http://nn.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://lq.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gh.haigaiapp.cn

[U46] PHP：可空类型
来源：http://yq.hnjuh.cn

?string $name = null
来源：http://pe.panjiajie.cn

[U47] PHP：联合类型
来源：http://xx.haigaiapp.cn

int|string $id
来源：http://lw.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://mu.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tb.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://bc.bjjhwx.cn

public readonly string $name
来源：http://gi.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://vr.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://zw.colortex.cn

[U51] PHP：数组解构
来源：http://gs.muxihuayi.cn

[$a, $b] = $arr;
来源：http://oo.colortex.cn

[U52] PHP：箭头函数
来源：http://zy.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://cb.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://dz.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://id.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://jn.jianghongdianzi.cn

$obj?->method()
来源：http://hu.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ow.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cc.asd995.cn

[U56] PHP：命名参数
来源：http://ig.muxihuayi.cn

f(a: 1, b: 2)
来源：http://ab.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://uh.muxihuayi.cn

"值: {$a}"
来源：http://ko.hnjuh.cn

[U58] PHP：数组三件套
来源：http://lx.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ti.shxzukj.cn

[U59] PHP：自定义排序
来源：http://pf.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://av.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://ev.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qv.shxzukj.cn

[U61] PHP：正则
来源：http://jb.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uk.muxihuayi.cn

[U62] PHP：日期对象
来源：http://rb.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qv.9csxet.cn

[U63] PHP：文件读写
来源：http://pk.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vu.panjiajie.cn

[U64] PHP：目录遍历
来源：http://rc.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://sf.haigaiapp.cn

[U65] PHP：会话
来源：http://vq.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sf.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://jp.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vr.nicolike.cn

[U67] PHP：处理文件上传
来源：http://de.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://um.521024.cn

[U68] PHP：PDO 连接
来源：http://ra.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dm.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://md.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ja.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ru.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mz.521024.cn

[U71] PHP：抛出异常
来源：http://wz.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://lo.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://jl.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://dk.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://de.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://lp.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://pb.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://hn.nszjky.cn

[U75] PHP：依赖注入
来源：http://rs.gzmigu.cn

composer require psr/container
来源：http://do.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://af.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ix.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://gb.newstarts.cn

composer require twig/twig
来源：http://br.huanxung.cn

[U78] PHP：单元测试
来源：http://kw.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://fb.muxihuayi.cn

[U79] PHP：静态分析
来源：http://kn.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://qs.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://xi.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hq.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://cq.hahajie.cn

npm init -y;  npm i express
来源：http://cf.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://an.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://si.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://tf.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yo.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://cz.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://df.nszjky.cn

[U85] JS：可选链
来源：http://ui.panjiajie.cn

a?.b?.c
来源：http://qe.chemitech.net.cn

[U86] JS：空值合并
来源：http://eq.hahajie.cn

a ?? b
来源：http://tx.szsharing.cn

[U87] JS：解构默认值
来源：http://tm.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://yp.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://wd.9csxet.cn

{ ...a, ...b }
来源：http://is.panjiajie.cn

[U89] JS：数组去重
来源：http://uk.yuexingan06.cn

[...new Set(arr)]
来源：http://cm.asd995.cn

[U90] JS：数字数组排序
来源：http://zt.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://sl.nicolike.cn

[U91] JS：对象键值遍历
来源：http://xu.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tk.szxytkj.cn

[U92] JS：深拷贝
来源：http://av.jctech888.com.cn

structuredClone(obj)
来源：http://io.lnxyls.cn

[U93] JS：模板字符串
来源：http://kk.szxytkj.cn

`共 ${n} 条`
来源：http://rr.hahajie.cn

[U94] JS：箭头函数
来源：http://rv.szxytkj.cn

const double = x => x * 2;
来源：http://kq.szxytkj.cn

[U95] JS：Promise 包装
来源：http://es.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://np.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://no.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uh.jctech888.com.cn

[U97] JS：并发请求
来源：http://ac.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://yp.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rj.hahajie.cn

[U99] JS：事件监听
来源：http://nq.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://qp.gzmigu.cn

[U100] JS：DOM 查询
来源：http://ah.hahajie.cn

document.querySelector(".item")
来源：http://qv.szsharing.cn

[U101] JS：classList 操作
来源：http://im.hnjuh.cn

el.classList.toggle("active")
来源：http://ln.hnjuh.cn

[U102] JS：本地存储
来源：http://ss.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fm.521024.cn

[U103] JS：定时器
来源：http://rp.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vt.nicolike.cn

[U104] JS：防抖
来源：http://cr.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ra.yuexingan06.cn

[U105] JS：节流
来源：http://ns.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zp.yuexingan06.cn

[U106] JS：日期格式化
来源：http://ts.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://re.muxihuayi.cn

[U107] JS：数字千分位
来源：http://oh.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sp.huixiangedu.cn

[U108] JS：随机整数
来源：http://xh.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kl.hnjuh.cn

[U109] JS：数组分组
来源：http://ng.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://rr.nszjky.cn

[U110] JS：数组分块
来源：http://ui.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://te.nicolike.cn

[U111] JS：对象转 Map
来源：http://gq.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://lp.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://to.panjiajie.cn

"7".padStart(3, "0")
来源：http://sw.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://fj.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://ln.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://qq.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ko.newstarts.cn

[U115] JS：生成 UUID
来源：http://sg.hnjuh.cn

crypto.randomUUID()
来源：http://ou.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://ng.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://ik.bookmarksfly.cn

[U117] JS：单元测试
来源：http://ql.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://hl.nszjky.cn

[U118] JS：开发服务器
来源：http://qv.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://fg.muxihuayi.cn

[U119] JS：生产构建
来源：http://bx.gzmigu.cn

npx vite build
来源：http://tx.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://vt.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://rs.huanxung.cn

================================================================================
来源：http://to.shxzukj.cn

统计汇总
来源：http://ye.yuntaijiaju.cn

================================================================================
来源：http://dq.jctech888.com.cn

按语言统计（条）：
来源：http://zl.gzmigu.cn

Python ......... 252
来源：http://sv.wgjwhj.cn

PHP ............ 252
来源：http://ei.shxzskj.cn

JavaScript ..... 252
来源：http://rm.hnjuh.cn

TypeScript ..... 212
来源：http://mi.yuexingan06.cn

Java ........... 212
来源：http://lp.nicolike.cn

Go ............. 212
来源：http://la.jianghongdianzi.cn

Ruby ........... 212
来源：http://tm.nicolike.cn

C# ............. 212
来源：http://bx.haigaiapp.cn

C .............. 30
来源：http://zb.bookmarksfly.cn

C++ ............ 30
来源：http://ww.colortex.cn

SQL ............ 90
来源：http://sl.panjiajie.cn

Bash ........... 80
来源：http://vy.hahajie.cn

Kotlin ......... 15
来源：http://hj.jianghongdianzi.cn

Swift .......... 15
来源：http://rn.muxihuayi.cn

Lua ............ 10
来源：http://ka.lnxyls.cn

Perl ........... 10
来源：http://co.9csxet.cn

Scala .......... 10
来源：http://vs.panjiajie.cn

------------------------------------
来源：http://xg.asd995.cn

合计 ........... 2106 条
来源：http://sd.hahajie.cn

按章节统计：
来源：http://sg.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sw.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ym.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uo.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lj.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gz.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zl.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ld.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xw.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pp.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://te.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ya.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rf.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vt.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zf.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nm.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kq.nszjky.cn

Q SQL 专题                              90
来源：http://mb.yuexingan06.cn

R Bash 专题                             80
来源：http://jk.9csxet.cn

S C / C++ 专题                          60
来源：http://ob.szsharing.cn

T 其他语言补充                          60
来源：http://le.colortex.cn

U 高频实用片段                         120
来源：http://gs.shxzskj.cn

------------------------------------
来源：http://qo.nszjky.cn

合计                                  2106 条
来源：http://qp.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://bs.shxzukj.cn

使用提醒
来源：http://zi.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://eb.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rt.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ih.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ks.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nb.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://so.bjjhwx.cn

—— 文件结束 ——
来源：http://sb.haigaiapp.cn

================================================================================
来源：http://ls.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://iz.nicolike.cn

Common Programming Examples Cheat Book
来源：http://zx.lnxyls.cn

================================================================================
来源：http://rr.muxihuayi.cn

【收录内容】
来源：http://fh.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yj.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zz.asd995.cn

SQL · Bash · C · C++
来源：http://tu.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ou.nszjky.cn

【使用说明】
来源：http://fz.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fh.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ny.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dl.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mc.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xz.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ec.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wc.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ee.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jx.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fy.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ie.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://me.yuexingan06.cn

【文件统计】
来源：http://nf.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ed.hahajie.cn

--------------------------------------------------------------------------------
来源：http://hw.shxzskj.cn

目  录
来源：http://ny.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ib.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hj.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ak.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mu.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ip.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oc.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bq.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://as.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cj.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wh.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yy.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nl.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zm.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qq.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cl.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zq.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hk.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wm.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pq.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qj.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bt.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pp.jctech888.com.cn

================================================================================
来源：http://zb.panjiajie.cn

A. 基础语法与类型
来源：http://gj.szxytkj.cn

================================================================================
来源：http://se.haigaiapp.cn

[A01] Hello World
来源：http://kb.9csxet.cn


<!-- 参考信息 -->