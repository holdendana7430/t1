代发 wailian999

[U15] Py：高精度计时
来源：http://qs.hnjuh.cn

t = time.perf_counter()
来源：http://cr.9csxet.cn

[U16] Py：命令行参数解析
来源：http://ke.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cl.shxzskj.cn

[U17] Py：初始化日志
来源：http://rk.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://ht.panjiajie.cn

[U18] Py：预编译正则
来源：http://zw.colortex.cn

pat = re.compile(r"\d+")
来源：http://ft.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://yc.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rj.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://xu.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://yr.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://ba.chemitech.net.cn

@contextlib.contextmanager
来源：http://vc.shxzukj.cn

[U22] Py：矩阵转置
来源：http://ps.nszjky.cn

list(zip(*m))
来源：http://fi.nicolike.cn

[U23] Py：分块读取大文件
来源：http://lc.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qj.newstarts.cn

[U24] Py：路径操作
来源：http://ui.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iv.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://lz.yuntaijiaju.cn

csv.DictReader(f)
来源：http://gf.shtwfgs.cn

[U26] Py：并发下载
来源：http://pb.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sv.9csxet.cn

[U27] Py：异步 HTTP
来源：http://sm.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://gd.yuexingan06.cn

[U28] Py：类型别名
来源：http://ju.hnjuh.cn

UserId = int
来源：http://qy.hahajie.cn

[U29] Py：属性校验
来源：http://at.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://yy.newstarts.cn

[U30] Py：数据类
来源：http://od.nszjky.cn

@dataclass(slots=True)
来源：http://xv.shtwfgs.cn

[U31] Py：单测
来源：http://uq.jianghongdianzi.cn

python -m pytest -q
来源：http://ja.szsharing.cn

[U32] Py：代码格式化
来源：http://sn.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://fd.szxytkj.cn

[U33] Py：打包发布
来源：http://zz.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://wc.panjiajie.cn

[U34] Py：判断编码
来源：http://vk.chemitech.net.cn

chardet.detect(raw)
来源：http://xd.szxytkj.cn

[U35] Py：发送邮件
来源：http://ft.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ux.asd995.cn

[U36] Py：定时任务
来源：http://qe.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://jb.shxzskj.cn

[U37] Py：读写 Excel
来源：http://du.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ho.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://tg.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://kz.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://eo.szsharing.cn

sys.stdout.isatty()
来源：http://kk.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ta.shxzskj.cn

print("err", file=sys.stderr)
来源：http://um.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://nx.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://te.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://tr.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jc.szsharing.cn

[U43] PHP：声明命名空间
来源：http://bv.shtwfgs.cn

namespace App\Http;
来源：http://aq.colortex.cn

[U44] PHP：开启严格类型
来源：http://dt.szxytkj.cn

declare(strict_types=1);
来源：http://sx.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://pl.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zz.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://cr.bjjhwx.cn

?string $name = null
来源：http://ns.szxytkj.cn

[U47] PHP：联合类型
来源：http://sl.9csxet.cn

int|string $id
来源：http://qs.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://gg.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ba.gzmigu.cn

[U49] PHP：只读属性
来源：http://iv.hahajie.cn

public readonly string $name
来源：http://kk.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://bd.szsharing.cn

public function __construct(private int $id) {}
来源：http://ov.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://xj.huixiangedu.cn

[$a, $b] = $arr;
来源：http://wp.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://va.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://uc.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://yx.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://bs.lnxyls.cn

[U54] PHP：空安全调用
来源：http://rr.huanxung.cn

$obj?->method()
来源：http://ge.newstarts.cn

[U55] PHP：match 表达式
来源：http://dm.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://el.asd995.cn

[U56] PHP：命名参数
来源：http://xw.wgjwhj.cn

f(a: 1, b: 2)
来源：http://nj.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://ys.jianghongdianzi.cn

"值: {$a}"
来源：http://tx.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ym.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://al.colortex.cn

[U59] PHP：自定义排序
来源：http://tv.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xc.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://xf.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kr.gzmigu.cn

