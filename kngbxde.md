代发 wailian999

[U19] Py：正则替换带回调
来源：http://cz.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gd.521024.cn

[U20] Py：缓存函数结果
来源：http://ns.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://gb.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://hd.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://nc.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://jh.huixinmuqiang.cn

list(zip(*m))
来源：http://vp.huanxung.cn

[U23] Py：分块读取大文件
来源：http://ue.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lr.shxzukj.cn

[U24] Py：路径操作
来源：http://pg.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gw.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://xo.jctech888.com.cn

csv.DictReader(f)
来源：http://gu.shtwfgs.cn

[U26] Py：并发下载
来源：http://ax.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gd.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://wa.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://qm.wgjwhj.cn

[U28] Py：类型别名
来源：http://pv.shxzskj.cn

UserId = int
来源：http://ka.szsharing.cn

[U29] Py：属性校验
来源：http://sh.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://ng.huanxung.cn

[U30] Py：数据类
来源：http://bj.shtwfgs.cn

@dataclass(slots=True)
来源：http://qy.panjiajie.cn

[U31] Py：单测
来源：http://xa.shxzskj.cn

python -m pytest -q
来源：http://al.wgjwhj.cn

[U32] Py：代码格式化
来源：http://bw.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://mm.chemitech.net.cn

[U33] Py：打包发布
来源：http://hl.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://lm.lnxyls.cn

[U34] Py：判断编码
来源：http://rq.muxihuayi.cn

chardet.detect(raw)
来源：http://wi.521024.cn

[U35] Py：发送邮件
来源：http://qq.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ug.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://bu.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://us.shxzskj.cn

[U37] Py：读写 Excel
来源：http://lv.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vo.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://yv.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://hn.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://os.haigaiapp.cn

sys.stdout.isatty()
来源：http://vi.521024.cn

[U40] Py：打印到标准错误
来源：http://ru.newstarts.cn

print("err", file=sys.stderr)
来源：http://in.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://bc.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ow.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://rk.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sq.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://lr.bookmarksfly.cn

namespace App\Http;
来源：http://ju.nicolike.cn

[U44] PHP：开启严格类型
来源：http://cw.haigaiapp.cn

declare(strict_types=1);
来源：http://uc.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://an.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.yuexingan06.cn

[U46] PHP：可空类型
来源：http://cb.szxytkj.cn

?string $name = null
来源：http://bl.nicolike.cn

[U47] PHP：联合类型
来源：http://bb.muxihuayi.cn

int|string $id
来源：http://os.lnxyls.cn

[U48] PHP：纯枚举
来源：http://sg.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://om.nszjky.cn

[U49] PHP：只读属性
来源：http://mc.szxytkj.cn

public readonly string $name
来源：http://qi.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://xw.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://dg.asd995.cn

[U51] PHP：数组解构
来源：http://sr.shxzukj.cn

[$a, $b] = $arr;
来源：http://rf.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://ca.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://cu.nicolike.cn

[U53] PHP：空合并运算符
来源：http://ia.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://cg.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://mq.shxzukj.cn

$obj?->method()
来源：http://ao.nszjky.cn

[U55] PHP：match 表达式
来源：http://xf.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xa.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://oh.lnxyls.cn

f(a: 1, b: 2)
来源：http://rt.shxzskj.cn

[U57] PHP：字符串插值
来源：http://og.huanxung.cn

"值: {$a}"
来源：http://yx.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ah.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ye.521024.cn

[U59] PHP：自定义排序
来源：http://ic.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iv.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://yx.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hb.wgjwhj.cn

[U61] PHP：正则
来源：http://en.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nb.wgjwhj.cn

[U62] PHP：日期对象
来源：http://ko.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hh.colortex.cn

[U63] PHP：文件读写
来源：http://ct.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nz.huanxung.cn

[U64] PHP：目录遍历
来源：http://vr.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://pb.hnjuh.cn

