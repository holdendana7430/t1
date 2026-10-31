代发 wailian999

[T03] Kotlin：字符串模板
来源：http://hh.muxihuayi.cn

"值: $b"
来源：http://vf.hahajie.cn

[T04] Kotlin：空安全
来源：http://dr.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://qs.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://oj.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jh.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://ag.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ga.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://rd.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mj.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://jk.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://qs.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://fm.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://mw.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://my.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bx.hahajie.cn

[T11] Kotlin：协程
来源：http://bo.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://um.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://td.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://gh.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://tj.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ss.muxihuayi.cn

[T14] Kotlin：循环
来源：http://na.521024.cn

for (i in 1..10) println(i)
来源：http://or.nszjky.cn

[T15] Kotlin：接口
来源：http://ou.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://qv.panjiajie.cn

[T16] Swift：Hello World
来源：http://gu.colortex.cn

print("Hello")
来源：http://yk.521024.cn

[T17] Swift：变量与常量
来源：http://bt.521024.cn

var a = 1;  let b = 2
来源：http://iw.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://dd.newstarts.cn

"值: \(b)"
来源：http://by.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://tr.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://af.muxihuayi.cn

[T20] Swift：数组操作
来源：http://sl.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zx.shxzskj.cn

[T21] Swift：遍历
来源：http://mm.newstarts.cn

for x in a { print(x) }
来源：http://xx.szxytkj.cn

[T22] Swift：字典
来源：http://dc.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dc.bookmarksfly.cn

[T23] Swift：函数
来源：http://hh.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yx.lnxyls.cn

[T24] Swift：闭包
来源：http://zw.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dh.shxzukj.cn

[T25] Swift：结构体
来源：http://gv.shtwfgs.cn

struct P { var x: Int }
来源：http://li.chemitech.net.cn

[T26] Swift：类与重写
来源：http://pd.gzmigu.cn

class A: Base { override func f() {} }
来源：http://lc.huixiangedu.cn

[T27] Swift：错误处理
来源：http://cj.521024.cn

do { try f() } catch { print(error) }
来源：http://ua.bookmarksfly.cn

[T28] Swift：枚举
来源：http://yz.huixinmuqiang.cn

enum Color { case red, green }
来源：http://nb.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://zl.bjjhwx.cn

guard let x = opt else { return }
来源：http://hh.521024.cn

[T30] Swift：协议
来源：http://sk.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://uu.huixiangedu.cn

[T31] Lua：Hello World
来源：http://dm.521024.cn

print("Hello")
来源：http://up.yuexingan06.cn

[T32] Lua：局部变量
来源：http://ex.huixiangedu.cn

local a = 1
来源：http://ng.521024.cn

[T33] Lua：表（数组）
来源：http://mc.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vi.gzmigu.cn

[T34] Lua：遍历表
来源：http://xs.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jx.nszjky.cn

[T35] Lua：字典表
来源：http://df.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://cc.huixinmuqiang.cn

[T36] Lua：函数
来源：http://oe.huixiangedu.cn

function add(a, b) return a + b end
来源：http://fb.hahajie.cn

[T37] Lua：字符串拼接
来源：http://uo.panjiajie.cn

"a" .. "b"
来源：http://ho.jianghongdianzi.cn

[T38] Lua：条件
来源：http://dc.521024.cn

if x > 0 then print("正") end
来源：http://dk.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://xs.gzmigu.cn

string.find(s, "%d+")
来源：http://zl.jctech888.com.cn

[T40] Lua：元表
来源：http://cs.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://wl.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://ep.hnjuh.cn

print "Hello\n";
来源：http://gk.nicolike.cn

[T42] Perl：变量类型
来源：http://zv.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nc.asd995.cn

[T43] Perl：字符串插值
来源：http://on.bjjhwx.cn

"值: $a"
来源：http://rp.shxzukj.cn

[T44] Perl：条件
来源：http://bj.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://tl.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://bf.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://wr.521024.cn

[T46] Perl：哈希操作
来源：http://vv.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uk.asd995.cn

[T47] Perl：正则捕获
来源：http://if.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qu.521024.cn

[T48] Perl：正则替换
来源：http://sa.lnxyls.cn