[U61] PHP：正则
来源：http://ta.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ow.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://vc.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://db.nszjky.cn

[U63] PHP：文件读写
来源：http://ag.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ul.lnxyls.cn

[U64] PHP：目录遍历
来源：http://yv.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://ng.yuntaijiaju.cn

[U65] PHP：会话
来源：http://ow.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gd.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://et.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sn.colortex.cn

[U67] PHP：处理文件上传
来源：http://vb.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ky.9csxet.cn

[U68] PHP：PDO 连接
来源：http://eq.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ja.asd995.cn

[U69] PHP：PDO 预处理
来源：http://wz.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ds.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://mx.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ye.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ix.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://ez.szxytkj.cn

[U72] PHP：写错误日志
来源：http://ro.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://vh.521024.cn

[U73] PHP：读取 ini 配置
来源：http://vz.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://rg.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://ua.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://np.panjiajie.cn

[U75] PHP：依赖注入
来源：http://iy.szxytkj.cn

composer require psr/container
来源：http://jm.hnjuh.cn

[U76] PHP：简单路由
来源：http://ul.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ck.shxzskj.cn

[U77] PHP：模板渲染
来源：http://ho.szxytkj.cn

composer require twig/twig
来源：http://yi.gzmigu.cn

[U78] PHP：单元测试
来源：http://pq.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://bo.colortex.cn

[U79] PHP：静态分析
来源：http://lk.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://cy.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://ms.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sc.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://hg.haigaiapp.cn

npm init -y;  npm i express
来源：http://yz.szsharing.cn

[U82] JS：package.json 脚本
来源：http://xy.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lf.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://cw.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zx.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://ix.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://su.haigaiapp.cn

[U85] JS：可选链
来源：http://dg.jianghongdianzi.cn

a?.b?.c
来源：http://vi.shxzskj.cn

[U86] JS：空值合并
来源：http://nr.9csxet.cn

a ?? b
来源：http://yc.chemitech.net.cn

[U87] JS：解构默认值
来源：http://oh.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://qc.shxzskj.cn

[U88] JS：对象展开合并
来源：http://fl.szxytkj.cn

{ ...a, ...b }
来源：http://er.muxihuayi.cn

[U89] JS：数组去重
来源：http://ia.szsharing.cn

[...new Set(arr)]
来源：http://yq.szsharing.cn

[U90] JS：数字数组排序
来源：http://fv.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://cv.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://dz.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ry.huixiangedu.cn

[U92] JS：深拷贝
来源：http://aw.bookmarksfly.cn

structuredClone(obj)
来源：http://ii.huixiangedu.cn

[U93] JS：模板字符串
来源：http://np.haigaiapp.cn

`共 ${n} 条`
来源：http://qc.shxzskj.cn

[U94] JS：箭头函数
来源：http://mc.shtwfgs.cn

const double = x => x * 2;
来源：http://ei.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://aq.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://yc.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://ts.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ye.shtwfgs.cn

[U97] JS：并发请求
来源：http://wi.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cb.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://xs.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cl.lnxyls.cn

[U99] JS：事件监听
来源：http://ds.nicolike.cn

el.addEventListener("click", e => {})
来源：http://pe.9csxet.cn

[U100] JS：DOM 查询
来源：http://ru.panjiajie.cn

document.querySelector(".item")
来源：http://fo.szsharing.cn

[U101] JS：classList 操作
来源：http://vp.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://ve.nicolike.cn

[U102] JS：本地存储
来源：http://ml.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gl.lnxyls.cn

[U103] JS：定时器
来源：http://wb.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://si.gzmigu.cn

[U104] JS：防抖
来源：http://xu.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://od.jianghongdianzi.cn

[U105] JS：节流
来源：http://pq.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lq.yuexingan06.cn

[U106] JS：日期格式化
来源：http://yj.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nj.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://jz.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fx.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://gf.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uf.asd995.cn

[U109] JS：数组分组
来源：http://sd.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://pv.asd995.cn