[U65] PHP：会话
来源：http://xq.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rf.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://lw.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://es.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://al.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nv.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://qg.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sr.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://kb.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vi.asd995.cn

[U70] PHP：PDO 事务
来源：http://rq.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://up.nicolike.cn

[U71] PHP：抛出异常
来源：http://yt.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://gl.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://xk.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://qx.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://cl.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://cj.colortex.cn

[U74] PHP：读取环境变量
来源：http://tp.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://mx.hahajie.cn

[U75] PHP：依赖注入
来源：http://ur.shtwfgs.cn

composer require psr/container
来源：http://rw.gzmigu.cn

[U76] PHP：简单路由
来源：http://hp.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zy.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://er.nszjky.cn

composer require twig/twig
来源：http://sl.haigaiapp.cn

[U78] PHP：单元测试
来源：http://nm.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ut.hnjuh.cn

[U79] PHP：静态分析
来源：http://hi.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://gw.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://di.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://md.lnxyls.cn

[U81] JS：初始化项目
来源：http://yh.nicolike.cn

npm init -y;  npm i express
来源：http://ml.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://mh.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qh.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://oj.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ar.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://mw.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xf.jctech888.com.cn

[U85] JS：可选链
来源：http://se.jctech888.com.cn

a?.b?.c
来源：http://hp.hnjuh.cn

[U86] JS：空值合并
来源：http://ce.bookmarksfly.cn

a ?? b
来源：http://al.hahajie.cn

[U87] JS：解构默认值
来源：http://sj.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://wc.nszjky.cn

[U88] JS：对象展开合并
来源：http://gm.wgjwhj.cn

{ ...a, ...b }
来源：http://ys.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://ws.hahajie.cn

[...new Set(arr)]
来源：http://zz.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://pd.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://of.nicolike.cn

[U91] JS：对象键值遍历
来源：http://tq.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cq.asd995.cn

[U92] JS：深拷贝
来源：http://ml.521024.cn

structuredClone(obj)
来源：http://hs.nicolike.cn

[U93] JS：模板字符串
来源：http://ao.lnxyls.cn

`共 ${n} 条`
来源：http://py.9csxet.cn

[U94] JS：箭头函数
来源：http://xe.huixiangedu.cn

const double = x => x * 2;
来源：http://tt.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ef.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://do.huanxung.cn

[U96] JS：async/await 与异常
来源：http://db.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zg.chemitech.net.cn

[U97] JS：并发请求
来源：http://gm.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ki.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://xt.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sn.nicolike.cn

[U99] JS：事件监听
来源：http://ep.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://ci.colortex.cn

[U100] JS：DOM 查询
来源：http://fx.panjiajie.cn

document.querySelector(".item")
来源：http://dn.shtwfgs.cn

[U101] JS：classList 操作
来源：http://zh.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://av.shxzskj.cn

[U102] JS：本地存储
来源：http://xn.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://al.chemitech.net.cn

[U103] JS：定时器
来源：http://qi.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aa.huanxung.cn

[U104] JS：防抖
来源：http://aj.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kt.yuexingan06.cn

[U105] JS：节流
来源：http://kh.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bn.nszjky.cn

[U106] JS：日期格式化
来源：http://mp.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cg.521024.cn

[U107] JS：数字千分位
来源：http://ez.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gw.shxzukj.cn

[U108] JS：随机整数
来源：http://wy.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hr.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://fj.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://cr.gzmigu.cn

[U110] JS：数组分块
来源：http://ow.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wm.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://gj.lnxyls.cn

new Map(Object.entries(obj))
来源：http://hf.wgjwhj.cn

[U112] JS：字符串补位
来源：http://cf.panjiajie.cn

"7".padStart(3, "0")
来源：http://vh.521024.cn

[U113] JS：正则替换全部
来源：http://ee.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://wr.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://so.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jg.lnxyls.cn

