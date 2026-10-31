代发 wailian999

[T01] Kotlin：Hello World
来源：http://db.shtwfgs.cn

println("Hello")
来源：http://ju.colortex.cn

[T02] Kotlin：变量
来源：http://km.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ic.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://rp.asd995.cn

"值: $b"
来源：http://yx.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://pf.hahajie.cn

val n: String? = null;  n?.length
来源：http://uv.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://lr.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://me.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://sm.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xn.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://fo.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gz.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://nm.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://go.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://bd.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://kd.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://zx.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sp.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ye.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jj.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://qr.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://qk.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://py.hahajie.cn

val m = mapOf("a" to 1)
来源：http://bm.huanxung.cn

[T14] Kotlin：循环
来源：http://jr.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://at.yuexingan06.cn

[T15] Kotlin：接口
来源：http://zb.colortex.cn

interface Shape { fun area(): Double }
来源：http://sp.shtwfgs.cn

[T16] Swift：Hello World
来源：http://vg.bookmarksfly.cn

print("Hello")
来源：http://jm.szsharing.cn

[T17] Swift：变量与常量
来源：http://us.shxzskj.cn

var a = 1;  let b = 2
来源：http://ml.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://vb.chemitech.net.cn

"值: \(b)"
来源：http://nq.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://gv.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://zg.hahajie.cn

[T20] Swift：数组操作
来源：http://bu.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ps.nicolike.cn

[T21] Swift：遍历
来源：http://hg.shtwfgs.cn

for x in a { print(x) }
来源：http://cj.shxzskj.cn

[T22] Swift：字典
来源：http://zp.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gu.shtwfgs.cn

[T23] Swift：函数
来源：http://xz.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sv.newstarts.cn

[T24] Swift：闭包
来源：http://on.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://em.shxzskj.cn

[T25] Swift：结构体
来源：http://yj.shtwfgs.cn

struct P { var x: Int }
来源：http://uf.nszjky.cn

[T26] Swift：类与重写
来源：http://bf.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://sm.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://xo.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://hn.muxihuayi.cn

[T28] Swift：枚举
来源：http://ot.szsharing.cn

enum Color { case red, green }
来源：http://we.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://sr.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://lr.shtwfgs.cn

[T30] Swift：协议
来源：http://sz.colortex.cn

protocol Shape { func area() -> Double }
来源：http://yc.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://oi.gzmigu.cn

print("Hello")
来源：http://ab.wgjwhj.cn

[T32] Lua：局部变量
来源：http://gx.9csxet.cn

local a = 1
来源：http://yr.huanxung.cn

[T33] Lua：表（数组）
来源：http://tn.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yt.shxzskj.cn

[T34] Lua：遍历表
来源：http://nh.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ev.shxzskj.cn

[T35] Lua：字典表
来源：http://gk.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://ko.9csxet.cn

[T36] Lua：函数
来源：http://oo.asd995.cn

function add(a, b) return a + b end
来源：http://pi.szsharing.cn

[T37] Lua：字符串拼接
来源：http://hz.colortex.cn

"a" .. "b"
来源：http://we.bjjhwx.cn

[T38] Lua：条件
来源：http://ha.gzmigu.cn

if x > 0 then print("正") end
来源：http://up.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://yv.yuexingan06.cn

string.find(s, "%d+")
来源：http://gr.newstarts.cn

[T40] Lua：元表
来源：http://lg.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://fl.szxytkj.cn

[T41] Perl：Hello World
来源：http://hx.yuexingan06.cn

print "Hello\n";
来源：http://kz.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://ka.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rm.newstarts.cn

[T43] Perl：字符串插值
来源：http://cs.huixinmuqiang.cn

"值: $a"
来源：http://cm.huixiangedu.cn

[T44] Perl：条件
来源：http://mv.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://xh.newstarts.cn

[T45] Perl：数组遍历
来源：http://qp.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://ew.hahajie.cn

[T46] Perl：哈希操作
来源：http://ou.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ij.gzmigu.cn

[T47] Perl：正则捕获
来源：http://lg.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rq.gzmigu.cn

