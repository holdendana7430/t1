代发 wailian999

[U15] Py：高精度计时
来源：http://jf.shxzukj.cn

t = time.perf_counter()
来源：http://ms.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://yd.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ss.jctech888.com.cn

[U17] Py：初始化日志
来源：http://rd.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://mc.bjjhwx.cn

[U18] Py：预编译正则
来源：http://rt.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://fy.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://sz.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ya.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://nw.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://kx.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://zm.huanxung.cn

@contextlib.contextmanager
来源：http://ez.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://wq.shxzskj.cn

list(zip(*m))
来源：http://kb.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://fl.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zb.lnxyls.cn

[U24] Py：路径操作
来源：http://eb.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ua.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://sx.hnjuh.cn

csv.DictReader(f)
来源：http://fu.colortex.cn

[U26] Py：并发下载
来源：http://cg.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jb.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://bu.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://qf.szsharing.cn

[U28] Py：类型别名
来源：http://vo.wgjwhj.cn

UserId = int
来源：http://zh.lnxyls.cn

[U29] Py：属性校验
来源：http://ei.szxytkj.cn

@property 与 @x.setter 配合
来源：http://bw.huixiangedu.cn

[U30] Py：数据类
来源：http://ar.shxzukj.cn

@dataclass(slots=True)
来源：http://ew.nicolike.cn

[U31] Py：单测
来源：http://yy.haigaiapp.cn

python -m pytest -q
来源：http://vh.bjjhwx.cn

[U32] Py：代码格式化
来源：http://zs.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://pw.nszjky.cn

[U33] Py：打包发布
来源：http://el.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://ss.9csxet.cn

[U34] Py：判断编码
来源：http://vd.wgjwhj.cn

chardet.detect(raw)
来源：http://kg.shtwfgs.cn

[U35] Py：发送邮件
来源：http://fh.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oz.chemitech.net.cn

[U36] Py：定时任务
来源：http://vv.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ru.huanxung.cn

[U37] Py：读写 Excel
来源：http://zl.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://km.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://jc.shxzukj.cn

Path(__file__).resolve().parent
来源：http://ms.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://eg.jctech888.com.cn

sys.stdout.isatty()
来源：http://lc.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://fj.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://ro.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://rj.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gf.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://uw.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vu.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://gq.asd995.cn

namespace App\Http;
来源：http://cb.huanxung.cn

[U44] PHP：开启严格类型
来源：http://xv.szxytkj.cn

declare(strict_types=1);
来源：http://yx.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://zk.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cc.9csxet.cn

[U46] PHP：可空类型
来源：http://ab.haigaiapp.cn

?string $name = null
来源：http://vi.jctech888.com.cn

[U47] PHP：联合类型
来源：http://ns.haigaiapp.cn

int|string $id
来源：http://fx.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://xu.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wc.lnxyls.cn

[U49] PHP：只读属性
来源：http://qv.asd995.cn

public readonly string $name
来源：http://xt.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ep.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://hu.shxzukj.cn

[U51] PHP：数组解构
来源：http://le.hahajie.cn

[$a, $b] = $arr;
来源：http://ft.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://rd.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://ea.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://xc.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://ml.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://nf.asd995.cn

$obj?->method()
来源：http://vx.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://bd.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xv.gzmigu.cn

[U56] PHP：命名参数
来源：http://kt.yuexingan06.cn

f(a: 1, b: 2)
来源：http://td.panjiajie.cn

[U57] PHP：字符串插值
来源：http://hd.yuexingan06.cn

"值: {$a}"
来源：http://en.szsharing.cn

[U58] PHP：数组三件套
来源：http://qm.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://je.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://na.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ew.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://ga.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pz.panjiajie.cn

[U61] PHP：正则
来源：http://rc.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nb.521024.cn

[U62] PHP：日期对象
来源：http://hd.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://af.bjjhwx.cn