[U115] JS：生成 UUID
来源：http://qt.chemitech.net.cn

crypto.randomUUID()
来源：http://ep.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://sz.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://ks.shxzukj.cn

[U117] JS：单元测试
来源：http://om.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://hd.huixiangedu.cn

[U118] JS：开发服务器
来源：http://ue.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://wh.bookmarksfly.cn

[U119] JS：生产构建
来源：http://nv.hnjuh.cn

npx vite build
来源：http://ca.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://xh.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://ty.jianghongdianzi.cn

================================================================================
来源：http://bq.lnxyls.cn

统计汇总
来源：http://ur.huixinmuqiang.cn

================================================================================
来源：http://pj.chemitech.net.cn

按语言统计（条）：
来源：http://pm.yuexingan06.cn

Python ......... 252
来源：http://in.jctech888.com.cn

PHP ............ 252
来源：http://iq.shxzskj.cn

JavaScript ..... 252
来源：http://rm.chemitech.net.cn

TypeScript ..... 212
来源：http://sl.gzmigu.cn

Java ........... 212
来源：http://kx.bjjhwx.cn

Go ............. 212
来源：http://rf.yuntaijiaju.cn

Ruby ........... 212
来源：http://az.haigaiapp.cn

C# ............. 212
来源：http://ty.newstarts.cn

C .............. 30
来源：http://eu.jianghongdianzi.cn

C++ ............ 30
来源：http://qd.bjjhwx.cn

SQL ............ 90
来源：http://cb.huixiangedu.cn

Bash ........... 80
来源：http://qs.hnjuh.cn

Kotlin ......... 15
来源：http://yg.haigaiapp.cn

Swift .......... 15
来源：http://dd.jctech888.com.cn

Lua ............ 10
来源：http://nr.colortex.cn

Perl ........... 10
来源：http://nc.szxytkj.cn

Scala .......... 10
来源：http://hu.bookmarksfly.cn

------------------------------------
来源：http://vm.gzmigu.cn

合计 ........... 2106 条
来源：http://lu.haigaiapp.cn

按章节统计：
来源：http://xe.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xn.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mc.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rm.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pt.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wx.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dm.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sx.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ts.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fa.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iu.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jd.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ht.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xr.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zh.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fl.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jk.lnxyls.cn

Q SQL 专题                              90
来源：http://xs.yuexingan06.cn

R Bash 专题                             80
来源：http://zw.haigaiapp.cn

S C / C++ 专题                          60
来源：http://mo.shxzukj.cn

T 其他语言补充                          60
来源：http://qd.newstarts.cn

U 高频实用片段                         120
来源：http://oi.shxzskj.cn

------------------------------------
来源：http://ee.colortex.cn

合计                                  2106 条
来源：http://vl.521024.cn

--------------------------------------------------------------------------------
来源：http://fe.panjiajie.cn

使用提醒
来源：http://av.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mk.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nn.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mr.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://td.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cp.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yl.jctech888.com.cn

—— 文件结束 ——
来源：http://bo.shxzskj.cn

================================================================================
来源：http://tk.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://gy.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://ys.hnjuh.cn

================================================================================
来源：http://sj.szxytkj.cn

【收录内容】
来源：http://ll.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ei.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hy.szsharing.cn

SQL · Bash · C · C++
来源：http://ox.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kj.lnxyls.cn

【使用说明】
来源：http://ai.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ci.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sy.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tl.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tz.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hr.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gy.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nz.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ug.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ep.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rp.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jb.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ej.bjjhwx.cn

【文件统计】
来源：http://mq.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://we.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://fw.shxzskj.cn

目  录
来源：http://xc.colortex.cn

--------------------------------------------------------------------------------
来源：http://az.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xg.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zy.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vk.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ci.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ps.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zv.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ek.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pn.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://es.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mm.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ao.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dv.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fz.nicolike.cn


<!-- 参考信息 -->