$s =~ s/old/new/g;
来源：http://jr.asd995.cn

[T49] Perl：函数
来源：http://dm.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://js.szsharing.cn

[T50] Perl：逐行读文件
来源：http://qj.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qu.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://oq.haigaiapp.cn

[T51] Scala：Hello World
来源：http://sp.nicolike.cn

println("Hello")
来源：http://ru.hahajie.cn

[T52] Scala：变量
来源：http://nd.muxihuayi.cn

val a = 1;  var b = 2
来源：http://me.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://aq.gzmigu.cn

s"值: $b"
来源：http://qu.9csxet.cn

[T54] Scala：集合映射
来源：http://il.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ws.newstarts.cn

[T55] Scala：集合过滤
来源：http://an.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qk.szsharing.cn

[T56] Scala：样例类
来源：http://bl.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://hc.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://mt.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lm.nszjky.cn

[T58] Scala：函数定义
来源：http://ji.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zu.hnjuh.cn

[T59] Scala：循环
来源：http://hk.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://xf.lnxyls.cn

[T60] Scala：折叠
来源：http://ax.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hq.wgjwhj.cn

================================================================================
来源：http://oe.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nf.hnjuh.cn

================================================================================
来源：http://gp.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://hp.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ku.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://uz.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qi.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://al.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tp.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://gp.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vv.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://ie.szsharing.cn

list(dict.fromkeys(arr))
来源：http://gx.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://pg.nicolike.cn

{**a, **b}
来源：http://ro.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://go.nicolike.cn

{v: k for k, v in d.items()}
来源：http://rz.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://yh.wgjwhj.cn

[y for x in nested for y in x]
来源：http://yd.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://lh.jianghongdianzi.cn

max(d, key=d.get)
来源：http://il.szsharing.cn

[U10] Py：按值排序字典
来源：http://pv.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oh.colortex.cn

[U11] Py：生成器表达式
来源：http://vn.nszjky.cn

(x * 2 for x in arr)
来源：http://kb.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dx.nszjky.cn

Counter(arr).most_common(3)
来源：http://vf.huanxung.cn

[U13] Py：固定长度队列
来源：http://uy.jctech888.com.cn

deque(maxlen=10)
来源：http://av.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://lg.yuntaijiaju.cn

defaultdict(list)
来源：http://lj.jctech888.com.cn

[U15] Py：高精度计时
来源：http://ry.szsharing.cn

t = time.perf_counter()
来源：http://dc.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://if.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://da.szsharing.cn

[U17] Py：初始化日志
来源：http://ho.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ne.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://ka.9csxet.cn

pat = re.compile(r"\d+")
来源：http://rh.colortex.cn

[U19] Py：正则替换带回调
来源：http://xc.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xn.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://gq.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://if.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://pd.panjiajie.cn

@contextlib.contextmanager
来源：http://th.hahajie.cn

[U22] Py：矩阵转置
来源：http://hs.colortex.cn

list(zip(*m))
来源：http://po.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://er.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ya.nszjky.cn

[U24] Py：路径操作
来源：http://wl.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iz.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://js.521024.cn

csv.DictReader(f)
来源：http://pb.9csxet.cn

[U26] Py：并发下载
来源：http://bi.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gx.nszjky.cn

[U27] Py：异步 HTTP
来源：http://uw.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://dk.bjjhwx.cn

[U28] Py：类型别名
来源：http://eb.9csxet.cn

UserId = int
来源：http://rs.gzmigu.cn

[U29] Py：属性校验
来源：http://pm.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://wn.chemitech.net.cn

[U30] Py：数据类
来源：http://tw.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://rd.hnjuh.cn

[U31] Py：单测
来源：http://zy.521024.cn

python -m pytest -q
来源：http://ae.shxzskj.cn

[U32] Py：代码格式化
来源：http://iv.huanxung.cn

ruff format . && ruff check --fix .
来源：http://df.shxzukj.cn

[U33] Py：打包发布
来源：http://lq.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://is.szxytkj.cn

[U34] Py：判断编码
来源：http://ic.bookmarksfly.cn

chardet.detect(raw)
来源：http://xe.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://sc.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://by.shtwfgs.cn

[U36] Py：定时任务
来源：http://cm.521024.cn