[U110] JS：数组分块
来源：http://jg.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vk.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://lx.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://pv.shtwfgs.cn

[U112] JS：字符串补位
来源：http://lu.colortex.cn

"7".padStart(3, "0")
来源：http://az.9csxet.cn

[U113] JS：正则替换全部
来源：http://xo.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://kv.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://xz.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bz.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://zn.bjjhwx.cn

crypto.randomUUID()
来源：http://wz.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://zd.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://xa.wgjwhj.cn

[U117] JS：单元测试
来源：http://cj.asd995.cn

npm i -D vitest;  npx vitest
来源：http://ux.shxzukj.cn

[U118] JS：开发服务器
来源：http://sd.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://hr.nicolike.cn

[U119] JS：生产构建
来源：http://ax.9csxet.cn

npx vite build
来源：http://oh.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://fq.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://tw.hahajie.cn

================================================================================
来源：http://rk.nicolike.cn

统计汇总
来源：http://lk.yuntaijiaju.cn

================================================================================
来源：http://wp.hnjuh.cn

按语言统计（条）：
来源：http://xa.colortex.cn

Python ......... 252
来源：http://yh.huixiangedu.cn

PHP ............ 252
来源：http://el.huixiangedu.cn

JavaScript ..... 252
来源：http://ka.hnjuh.cn

TypeScript ..... 212
来源：http://zi.chemitech.net.cn

Java ........... 212
来源：http://ok.yuexingan06.cn

Go ............. 212
来源：http://pq.szxytkj.cn

Ruby ........... 212
来源：http://xn.shtwfgs.cn

C# ............. 212
来源：http://zk.jianghongdianzi.cn

C .............. 30
来源：http://or.shxzukj.cn

C++ ............ 30
来源：http://cq.jctech888.com.cn

SQL ............ 90
来源：http://tf.yuntaijiaju.cn

Bash ........... 80
来源：http://bi.newstarts.cn

Kotlin ......... 15
来源：http://ql.newstarts.cn

Swift .......... 15
来源：http://it.colortex.cn

Lua ............ 10
来源：http://cl.jctech888.com.cn

Perl ........... 10
来源：http://pf.huixinmuqiang.cn

Scala .......... 10
来源：http://fl.lnxyls.cn

------------------------------------
来源：http://gr.hahajie.cn

合计 ........... 2106 条
来源：http://qq.newstarts.cn

按章节统计：
来源：http://ay.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sl.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://py.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dw.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://td.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bw.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yr.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dh.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xg.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://me.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cn.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pt.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mc.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ul.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ct.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://id.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nq.shtwfgs.cn

Q SQL 专题                              90
来源：http://px.szxytkj.cn

R Bash 专题                             80
来源：http://rd.jctech888.com.cn

S C / C++ 专题                          60
来源：http://gf.chemitech.net.cn

T 其他语言补充                          60
来源：http://rg.huanxung.cn

U 高频实用片段                         120
来源：http://yl.haigaiapp.cn

------------------------------------
来源：http://yn.huixiangedu.cn

合计                                  2106 条
来源：http://pf.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ka.huanxung.cn

使用提醒
来源：http://jl.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://gx.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yj.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pl.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mc.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rk.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hg.nicolike.cn

—— 文件结束 ——
来源：http://aj.colortex.cn

================================================================================
来源：http://tt.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://hh.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://on.haigaiapp.cn

================================================================================
来源：http://ix.9csxet.cn

【收录内容】
来源：http://bj.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://be.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sj.shtwfgs.cn

SQL · Bash · C · C++
来源：http://pr.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gx.huixiangedu.cn

【使用说明】
来源：http://mt.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mp.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sa.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yx.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://du.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fo.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wt.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://of.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fz.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eb.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jd.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ix.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vn.huixiangedu.cn

【文件统计】
来源：http://gx.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ok.szsharing.cn

--------------------------------------------------------------------------------
来源：http://yj.wgjwhj.cn

目  录
来源：http://wa.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://dv.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cy.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://af.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zn.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ao.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zo.wgjwhj.cn


<!-- 参考信息 -->