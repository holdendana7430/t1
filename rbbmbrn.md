代发 wailian999

[T47] Perl：正则捕获
来源：http://ty.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xc.huixiangedu.cn

[T48] Perl：正则替换
来源：http://pc.521024.cn

$s =~ s/old/new/g;
来源：http://kp.szxytkj.cn

[T49] Perl：函数
来源：http://we.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wp.nszjky.cn

[T50] Perl：逐行读文件
来源：http://an.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ty.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://rk.shxzukj.cn

[T51] Scala：Hello World
来源：http://ks.chemitech.net.cn

println("Hello")
来源：http://rs.szsharing.cn

[T52] Scala：变量
来源：http://xp.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://zt.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://ov.lnxyls.cn

s"值: $b"
来源：http://xv.jctech888.com.cn

[T54] Scala：集合映射
来源：http://nb.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://gw.521024.cn

[T55] Scala：集合过滤
来源：http://at.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ua.szxytkj.cn

[T56] Scala：样例类
来源：http://mm.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://hq.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ew.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sm.9csxet.cn

[T58] Scala：函数定义
来源：http://wp.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://da.521024.cn

[T59] Scala：循环
来源：http://at.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://xe.newstarts.cn

[T60] Scala：折叠
来源：http://bl.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fx.asd995.cn

================================================================================
来源：http://bp.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ma.hahajie.cn

================================================================================
来源：http://ju.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://bp.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://de.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://wu.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ts.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://fz.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ag.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://dl.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uo.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://vi.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://gk.nicolike.cn

[U06] Py：合并两个字典
来源：http://do.haigaiapp.cn

{**a, **b}
来源：http://fj.521024.cn

[U07] Py：反转字典键值
来源：http://qi.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://la.nicolike.cn

[U08] Py：展平二维列表
来源：http://qr.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://bm.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://bl.muxihuayi.cn

max(d, key=d.get)
来源：http://lo.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://me.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://on.nicolike.cn

[U11] Py：生成器表达式
来源：http://gl.shxzukj.cn

(x * 2 for x in arr)
来源：http://vo.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pd.521024.cn

Counter(arr).most_common(3)
来源：http://bq.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ch.lnxyls.cn

deque(maxlen=10)
来源：http://qy.asd995.cn

[U14] Py：分组收集到列表
来源：http://yi.nszjky.cn

defaultdict(list)
来源：http://sq.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ky.nszjky.cn

t = time.perf_counter()
来源：http://aq.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://tm.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lk.shxzukj.cn

[U17] Py：初始化日志
来源：http://dg.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ga.shxzukj.cn

[U18] Py：预编译正则
来源：http://hj.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://bk.9csxet.cn

[U19] Py：正则替换带回调
来源：http://vv.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gh.hahajie.cn

[U20] Py：缓存函数结果
来源：http://vn.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://kn.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ya.asd995.cn

@contextlib.contextmanager
来源：http://ia.szxytkj.cn

[U22] Py：矩阵转置
来源：http://tr.yuntaijiaju.cn

list(zip(*m))
来源：http://cl.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://au.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kj.shtwfgs.cn

[U24] Py：路径操作
来源：http://xv.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://my.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://df.yuntaijiaju.cn

csv.DictReader(f)
来源：http://cz.nicolike.cn

[U26] Py：并发下载
来源：http://cs.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yc.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://qd.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://hy.szsharing.cn

[U28] Py：类型别名
来源：http://ss.muxihuayi.cn

UserId = int
来源：http://dl.colortex.cn

[U29] Py：属性校验
来源：http://ty.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://no.shtwfgs.cn

[U30] Py：数据类
来源：http://zw.shtwfgs.cn

@dataclass(slots=True)
来源：http://gb.colortex.cn

[U31] Py：单测
来源：http://oj.521024.cn

python -m pytest -q
来源：http://gx.huanxung.cn

[U32] Py：代码格式化
来源：http://ix.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://lh.szxytkj.cn

[U33] Py：打包发布
来源：http://jx.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://zh.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://zd.hahajie.cn

chardet.detect(raw)
来源：http://uy.shxzskj.cn