schedule.every(10).minutes.do(job)
来源：http://df.nszjky.cn

[U37] Py：读写 Excel
来源：http://pg.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wp.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://bx.nszjky.cn

Path(__file__).resolve().parent
来源：http://ot.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://be.szxytkj.cn

sys.stdout.isatty()
来源：http://yi.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://ww.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://yf.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://qc.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qz.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://oz.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qv.newstarts.cn

[U43] PHP：声明命名空间
来源：http://te.chemitech.net.cn

namespace App\Http;
来源：http://nj.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://bz.huanxung.cn

declare(strict_types=1);
来源：http://hf.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://vy.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ec.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://wt.huanxung.cn

?string $name = null
来源：http://ns.yuexingan06.cn

[U47] PHP：联合类型
来源：http://qp.huixinmuqiang.cn

int|string $id
来源：http://wa.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://ow.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kr.newstarts.cn

[U49] PHP：只读属性
来源：http://mi.gzmigu.cn

public readonly string $name
来源：http://dj.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://ot.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://cd.jctech888.com.cn

[U51] PHP：数组解构
来源：http://hx.gzmigu.cn

[$a, $b] = $arr;
来源：http://xq.nszjky.cn

[U52] PHP：箭头函数
来源：http://un.521024.cn

$double = fn($x) => $x * 2;
来源：http://uo.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://fq.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://qy.9csxet.cn

[U54] PHP：空安全调用
来源：http://cp.asd995.cn

$obj?->method()
来源：http://pq.nszjky.cn

[U55] PHP：match 表达式
来源：http://il.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vf.muxihuayi.cn

[U56] PHP：命名参数
来源：http://sa.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://pm.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://mq.hahajie.cn

"值: {$a}"
来源：http://ps.shxzskj.cn

[U58] PHP：数组三件套
来源：http://os.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ua.gzmigu.cn

[U59] PHP：自定义排序
来源：http://xq.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cu.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://lk.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lm.hnjuh.cn

[U61] PHP：正则
来源：http://vn.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://li.bjjhwx.cn

[U62] PHP：日期对象
来源：http://qw.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iu.nicolike.cn

[U63] PHP：文件读写
来源：http://ja.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lj.huanxung.cn

[U64] PHP：目录遍历
来源：http://tx.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://ms.bjjhwx.cn

[U65] PHP：会话
来源：http://jg.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lf.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://au.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xy.szsharing.cn

[U67] PHP：处理文件上传
来源：http://km.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yu.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://tp.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mg.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://bf.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ll.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://dw.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kr.lnxyls.cn

[U71] PHP：抛出异常
来源：http://ol.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://pw.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://nq.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://qb.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://li.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://eg.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://ao.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://ra.hahajie.cn

[U75] PHP：依赖注入
来源：http://py.bookmarksfly.cn

composer require psr/container
来源：http://nl.bjjhwx.cn

[U76] PHP：简单路由
来源：http://xf.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bd.nicolike.cn

[U77] PHP：模板渲染
来源：http://ey.lnxyls.cn

composer require twig/twig
来源：http://ik.muxihuayi.cn

[U78] PHP：单元测试
来源：http://xt.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://bb.wgjwhj.cn

[U79] PHP：静态分析
来源：http://fu.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://pz.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://nf.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jr.shtwfgs.cn

[U81] JS：初始化项目
来源：http://da.gzmigu.cn

npm init -y;  npm i express
来源：http://rv.hahajie.cn

[U82] JS：package.json 脚本
来源：http://fa.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wc.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://ut.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hh.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://ys.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gc.asd995.cn

[U85] JS：可选链
来源：http://hh.nicolike.cn

a?.b?.c
来源：http://jo.colortex.cn

[U86] JS：空值合并
来源：http://fj.szsharing.cn

a ?? b
来源：http://cr.jctech888.com.cn

[U87] JS：解构默认值
来源：http://nf.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://gd.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://ln.wgjwhj.cn

{ ...a, ...b }
来源：http://jt.521024.cn

[U89] JS：数组去重
来源：http://pd.colortex.cn

[...new Set(arr)]
来源：http://fd.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://zz.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://xu.nicolike.cn


<!-- 参考信息 -->