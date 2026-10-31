代发 wailian999

[U29] Py：属性校验
来源：http://mn.shxzskj.cn

@property 与 @x.setter 配合
来源：http://cb.bookmarksfly.cn

[U30] Py：数据类
来源：http://gk.lnxyls.cn

@dataclass(slots=True)
来源：http://jf.9csxet.cn

[U31] Py：单测
来源：http://rm.chemitech.net.cn

python -m pytest -q
来源：http://ry.shxzskj.cn

[U32] Py：代码格式化
来源：http://rt.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://vr.bjjhwx.cn

[U33] Py：打包发布
来源：http://zm.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://cg.newstarts.cn

[U34] Py：判断编码
来源：http://ul.asd995.cn

chardet.detect(raw)
来源：http://dt.huanxung.cn

[U35] Py：发送邮件
来源：http://bw.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gd.panjiajie.cn

[U36] Py：定时任务
来源：http://kh.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://ho.shxzskj.cn

[U37] Py：读写 Excel
来源：http://ma.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jp.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://np.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://zp.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://xr.panjiajie.cn

sys.stdout.isatty()
来源：http://xa.colortex.cn

[U40] Py：打印到标准错误
来源：http://xl.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://aj.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://ai.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jg.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://ur.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://st.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://xk.bjjhwx.cn

namespace App\Http;
来源：http://uv.huanxung.cn

[U44] PHP：开启严格类型
来源：http://en.asd995.cn

declare(strict_types=1);
来源：http://gu.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://am.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://av.gzmigu.cn

[U46] PHP：可空类型
来源：http://tj.asd995.cn

?string $name = null
来源：http://ku.newstarts.cn

[U47] PHP：联合类型
来源：http://hj.huixiangedu.cn

int|string $id
来源：http://ua.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://tk.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hs.haigaiapp.cn

[U49] PHP：只读属性
来源：http://sz.bjjhwx.cn

public readonly string $name
来源：http://ag.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://fd.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ic.nszjky.cn

[U51] PHP：数组解构
来源：http://fh.lnxyls.cn

[$a, $b] = $arr;
来源：http://lw.hahajie.cn

[U52] PHP：箭头函数
来源：http://ai.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://nb.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://zs.521024.cn

$v = $a ?? $b ?? "default";
来源：http://be.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://nb.shtwfgs.cn

$obj?->method()
来源：http://cr.nszjky.cn

[U55] PHP：match 表达式
来源：http://oc.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mx.wgjwhj.cn

[U56] PHP：命名参数
来源：http://dg.muxihuayi.cn

f(a: 1, b: 2)
来源：http://fp.huanxung.cn

[U57] PHP：字符串插值
来源：http://je.wgjwhj.cn

"值: {$a}"
来源：http://qu.asd995.cn

[U58] PHP：数组三件套
来源：http://df.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ot.huanxung.cn

[U59] PHP：自定义排序
来源：http://mc.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://py.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://qn.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ac.huixinmuqiang.cn

[U61] PHP：正则
来源：http://sd.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ky.chemitech.net.cn

[U62] PHP：日期对象
来源：http://vp.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wf.asd995.cn

[U63] PHP：文件读写
来源：http://ti.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zr.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://jr.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://ye.gzmigu.cn

[U65] PHP：会话
来源：http://kb.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jz.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://ri.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://td.hahajie.cn

[U67] PHP：处理文件上传
来源：http://kg.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ak.szsharing.cn

[U68] PHP：PDO 连接
来源：http://qb.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gj.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://ss.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uu.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://oq.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gb.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://ud.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://wq.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://yc.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://qb.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://mz.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://kq.nszjky.cn

[U74] PHP：读取环境变量
来源：http://ra.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://vs.colortex.cn

[U75] PHP：依赖注入
来源：http://wc.nicolike.cn

composer require psr/container
来源：http://hb.newstarts.cn

[U76] PHP：简单路由
来源：http://xz.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://er.nicolike.cn

[U77] PHP：模板渲染
来源：http://zr.haigaiapp.cn

composer require twig/twig
来源：http://mn.asd995.cn

[U78] PHP：单元测试
来源：http://wd.521024.cn

composer require --dev phpunit/phpunit
来源：http://ha.shxzskj.cn

[U79] PHP：静态分析
来源：http://fw.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://qp.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://sk.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ex.szxytkj.cn

[U81] JS：初始化项目
来源：http://mp.bookmarksfly.cn

npm init -y;  npm i express
来源：http://im.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://be.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tj.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://um.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lq.521024.cn

[U84] JS：CommonJS 写法
来源：http://wi.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gh.huixinmuqiang.cn

[U85] JS：可选链
来源：http://wx.chemitech.net.cn

a?.b?.c
来源：http://zs.hahajie.cn

[U86] JS：空值合并
来源：http://sc.shtwfgs.cn

a ?? b
来源：http://zf.muxihuayi.cn

[U87] JS：解构默认值
来源：http://mi.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://jl.huanxung.cn

[U88] JS：对象展开合并
来源：http://hy.bookmarksfly.cn

{ ...a, ...b }
来源：http://vy.bjjhwx.cn

[U89] JS：数组去重
来源：http://kw.newstarts.cn

[...new Set(arr)]
来源：http://ax.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://by.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://zn.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://lg.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ra.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://zl.nszjky.cn

structuredClone(obj)
来源：http://ih.panjiajie.cn

[U93] JS：模板字符串
来源：http://ho.yuexingan06.cn

`共 ${n} 条`
来源：http://vo.panjiajie.cn

[U94] JS：箭头函数
来源：http://il.shxzskj.cn

