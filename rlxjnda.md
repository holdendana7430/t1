代发 wailian999

[U19] Py：正则替换带回调
来源：http://wj.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kv.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://af.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://zr.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://zd.hnjuh.cn

@contextlib.contextmanager
来源：http://dz.hnjuh.cn

[U22] Py：矩阵转置
来源：http://ed.wgjwhj.cn

list(zip(*m))
来源：http://yg.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://fw.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ut.muxihuayi.cn

[U24] Py：路径操作
来源：http://em.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://im.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://eg.chemitech.net.cn

csv.DictReader(f)
来源：http://bm.huanxung.cn

[U26] Py：并发下载
来源：http://kr.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ek.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://to.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://ut.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://ji.nszjky.cn

UserId = int
来源：http://qb.szxytkj.cn

[U29] Py：属性校验
来源：http://ew.szsharing.cn

@property 与 @x.setter 配合
来源：http://hn.nszjky.cn

[U30] Py：数据类
来源：http://kk.huixiangedu.cn

@dataclass(slots=True)
来源：http://dp.hnjuh.cn

[U31] Py：单测
来源：http://hv.gzmigu.cn

python -m pytest -q
来源：http://ff.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://se.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://zg.szsharing.cn

[U33] Py：打包发布
来源：http://yb.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://cl.yuexingan06.cn

[U34] Py：判断编码
来源：http://ba.chemitech.net.cn

chardet.detect(raw)
来源：http://jg.chemitech.net.cn

[U35] Py：发送邮件
来源：http://zo.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zh.muxihuayi.cn

[U36] Py：定时任务
来源：http://ry.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://yw.asd995.cn

[U37] Py：读写 Excel
来源：http://nn.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bs.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://dv.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://yw.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://sv.lnxyls.cn

sys.stdout.isatty()
来源：http://ks.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://ze.szsharing.cn

print("err", file=sys.stderr)
来源：http://tg.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://no.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xo.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://dc.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://te.huanxung.cn

[U43] PHP：声明命名空间
来源：http://te.bookmarksfly.cn

namespace App\Http;
来源：http://hd.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://hh.newstarts.cn

declare(strict_types=1);
来源：http://by.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://iq.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mf.yuexingan06.cn

[U46] PHP：可空类型
来源：http://ks.9csxet.cn

?string $name = null
来源：http://ra.shxzskj.cn

[U47] PHP：联合类型
来源：http://kn.panjiajie.cn

int|string $id
来源：http://ob.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://ar.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ho.muxihuayi.cn

[U49] PHP：只读属性
来源：http://qo.yuntaijiaju.cn

public readonly string $name
来源：http://vk.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://nn.hnjuh.cn

public function __construct(private int $id) {}
来源：http://uv.jctech888.com.cn

[U51] PHP：数组解构
来源：http://xn.nicolike.cn

[$a, $b] = $arr;
来源：http://iq.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://qc.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://fr.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://ul.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://uq.nszjky.cn

[U54] PHP：空安全调用
来源：http://cm.9csxet.cn

$obj?->method()
来源：http://xt.shxzskj.cn

[U55] PHP：match 表达式
来源：http://mr.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ts.hahajie.cn

[U56] PHP：命名参数
来源：http://he.gzmigu.cn

f(a: 1, b: 2)
来源：http://fa.shxzskj.cn

[U57] PHP：字符串插值
来源：http://qa.szsharing.cn

"值: {$a}"
来源：http://sx.asd995.cn

[U58] PHP：数组三件套
来源：http://el.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ku.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://wl.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uh.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://am.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hr.huanxung.cn

[U61] PHP：正则
来源：http://ww.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ne.haigaiapp.cn

[U62] PHP：日期对象
来源：http://gm.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hn.hnjuh.cn

[U63] PHP：文件读写
来源：http://kg.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://py.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://jv.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://ok.hnjuh.cn

[U65] PHP：会话
来源：http://gh.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pl.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://tb.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zc.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://hh.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xq.colortex.cn

[U68] PHP：PDO 连接
来源：http://iu.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ye.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://zi.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ta.nszjky.cn

[U70] PHP：PDO 事务
来源：http://tw.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pt.521024.cn

[U71] PHP：抛出异常
来源：http://az.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://fx.521024.cn

[U72] PHP：写错误日志
来源：http://zn.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://gb.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://in.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://ua.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://hr.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://vy.hnjuh.cn

[U75] PHP：依赖注入
来源：http://du.colortex.cn

composer require psr/container
来源：http://os.wgjwhj.cn

[U76] PHP：简单路由
来源：http://qo.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tr.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://mc.shxzskj.cn

composer require twig/twig
来源：http://sk.bjjhwx.cn

[U78] PHP：单元测试
来源：http://ew.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://bi.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://ox.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://rc.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://oo.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pk.chemitech.net.cn

[U81] JS：初始化项目
来源：http://qk.haigaiapp.cn

npm init -y;  npm i express
来源：http://kg.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://af.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kr.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://jp.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xe.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://uh.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yx.lnxyls.cn

[U85] JS：可选链
来源：http://wz.hahajie.cn

a?.b?.c
来源：http://wg.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://qz.huixinmuqiang.cn

a ?? b
来源：http://gx.haigaiapp.cn

[U87] JS：解构默认值
来源：http://xn.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://gb.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://mo.jianghongdianzi.cn

{ ...a, ...b }
来源：http://va.szsharing.cn

[U89] JS：数组去重
来源：http://wq.shxzskj.cn

[...new Set(arr)]
来源：http://yt.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://ou.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://kg.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://jy.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fw.panjiajie.cn

[U92] JS：深拷贝
来源：http://pc.hahajie.cn