[U35] Py：发送邮件
来源：http://eb.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ka.521024.cn

[U36] Py：定时任务
来源：http://qv.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://vb.colortex.cn

[U37] Py：读写 Excel
来源：http://pm.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://od.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://ia.nicolike.cn

Path(__file__).resolve().parent
来源：http://dr.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://if.chemitech.net.cn

sys.stdout.isatty()
来源：http://wb.nicolike.cn

[U40] Py：打印到标准错误
来源：http://fr.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://ma.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://fp.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://me.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://bs.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://le.nszjky.cn

[U43] PHP：声明命名空间
来源：http://su.nicolike.cn

namespace App\Http;
来源：http://fd.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://hu.521024.cn

declare(strict_types=1);
来源：http://pf.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://wl.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.wgjwhj.cn

[U46] PHP：可空类型
来源：http://vp.bjjhwx.cn

?string $name = null
来源：http://kp.lnxyls.cn

[U47] PHP：联合类型
来源：http://dg.bjjhwx.cn

int|string $id
来源：http://bn.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://lt.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ud.bjjhwx.cn

[U49] PHP：只读属性
来源：http://kj.huanxung.cn

public readonly string $name
来源：http://oq.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://pi.shxzukj.cn

public function __construct(private int $id) {}
来源：http://wi.nicolike.cn

[U51] PHP：数组解构
来源：http://ix.colortex.cn

[$a, $b] = $arr;
来源：http://lg.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ds.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ow.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://do.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://tm.521024.cn

[U54] PHP：空安全调用
来源：http://yo.muxihuayi.cn

$obj?->method()
来源：http://cd.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://lm.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iz.bjjhwx.cn

[U56] PHP：命名参数
来源：http://rt.chemitech.net.cn

f(a: 1, b: 2)
来源：http://ah.panjiajie.cn

[U57] PHP：字符串插值
来源：http://dg.bookmarksfly.cn

"值: {$a}"
来源：http://uf.9csxet.cn

[U58] PHP：数组三件套
来源：http://ob.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bl.nicolike.cn

[U59] PHP：自定义排序
来源：http://xq.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ti.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://sf.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yr.9csxet.cn

[U61] PHP：正则
来源：http://il.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vr.lnxyls.cn

[U62] PHP：日期对象
来源：http://dk.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fa.nicolike.cn

[U63] PHP：文件读写
来源：http://ut.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qz.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://rz.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://jn.lnxyls.cn

[U65] PHP：会话
来源：http://ye.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bz.colortex.cn

[U66] PHP：设置 Cookie
来源：http://xn.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sg.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://ld.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ld.521024.cn

[U68] PHP：PDO 连接
来源：http://uo.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oh.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://gu.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xt.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://wg.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ee.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://wb.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://rv.nszjky.cn

[U72] PHP：写错误日志
来源：http://wa.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://pl.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://kz.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://po.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://sr.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://mx.lnxyls.cn

[U75] PHP：依赖注入
来源：http://cm.huanxung.cn

composer require psr/container
来源：http://cp.jctech888.com.cn

[U76] PHP：简单路由
来源：http://nh.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jo.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://km.huixinmuqiang.cn

composer require twig/twig
来源：http://wl.9csxet.cn

[U78] PHP：单元测试
来源：http://et.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://qf.hahajie.cn

[U79] PHP：静态分析
来源：http://hk.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://ju.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://nb.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://on.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://wm.nszjky.cn

npm init -y;  npm i express
来源：http://ul.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://wn.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://be.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://as.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sc.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ub.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xv.yuntaijiaju.cn

[U85] JS：可选链
来源：http://hl.shxzskj.cn

a?.b?.c
来源：http://ed.521024.cn

[U86] JS：空值合并
来源：http://fu.muxihuayi.cn

a ?? b
来源：http://mx.hnjuh.cn

[U87] JS：解构默认值
来源：http://yb.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://gy.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://hs.hahajie.cn

{ ...a, ...b }
来源：http://md.muxihuayi.cn

[U89] JS：数组去重
来源：http://jf.bjjhwx.cn

[...new Set(arr)]
来源：http://tm.lnxyls.cn