const double = x => x * 2;
来源：http://fz.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://mb.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://ac.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ci.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://me.wgjwhj.cn

[U97] JS：并发请求
来源：http://iz.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zu.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://ol.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vz.shtwfgs.cn

[U99] JS：事件监听
来源：http://pf.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://kx.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://lu.9csxet.cn

document.querySelector(".item")
来源：http://cn.colortex.cn

[U101] JS：classList 操作
来源：http://vl.521024.cn

el.classList.toggle("active")
来源：http://vt.yuexingan06.cn

[U102] JS：本地存储
来源：http://yv.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fm.nicolike.cn

[U103] JS：定时器
来源：http://py.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oi.521024.cn

[U104] JS：防抖
来源：http://bp.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zi.nicolike.cn

[U105] JS：节流
来源：http://ol.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://in.hahajie.cn

[U106] JS：日期格式化
来源：http://rl.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ek.lnxyls.cn

[U107] JS：数字千分位
来源：http://ue.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kx.wgjwhj.cn

[U108] JS：随机整数
来源：http://ja.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qu.nszjky.cn

[U109] JS：数组分组
来源：http://ag.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://cn.chemitech.net.cn

[U110] JS：数组分块
来源：http://mt.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://to.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://us.lnxyls.cn

new Map(Object.entries(obj))
来源：http://dx.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://wz.hnjuh.cn

"7".padStart(3, "0")
来源：http://le.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://al.gzmigu.cn

s.replaceAll("a", "b")
来源：http://co.szsharing.cn

[U114] JS：JSON 深比较
来源：http://gp.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qr.nicolike.cn

[U115] JS：生成 UUID
来源：http://wr.huixinmuqiang.cn

crypto.randomUUID()
来源：http://ah.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://ir.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://rc.9csxet.cn

[U117] JS：单元测试
来源：http://bq.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ua.yuexingan06.cn

[U118] JS：开发服务器
来源：http://ew.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://zr.szxytkj.cn

[U119] JS：生产构建
来源：http://fn.bjjhwx.cn

npx vite build
来源：http://jd.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://nv.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://sw.yuexingan06.cn

================================================================================
来源：http://ef.bjjhwx.cn

统计汇总
来源：http://zf.asd995.cn

================================================================================
来源：http://ke.bookmarksfly.cn

按语言统计（条）：
来源：http://st.huixinmuqiang.cn

Python ......... 252
来源：http://bp.yuntaijiaju.cn

PHP ............ 252
来源：http://ir.panjiajie.cn

JavaScript ..... 252
来源：http://wf.lnxyls.cn

TypeScript ..... 212
来源：http://ao.jctech888.com.cn

Java ........... 212
来源：http://zx.panjiajie.cn

Go ............. 212
来源：http://rl.bookmarksfly.cn

Ruby ........... 212
来源：http://rm.521024.cn

C# ............. 212
来源：http://hv.nszjky.cn

C .............. 30
来源：http://ai.lnxyls.cn

C++ ............ 30
来源：http://gt.nszjky.cn

SQL ............ 90
来源：http://ft.yuntaijiaju.cn

Bash ........... 80
来源：http://rk.bookmarksfly.cn

Kotlin ......... 15
来源：http://jy.shxzukj.cn

Swift .......... 15
来源：http://ql.9csxet.cn

Lua ............ 10
来源：http://gf.yuntaijiaju.cn

Perl ........... 10
来源：http://ua.shtwfgs.cn

Scala .......... 10
来源：http://gg.huixiangedu.cn

------------------------------------
来源：http://nq.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://yx.nszjky.cn

按章节统计：
来源：http://ni.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tc.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aj.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://im.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vr.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ni.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lc.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xr.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://os.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lg.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bn.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lm.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dr.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bq.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://in.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yl.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yz.gzmigu.cn

Q SQL 专题                              90
来源：http://ey.yuexingan06.cn

R Bash 专题                             80
来源：http://uf.lnxyls.cn

S C / C++ 专题                          60
来源：http://ba.lnxyls.cn

T 其他语言补充                          60
来源：http://rm.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://zr.bjjhwx.cn

------------------------------------
来源：http://bn.chemitech.net.cn

合计                                  2106 条
来源：http://bd.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://xr.panjiajie.cn

使用提醒
来源：http://eq.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ot.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mc.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jm.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://no.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ei.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://px.shtwfgs.cn

—— 文件结束 ——
来源：http://jq.wgjwhj.cn

================================================================================
来源：http://mu.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://cc.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://dn.nszjky.cn

================================================================================
来源：http://kk.huanxung.cn

【收录内容】
来源：http://sb.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qz.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bi.hahajie.cn

SQL · Bash · C · C++
来源：http://mb.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fm.shxzskj.cn

【使用说明】
来源：http://nw.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://io.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ns.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ng.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lp.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cx.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://at.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rb.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rf.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hk.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kc.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iz.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bc.asd995.cn

【文件统计】
来源：http://hs.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lb.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ix.haigaiapp.cn

目  录
来源：http://mo.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://et.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cg.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tk.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nb.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hf.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kz.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vd.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mx.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ij.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iz.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://co.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eh.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tt.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ec.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gu.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zs.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://op.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sv.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ky.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xx.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kx.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lc.lnxyls.cn

================================================================================
来源：http://bi.hnjuh.cn

A. 基础语法与类型
来源：http://ox.szsharing.cn

================================================================================
来源：http://lz.panjiajie.cn

[A01] Hello World
来源：http://ll.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://xf.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://lr.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://am.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fi.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://fd.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://uo.521024.cn

Ruby: puts "Hello, World!"
来源：http://at.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kg.nicolike.cn


<!-- 参考信息 -->