[T48] Perl：正则替换
来源：http://ms.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://ji.szxytkj.cn

[T49] Perl：函数
来源：http://rf.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tv.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://kt.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qu.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://am.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://lq.shxzskj.cn

println("Hello")
来源：http://nd.panjiajie.cn

[T52] Scala：变量
来源：http://vo.wgjwhj.cn

val a = 1;  var b = 2
来源：http://ah.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://ao.muxihuayi.cn

s"值: $b"
来源：http://of.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://fj.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://op.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ar.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uy.shtwfgs.cn

[T56] Scala：样例类
来源：http://fv.nszjky.cn

case class User(name: String, age: Int)
来源：http://pr.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://jl.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://op.nszjky.cn

[T58] Scala：函数定义
来源：http://sa.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xb.shxzukj.cn

[T59] Scala：循环
来源：http://hf.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://lz.panjiajie.cn

[T60] Scala：折叠
来源：http://zn.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gc.shxzukj.cn

================================================================================
来源：http://rf.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cy.chemitech.net.cn

================================================================================
来源：http://sd.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ux.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ip.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://is.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vl.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://lb.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sa.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://fq.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ks.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://hw.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://kj.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://kp.hahajie.cn

{**a, **b}
来源：http://hb.521024.cn

[U07] Py：反转字典键值
来源：http://oz.szsharing.cn

{v: k for k, v in d.items()}
来源：http://bo.huanxung.cn

[U08] Py：展平二维列表
来源：http://oo.colortex.cn

[y for x in nested for y in x]
来源：http://xb.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://uk.yuntaijiaju.cn

max(d, key=d.get)
来源：http://dh.nicolike.cn

[U10] Py：按值排序字典
来源：http://vs.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://px.huanxung.cn

[U11] Py：生成器表达式
来源：http://pv.lnxyls.cn

(x * 2 for x in arr)
来源：http://yf.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://it.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://hz.asd995.cn

[U13] Py：固定长度队列
来源：http://mu.huanxung.cn

deque(maxlen=10)
来源：http://ya.9csxet.cn

[U14] Py：分组收集到列表
来源：http://tz.wgjwhj.cn

defaultdict(list)
来源：http://vb.shtwfgs.cn

[U15] Py：高精度计时
来源：http://lz.yuexingan06.cn

t = time.perf_counter()
来源：http://nj.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://rt.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lt.muxihuayi.cn

[U17] Py：初始化日志
来源：http://sv.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://iy.521024.cn

[U18] Py：预编译正则
来源：http://ox.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://gg.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://rm.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lo.521024.cn

[U20] Py：缓存函数结果
来源：http://ij.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://yx.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://qh.chemitech.net.cn

@contextlib.contextmanager
来源：http://ea.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://er.nszjky.cn

list(zip(*m))
来源：http://wz.9csxet.cn

[U23] Py：分块读取大文件
来源：http://yw.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bi.gzmigu.cn

[U24] Py：路径操作
来源：http://dy.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ei.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://xa.9csxet.cn

csv.DictReader(f)
来源：http://zq.9csxet.cn

[U26] Py：并发下载
来源：http://dl.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mv.nicolike.cn

[U27] Py：异步 HTTP
来源：http://ph.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://td.chemitech.net.cn

[U28] Py：类型别名
来源：http://ei.huixiangedu.cn

UserId = int
来源：http://ka.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://oo.9csxet.cn

@property 与 @x.setter 配合
来源：http://kz.szxytkj.cn

[U30] Py：数据类
来源：http://nz.shtwfgs.cn

@dataclass(slots=True)
来源：http://pj.gzmigu.cn

[U31] Py：单测
来源：http://mf.lnxyls.cn

python -m pytest -q
来源：http://ir.wgjwhj.cn

[U32] Py：代码格式化
来源：http://hr.huanxung.cn

ruff format . && ruff check --fix .
来源：http://oh.gzmigu.cn

[U33] Py：打包发布
来源：http://bc.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://gx.9csxet.cn

[U34] Py：判断编码
来源：http://vl.shxzukj.cn