structuredClone(obj)
来源：http://lp.szsharing.cn

[U93] JS：模板字符串
来源：http://xa.yuntaijiaju.cn

`共 ${n} 条`
来源：http://pi.szsharing.cn

[U94] JS：箭头函数
来源：http://yi.jctech888.com.cn

const double = x => x * 2;
来源：http://qz.hahajie.cn

[U95] JS：Promise 包装
来源：http://sb.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://yr.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://xq.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://im.szsharing.cn

[U97] JS：并发请求
来源：http://wl.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://po.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://hy.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tb.asd995.cn

[U99] JS：事件监听
来源：http://px.hahajie.cn

el.addEventListener("click", e => {})
来源：http://rv.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://su.newstarts.cn

document.querySelector(".item")
来源：http://ju.wgjwhj.cn

[U101] JS：classList 操作
来源：http://yc.asd995.cn

el.classList.toggle("active")
来源：http://sk.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://vf.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nn.panjiajie.cn

[U103] JS：定时器
来源：http://fx.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rd.shxzukj.cn

[U104] JS：防抖
来源：http://sa.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xm.szsharing.cn

[U105] JS：节流
来源：http://ud.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://at.nszjky.cn

[U106] JS：日期格式化
来源：http://tq.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ns.wgjwhj.cn

[U107] JS：数字千分位
来源：http://mr.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eq.haigaiapp.cn

[U108] JS：随机整数
来源：http://ll.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cp.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://vw.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://fo.huixiangedu.cn

[U110] JS：数组分块
来源：http://er.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ly.nicolike.cn

[U111] JS：对象转 Map
来源：http://uj.huanxung.cn

new Map(Object.entries(obj))
来源：http://sg.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://to.huanxung.cn

"7".padStart(3, "0")
来源：http://ck.hahajie.cn

[U113] JS：正则替换全部
来源：http://gy.asd995.cn

s.replaceAll("a", "b")
来源：http://wj.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://zs.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vl.hnjuh.cn

[U115] JS：生成 UUID
来源：http://cd.nicolike.cn

crypto.randomUUID()
来源：http://oy.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://li.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://yz.panjiajie.cn

[U117] JS：单元测试
来源：http://ly.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://kz.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://zx.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://qk.hnjuh.cn

[U119] JS：生产构建
来源：http://zu.szxytkj.cn

npx vite build
来源：http://sh.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://jl.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://ud.hnjuh.cn

================================================================================
来源：http://zo.shxzskj.cn

统计汇总
来源：http://lo.bookmarksfly.cn

================================================================================
来源：http://ds.colortex.cn

按语言统计（条）：
来源：http://zp.wgjwhj.cn

Python ......... 252
来源：http://bu.szsharing.cn

PHP ............ 252
来源：http://hb.jctech888.com.cn

JavaScript ..... 252
来源：http://rn.huanxung.cn

TypeScript ..... 212
来源：http://pw.hahajie.cn

Java ........... 212
来源：http://la.521024.cn

Go ............. 212
来源：http://tk.yuntaijiaju.cn

Ruby ........... 212
来源：http://bd.haigaiapp.cn

C# ............. 212
来源：http://zf.newstarts.cn

C .............. 30
来源：http://pf.wgjwhj.cn

C++ ............ 30
来源：http://xw.szsharing.cn

SQL ............ 90
来源：http://lc.9csxet.cn

Bash ........... 80
来源：http://dm.hahajie.cn

Kotlin ......... 15
来源：http://rm.yuexingan06.cn

Swift .......... 15
来源：http://za.gzmigu.cn

Lua ............ 10
来源：http://eu.hahajie.cn

Perl ........... 10
来源：http://mx.bookmarksfly.cn

Scala .......... 10
来源：http://or.jianghongdianzi.cn

------------------------------------
来源：http://wx.muxihuayi.cn

合计 ........... 2106 条
来源：http://cf.bookmarksfly.cn

按章节统计：
来源：http://fv.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tw.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mi.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qb.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://af.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://db.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://od.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://et.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iz.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hq.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tn.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nl.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pw.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zd.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ge.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dd.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mv.shxzukj.cn

Q SQL 专题                              90
来源：http://on.shxzskj.cn

R Bash 专题                             80
来源：http://xr.chemitech.net.cn

S C / C++ 专题                          60
来源：http://gc.panjiajie.cn

T 其他语言补充                          60
来源：http://pw.lnxyls.cn

U 高频实用片段                         120
来源：http://xl.szxytkj.cn

------------------------------------
来源：http://zo.jianghongdianzi.cn

合计                                  2106 条
来源：http://on.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://vn.colortex.cn

使用提醒
来源：http://di.nicolike.cn

--------------------------------------------------------------------------------
来源：http://uk.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fg.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bs.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bu.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ky.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jb.yuexingan06.cn

—— 文件结束 ——
来源：http://hh.gzmigu.cn

================================================================================
来源：http://vi.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://ds.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://me.jctech888.com.cn

================================================================================
来源：http://jm.nicolike.cn

【收录内容】
来源：http://co.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pr.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vw.huanxung.cn

SQL · Bash · C · C++
来源：http://nb.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jt.hnjuh.cn

【使用说明】
来源：http://jb.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zm.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ge.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://om.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dy.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ec.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gw.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ij.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xh.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sb.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ee.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gj.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cz.muxihuayi.cn

【文件统计】
来源：http://dp.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ng.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://rd.huixiangedu.cn

目  录
来源：http://ke.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://rj.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xu.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mv.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cg.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tn.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zw.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qk.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vx.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hq.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rk.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rt.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://um.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vf.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hl.asd995.cn


<!-- 参考信息 -->