[U63] PHP：文件读写
来源：http://cz.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uk.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://hz.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://pf.hnjuh.cn

[U65] PHP：会话
来源：http://bs.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lw.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://no.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fw.huanxung.cn

[U67] PHP：处理文件上传
来源：http://hq.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kv.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://co.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uf.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://gl.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cs.newstarts.cn

[U70] PHP：PDO 事务
来源：http://bs.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sa.szxytkj.cn

[U71] PHP：抛出异常
来源：http://wx.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://hq.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://jm.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://cz.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://fu.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://mp.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://ih.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://eb.lnxyls.cn

[U75] PHP：依赖注入
来源：http://za.yuntaijiaju.cn

composer require psr/container
来源：http://ed.521024.cn

[U76] PHP：简单路由
来源：http://bd.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ax.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://rm.szsharing.cn

composer require twig/twig
来源：http://fo.gzmigu.cn

[U78] PHP：单元测试
来源：http://lr.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://lf.szxytkj.cn

[U79] PHP：静态分析
来源：http://ox.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://ze.hahajie.cn

[U80] PHP：代码规范修复
来源：http://wi.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ym.yuexingan06.cn

[U81] JS：初始化项目
来源：http://vb.panjiajie.cn

npm init -y;  npm i express
来源：http://mk.asd995.cn

[U82] JS：package.json 脚本
来源：http://ny.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ez.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://qx.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pp.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://go.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jn.panjiajie.cn

[U85] JS：可选链
来源：http://wy.newstarts.cn

a?.b?.c
来源：http://id.9csxet.cn

[U86] JS：空值合并
来源：http://rk.shxzskj.cn

a ?? b
来源：http://hm.lnxyls.cn

[U87] JS：解构默认值
来源：http://mt.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://tr.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://eb.nszjky.cn

{ ...a, ...b }
来源：http://pr.hnjuh.cn

[U89] JS：数组去重
来源：http://oq.asd995.cn

[...new Set(arr)]
来源：http://ms.colortex.cn

[U90] JS：数字数组排序
来源：http://ji.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://ed.colortex.cn

[U91] JS：对象键值遍历
来源：http://pe.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ur.9csxet.cn

[U92] JS：深拷贝
来源：http://xk.bjjhwx.cn

structuredClone(obj)
来源：http://ql.muxihuayi.cn

[U93] JS：模板字符串
来源：http://mt.nicolike.cn

`共 ${n} 条`
来源：http://zg.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://va.yuexingan06.cn

const double = x => x * 2;
来源：http://rq.asd995.cn

[U95] JS：Promise 包装
来源：http://az.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://ye.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://dh.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hg.huanxung.cn

[U97] JS：并发请求
来源：http://ep.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tz.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://vr.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lr.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://mp.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://bz.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://yt.lnxyls.cn

document.querySelector(".item")
来源：http://vb.yuexingan06.cn

[U101] JS：classList 操作
来源：http://wj.521024.cn

el.classList.toggle("active")
来源：http://xq.yuexingan06.cn

[U102] JS：本地存储
来源：http://es.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mm.yuexingan06.cn

[U103] JS：定时器
来源：http://gg.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vq.colortex.cn

[U104] JS：防抖
来源：http://pc.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xu.jianghongdianzi.cn

[U105] JS：节流
来源：http://dd.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fq.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://zq.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jd.shxzskj.cn

[U107] JS：数字千分位
来源：http://rj.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cl.haigaiapp.cn

[U108] JS：随机整数
来源：http://vg.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://or.hnjuh.cn

[U109] JS：数组分组
来源：http://it.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://ab.hnjuh.cn

[U110] JS：数组分块
来源：http://vf.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sb.nszjky.cn

[U111] JS：对象转 Map
来源：http://wy.asd995.cn

new Map(Object.entries(obj))
来源：http://mt.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://dg.panjiajie.cn