chardet.detect(raw)
来源：http://bu.bjjhwx.cn

[U35] Py：发送邮件
来源：http://mb.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nu.newstarts.cn

[U36] Py：定时任务
来源：http://yx.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://hy.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://nu.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bt.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://tn.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://fp.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://iv.gzmigu.cn

sys.stdout.isatty()
来源：http://pu.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://wd.521024.cn

print("err", file=sys.stderr)
来源：http://li.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://cw.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hc.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://pf.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xg.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://pl.bookmarksfly.cn

namespace App\Http;
来源：http://jk.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://le.chemitech.net.cn

declare(strict_types=1);
来源：http://us.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://nd.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kz.yuexingan06.cn

[U46] PHP：可空类型
来源：http://bl.gzmigu.cn

?string $name = null
来源：http://wk.wgjwhj.cn

[U47] PHP：联合类型
来源：http://xx.chemitech.net.cn

int|string $id
来源：http://dx.huanxung.cn

[U48] PHP：纯枚举
来源：http://at.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rd.jctech888.com.cn

[U49] PHP：只读属性
来源：http://dg.wgjwhj.cn

public readonly string $name
来源：http://ug.asd995.cn

[U50] PHP：构造器属性提升
来源：http://yu.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://zf.lnxyls.cn

[U51] PHP：数组解构
来源：http://oe.521024.cn

[$a, $b] = $arr;
来源：http://pc.nicolike.cn

[U52] PHP：箭头函数
来源：http://du.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://vg.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://sc.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://gw.shxzskj.cn

[U54] PHP：空安全调用
来源：http://tm.yuntaijiaju.cn

$obj?->method()
来源：http://ls.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://in.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oe.szsharing.cn

[U56] PHP：命名参数
来源：http://lz.huixiangedu.cn

f(a: 1, b: 2)
来源：http://tq.szxytkj.cn

[U57] PHP：字符串插值
来源：http://qp.bookmarksfly.cn

"值: {$a}"
来源：http://dj.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://nx.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://el.gzmigu.cn

[U59] PHP：自定义排序
来源：http://kx.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://og.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://rs.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ne.colortex.cn

[U61] PHP：正则
来源：http://ru.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qa.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://xl.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uh.521024.cn

[U63] PHP：文件读写
来源：http://hm.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://am.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://ft.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://xg.haigaiapp.cn

[U65] PHP：会话
来源：http://mt.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fz.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://wn.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nu.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://bg.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fu.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://az.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qw.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://vb.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uz.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://mf.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rg.nszjky.cn

[U71] PHP：抛出异常
来源：http://qs.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://qg.szxytkj.cn

[U72] PHP：写错误日志
来源：http://gx.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://fi.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://uf.asd995.cn

parse_ini_file("config.ini", true)
来源：http://dz.huanxung.cn

[U74] PHP：读取环境变量
来源：http://rv.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://zu.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://mj.yuntaijiaju.cn

composer require psr/container
来源：http://kg.chemitech.net.cn

[U76] PHP：简单路由
来源：http://nc.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rx.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://sw.lnxyls.cn

composer require twig/twig
来源：http://ev.huanxung.cn

[U78] PHP：单元测试
来源：http://ot.521024.cn

composer require --dev phpunit/phpunit
来源：http://jb.yuexingan06.cn

[U79] PHP：静态分析
来源：http://lj.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://ik.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://hb.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ck.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://lr.colortex.cn

npm init -y;  npm i express
来源：http://pt.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://mu.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eb.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://no.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://am.asd995.cn

[U84] JS：CommonJS 写法
来源：http://wq.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yl.nszjky.cn

[U85] JS：可选链
来源：http://vf.wgjwhj.cn

a?.b?.c
来源：http://gi.hahajie.cn

[U86] JS：空值合并
来源：http://zn.asd995.cn

a ?? b
来源：http://so.bjjhwx.cn

[U87] JS：解构默认值
来源：http://ws.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://of.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://jj.chemitech.net.cn

{ ...a, ...b }
来源：http://ut.asd995.cn


<!-- 参考信息 -->