[U90] JS：数字数组排序
来源：http://hn.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://nq.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://qc.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zj.huanxung.cn

[U92] JS：深拷贝
来源：http://op.haigaiapp.cn

structuredClone(obj)
来源：http://sh.nicolike.cn

[U93] JS：模板字符串
来源：http://ux.szsharing.cn

`共 ${n} 条`
来源：http://ig.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ds.huixiangedu.cn

const double = x => x * 2;
来源：http://ha.szxytkj.cn

[U95] JS：Promise 包装
来源：http://dw.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://if.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://iw.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vo.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://qx.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dk.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://if.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ef.shxzukj.cn

[U99] JS：事件监听
来源：http://oe.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://yq.shxzskj.cn

[U100] JS：DOM 查询
来源：http://eq.huanxung.cn

document.querySelector(".item")
来源：http://rs.shxzskj.cn

[U101] JS：classList 操作
来源：http://vn.szsharing.cn

el.classList.toggle("active")
来源：http://ew.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://yu.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tk.yuntaijiaju.cn

[U103] JS：定时器
来源：http://xz.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ol.nicolike.cn

[U104] JS：防抖
来源：http://ym.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dy.nicolike.cn

[U105] JS：节流
来源：http://ex.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://is.szsharing.cn

[U106] JS：日期格式化
来源：http://nj.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dr.shxzskj.cn

[U107] JS：数字千分位
来源：http://hp.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lh.shxzukj.cn

[U108] JS：随机整数
来源：http://wr.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xw.nszjky.cn

[U109] JS：数组分组
来源：http://on.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://dj.huanxung.cn

[U110] JS：数组分块
来源：http://aq.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kk.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://cv.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://js.hahajie.cn

[U112] JS：字符串补位
来源：http://gl.colortex.cn

"7".padStart(3, "0")
来源：http://kt.hahajie.cn

[U113] JS：正则替换全部
来源：http://th.hahajie.cn

s.replaceAll("a", "b")
来源：http://jb.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ii.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ef.nszjky.cn

[U115] JS：生成 UUID
来源：http://ez.jianghongdianzi.cn

crypto.randomUUID()
来源：http://im.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://vm.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://kh.9csxet.cn

[U117] JS：单元测试
来源：http://xj.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://vh.newstarts.cn

[U118] JS：开发服务器
来源：http://by.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://vq.wgjwhj.cn

[U119] JS：生产构建
来源：http://nn.huanxung.cn

npx vite build
来源：http://mz.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://tv.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://bv.lnxyls.cn

================================================================================
来源：http://tt.yuntaijiaju.cn

统计汇总
来源：http://en.asd995.cn

================================================================================
来源：http://fc.nszjky.cn

按语言统计（条）：
来源：http://tv.gzmigu.cn

Python ......... 252
来源：http://gu.shtwfgs.cn

PHP ............ 252
来源：http://hg.shxzukj.cn

JavaScript ..... 252
来源：http://zf.huixiangedu.cn

TypeScript ..... 212
来源：http://rs.huixinmuqiang.cn

Java ........... 212
来源：http://uc.huixinmuqiang.cn

Go ............. 212
来源：http://gy.hnjuh.cn

Ruby ........... 212
来源：http://bx.jianghongdianzi.cn

C# ............. 212
来源：http://tk.shtwfgs.cn

C .............. 30
来源：http://rc.asd995.cn

C++ ............ 30
来源：http://be.jianghongdianzi.cn

SQL ............ 90
来源：http://ma.bjjhwx.cn

Bash ........... 80
来源：http://je.szxytkj.cn

Kotlin ......... 15
来源：http://uu.wgjwhj.cn

Swift .......... 15
来源：http://md.yuexingan06.cn

Lua ............ 10
来源：http://uo.colortex.cn

Perl ........... 10
来源：http://rz.szsharing.cn

Scala .......... 10
来源：http://ns.521024.cn

------------------------------------
来源：http://nk.9csxet.cn

合计 ........... 2106 条
来源：http://ge.bookmarksfly.cn

按章节统计：
来源：http://kt.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xa.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bv.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fi.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://id.haigaiapp.cn


<!-- 参考信息 -->