"7".padStart(3, "0")
来源：http://ub.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://fz.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://od.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://sp.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tq.szxytkj.cn

[U115] JS：生成 UUID
来源：http://sa.muxihuayi.cn

crypto.randomUUID()
来源：http://wd.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://kz.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://yu.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://oj.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://bz.521024.cn

[U118] JS：开发服务器
来源：http://ji.szxytkj.cn

npm i -D vite;  npx vite
来源：http://iw.colortex.cn

[U119] JS：生产构建
来源：http://du.huixiangedu.cn

npx vite build
来源：http://zk.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://ke.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://ob.lnxyls.cn

================================================================================
来源：http://yc.panjiajie.cn

统计汇总
来源：http://wl.asd995.cn

================================================================================
来源：http://uw.shtwfgs.cn

按语言统计（条）：
来源：http://sl.jctech888.com.cn

Python ......... 252
来源：http://iv.jctech888.com.cn

PHP ............ 252
来源：http://dd.bjjhwx.cn

JavaScript ..... 252
来源：http://jw.521024.cn

TypeScript ..... 212
来源：http://id.jianghongdianzi.cn

Java ........... 212
来源：http://jg.huixiangedu.cn

Go ............. 212
来源：http://zh.shxzskj.cn

Ruby ........... 212
来源：http://ft.huixinmuqiang.cn

C# ............. 212
来源：http://on.521024.cn

C .............. 30
来源：http://hl.panjiajie.cn

C++ ............ 30
来源：http://pm.jctech888.com.cn

SQL ............ 90
来源：http://wu.hahajie.cn

Bash ........... 80
来源：http://yz.shxzskj.cn

Kotlin ......... 15
来源：http://ze.shxzukj.cn

Swift .......... 15
来源：http://zv.haigaiapp.cn

Lua ............ 10
来源：http://qy.yuexingan06.cn

Perl ........... 10
来源：http://uc.jianghongdianzi.cn

Scala .......... 10
来源：http://ex.colortex.cn

------------------------------------
来源：http://qd.jctech888.com.cn

合计 ........... 2106 条
来源：http://sz.nszjky.cn

按章节统计：
来源：http://yf.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hm.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uj.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ke.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rp.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fx.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ff.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tf.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ae.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bn.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ja.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://er.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fx.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rm.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mz.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eu.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sb.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://co.nicolike.cn

R Bash 专题                             80
来源：http://jz.szxytkj.cn

S C / C++ 专题                          60
来源：http://pb.chemitech.net.cn

T 其他语言补充                          60
来源：http://is.hnjuh.cn

U 高频实用片段                         120
来源：http://zr.wgjwhj.cn

------------------------------------
来源：http://st.nszjky.cn

合计                                  2106 条
来源：http://ca.asd995.cn

--------------------------------------------------------------------------------
来源：http://xw.shtwfgs.cn

使用提醒
来源：http://gz.szsharing.cn

--------------------------------------------------------------------------------
来源：http://sg.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yo.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dd.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zm.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rs.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ve.haigaiapp.cn

—— 文件结束 ——
来源：http://gi.gzmigu.cn

================================================================================
来源：http://qq.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://em.szsharing.cn

Common Programming Examples Cheat Book
来源：http://mw.chemitech.net.cn

================================================================================
来源：http://pw.panjiajie.cn

【收录内容】
来源：http://ya.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ex.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tg.9csxet.cn

SQL · Bash · C · C++
来源：http://is.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://me.nicolike.cn

【使用说明】
来源：http://dy.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eq.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://io.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ws.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xd.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ap.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fj.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vd.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ny.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ty.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yx.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kp.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pe.wgjwhj.cn

【文件统计】
来源：http://uf.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ku.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ny.nicolike.cn

目  录
来源：http://pa.asd995.cn

--------------------------------------------------------------------------------
来源：http://nd.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dp.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ut.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cv.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ri.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qg.bjjhwx.cn


<!-- 参考信息 -->